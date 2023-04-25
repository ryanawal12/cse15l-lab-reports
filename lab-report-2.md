## **PART 1**

In Part 1, I will create a web server called ``StringServer`` that supports the path and behavior described in [Lab Report 2 - Servers and Bugs (Week 3)](https://ucsd-cse15l-s23.github.io/week/week3/#week3-lab-report). The ``StringServer`` class keeps track of a string and responds with it every time the URI is visited. The requests in the URI look like ```/add-message?s=<string>``` and every time it runs, the new string is printed on a new line using ``("\n")``

The Code for StringServer is as follows. I have used a lot of the code from the Lab 2 wavelet repository and made modifications in accordance with the requirements of this web server.

```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String s = "";
    String test = "hi";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format("");
        } 
        else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                
                if (parameters[0].equals("s"))
                {
                    s+= parameters[1]+"\n";
                }
                return s;
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```

After writing this code, committing and pushing it, I compiled the java files and started the server, using the techniques taught in [LAB 2](https://ucsd-cse15l-s23.github.io/week/week2/#building-and-running-the-server)
Here is a screenshot of my doing this in the terminal:

![Image](Running the server.png)

I then used the link ``(http://localhost:4029)`` in the browser and added a query of the format ```/add-message?s=<string>``` My first string was "Hello" and you can see the output in the screenshot below:

![Image](ADD MESSAGE 1.png)

Using ```/add-message?s=Hello``` , my ```String handleRequest(URI url)``` method is called. ```url``` is the argument for this method that gets the whole URL => ```http://localhost:4029/add-message?s=Hello``` Then ```url.getPath()``` gets the path part of the address. At this point String s is empty. The array of strings ``parameters`` takes the query part, which is ``s=Hello`` which is split at the "=" using the method ```split("=")``` that is also called.
Now ``parameters`` has ``{"s","Hello"}``. At this point the string s gets updated to contain ``"Hello\n"``

Onto the next message with the string "How are you. My name is Ryan Awal"

![Image](ADD MESSAGE 2.png)

Using ```/add-message?s=How%20are%20you.%20My%20name%20is%20Ryan%20Awal``` , my ```String handleRequest(URI url)``` method is called. ```url``` is the argument for this method that gets the whole URL => ```http://localhost:4029/add-message?s=How%20are%20you.%20My%20name%20is%20Ryan%20Awal``` Then ```url.getPath()``` gets the path part of the address. At this point String s has ``"Hello\n"``. The array of strings ``parameters`` takes the query part, which is ``s=Hello`` which is split at the "=" using the method ```split("=")``` that is also called.
Now ``parameters`` has ``{"s","How%20are%20you.%20My%20name%20is%20Ryan%20Awal"}``. At this point the string s gets updated to contain ``"Hello\nHow are you. My name is Ryan Awal\n"``

## **PART 2**


