## **PART 1**

In Part 1, I will create a web server called ``StringServer`` that supports the path and behavior described in [Lab Report 2 - Servers and Bugs (Week 3)](https://ucsd-cse15l-s23.github.io/week/week3/#week3-lab-report). The ``StringServer`` class keeps track of a string and responds with it every time the URI is visited. The requests in the URI look like ```/add-message?s=<string>``` and every time it runs, the new string is printed on a new line using ``("\n")``

The Code for StringServer is as follows. I have used a lot of the code from the Lab 2 wavelet repository and made modifications in accordance with the requirements of this web server.

```
{
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
}
```

