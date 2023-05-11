# **LAB REPORT 3 - RESEARCHING COMMANDS (grep)**

In this lab report, I will be going over 4 alternate uses for the ``grep`` command, including 2 examples in the path ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical`` for each of the 4 uses.

I researched the uses of grep using first the ``man grep`` command on the terminal to open the manual. I then used ChatGPT and [this link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/) to further my knowledge. This is what I came up with:

## **USE 1 : TO SEARCH FOR A PATTERN RECURSIVELY IN A DIRECTORY  ``(grep -r)``**

I used `` grep -r `` in ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical``

### *EXAMPLE 1:*

COMMAND:

```
grep -r "air traffic control" ./911report
```

The above command searches recursively through all the files in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/911report`` for the string pattern "air traffic control"

OUTPUT:

```
./911report/chapter-1.txt:    At that same time, American 11 had its last routine communication with the ground when it acknowledged navigational instructions from the FAA's air traffic control (ATC) center in Boston. Sixteen seconds after that transmission, ATC instructed the aircraft's pilots to climb to 35,000 feet. That message and all subsequent attempts to contact the flight were not acknowledged. From this and other evidence, we believe the hijacking began at 8:14 or shortly thereafter.
./911report/chapter-1.txt:    At 8:21, one of the American employees receiving Ong's call in North Carolina, Nydia Gonzalez, alerted the American Airlines operations center in Fort Worth, Texas, reaching Craig Marquis, the manager on duty. Marquis soon realized this was an emergency and instructed the airline's dispatcher responsible for the flight to contact the cockpit. At 8:23, the dispatcher tried unsuccessfully to contact the aircraft. Six minutes later, the air traffic control specialist in American's operations center contacted the FAA's Boston Air Traffic Control Center about the flight. The center was already aware of the problem.
./911report/chapter-1.txt:    Boston Center knew of a problem on the flight in part because just before 8:25 the hijackers had attempted to communicate with the passengers. The microphone was keyed, and immediately one of the hijackers said, "Nobody move. Everything will be okay. If you try to make any moves, you'll endanger yourself and the airplane. Just stay quiet." Air traffic controllers heard the transmission; Ong did not. The hijackers probably did not know how to operate the cockpit radio communication system correctly, and thus inadvertently broadcast their message over the air traffic control channel instead of the cabin public-address channel. Also at 8:25, and again at 8:29, Amy Sweeney got through to the American Flight Services Office in Boston but was cut off after she reported someone was hurt aboard the flight. Three minutes later, Sweeney was reconnected to the office and began relaying updates to the manager, Michael Woodward.
./911report/chapter-1.txt:    At 8:41, in American's operations center, a colleague told Marquis that the air traffic controllers declared Flight 11 a hijacking and "think he's [American 11] headed toward Kennedy [airport in New York City]. They're moving everybody out of the way. They seem to have him on a primary radar. They seem to think that he is descending."
./911report/chapter-1.txt:    The first operational evidence that something was abnormal on United 175 came at 8:47, when the aircraft changed beacon codes twice within a minute. At 8:51, the flight deviated from its assigned altitude, and a minute later New York air traffic controllers began repeatedly and unsuccessfully trying to contact it.
./911report/chapter-1.txt:    Several FAA air traffic control officials told us it was the air carriers' responsibility to notify their planes of security problems. One senior FAA air traffic control manager said that it was simply not the FAA's place to order the airlines what to tell their pilots.
./911report/chapter-1.txt:    The hijackers attacked at 9:28. While traveling 35,000 feet above eastern Ohio, United 93 suddenly dropped 700 feet. Eleven seconds into the descent, the FAA's air traffic control center in Cleveland received the first of two radio transmissions from the aircraft. During the first broadcast, the captain or first officer could be heard declaring "Mayday" amid the sounds of a physical struggle in the cockpit. The second radio transmission, 35 seconds later, indicated that the fight was continuing. The captain or first officer could be heard shouting:" Hey get out of here-get out of here-get out of here."
./911report/chapter-1.txt:    On 9/11, the defense of U.S. airspace depended on close interaction between two federal agencies: the FAA and the North American Aerospace Defense Command (NORAD). The most recent hijacking that involved U.S. air traffic controllers, FAA management, and military coordination had occurred in 1993.90 In order to understand how the two agencies interacted eight years later, we will review their missions, command and control structures, and working relationship on the morning of 9/11.
./911report/chapter-1.txt:    FAA Mission and Structure. As of September 11, 2001, the FAA was mandated by law to regulate the safety and security of civil aviation. From an air traffic controller's perspective, that meant maintaining a safe distance between airborne aircraft.
./911report/chapter-1.txt:    The NMCC would keep the FAA hijack coordinator up to date and help the FAA centers coordinate directly with the military. NORAD would receive tracking information for the hijacked aircraft either from joint use radar or from the relevant FAA air traffic control facility. Every attempt would be made to have the hijacked aircraft squawk 7500 to help NORAD track it.
./911report/chapter-1.txt:FAA Awareness. Although the Boston Center air traffic controller realized at an early stage that there was something wrong with American 11, he did not immediately interpret the plane's failure to respond as a sign that it had been hijacked. At 8:14, when the flight failed to heed his instruction to climb to 35,000 feet, the controller repeatedly tried to raise the flight. He reached out to the pilot on the emergency frequency. Though there was no response, he kept trying to contact the aircraft.
./911report/chapter-1.txt:    Minutes later, United 175 turned southwest without clearance from air traffic control. At 8:47, seconds after the impact of American 11, United 175's transponder code changed, and then changed again. These changes were not noticed for several minutes, however, because the same New York Center controller was assigned to both American 11 and United 175. The controller knew American 11 was hijacked; he was focused on searching for it after the aircraft disappeared at 8:46.
./911report/chapter-1.txt:    At 9:42, the Command Center learned from news reports that a plane had struck the Pentagon. The Command Center's national operations manager, Ben Sliney, ordered all FAA facilities to instruct all aircraft to land at the nearest airport. This was an unprecedented order. The air traffic control system handled it with great skill, as about 4,500 commercial and general aviation aircraft soon landed without incident.
./911report/chapter-1.txt:    United 93 crashed in Pennsylvania at 10:03:11, 125 miles from Washington, D.C. The precise crash time has been the subject of some dispute. The 10:03:11 impact time is supported by previous National Transportation Safety Board analysis and by evidence from the Commission staff 's analysis of radar, the flight data recorder, the cockpit voice recorder, infrared satellite data, and air traffic control transmissions.
./911report/chapter-13.2.txt:            23. Commission analysis of NTSB and FAA air traffic control and radar data. See AAL
./911report/chapter-13.2.txt:                previous instructions from air traffic control that morning within a matter of
./911report/chapter-13.2.txt:            42. Asked by air traffic controllers at 8:37 to look for an American Airlines 767
./911report/chapter-13.2.txt:            64. Commission analysis of FAA air traffic control data. On the FAA's awareness of
./911report/chapter-13.2.txt:            68. Ellen King interview (Apr. 5, 2004). FAA air traffic control tapes indicate that
./911report/chapter-13.2.txt:                FAA centers, we learned that an air traffic controller's first response to an
./911report/chapter-13.2.txt:                was 9:03:11 based on our analysis of FAA radar data and air traffic control software
./911report/chapter-13.2.txt:            138. Commission analysis of FAA radar data and air traffic control transmissions.
./911report/chapter-13.2.txt:                Pentagon is based on Commission analysis of FDR, air traffic control, radar, and
./911report/chapter-13.5.txt:                Commission analysis of FAA radar data and air traffic control software logic. For
./911report/chapter-13.5.txt:                Sheets," Sept. 11, 2001. For communications with air traffic controllers and their
./911report/chapter-13.5.txt:                returns and Commission analysis of FAA radar data and air traffic control software
./911report/chapter-3.txt:                medical services, air traffic control, financial services, telephone systems, and
./911report/chapter-9.txt:                airplane crash at the World Trade Center. The air traffic controllers had been

```

Thus, we can see that this command has parsed through all the files in the directory ``./technical/911report`` and returned the file name and the lines which contain instances of the phrase "air traffic control"

### *EXAMPLE 2:*

COMMAND: 

```
grep -r "Legal aid" ./government/Media
```

The above command searches recursively through all the files in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/government/Media`` for the string pattern "Legal aid"

OUTPUT:

```
./government/Media/Anthem_Payout.txt:Legal aid lawyers in Kentucky have put together an action team
./government/Media/Barnes_pro_bono.txt:Legal aid's volunteer lawyers work on behalf of low-income
./government/Media/Barnes_pro_bono.txt:protect borrowers from socalled "predatory lenders." Legal aid
./government/Media/BergenCountyRecord.txt:Legal aid unit fights for survival
./government/Media/Farm_workers.txt:Report: Farm workers plagued by pesticides Legal aid group
./government/Media/Funds_Shortage.txt:Foundation. Legal aid providers in the state are already scrounging
./government/Media/Lockyer_Warns.txt:Legal aid services are nonprofit, publicly funded organizations
./government/Media/Pro_Bono_Services.txt:Legal aid organizations are in great need of increased
./government/Media/The_Bend_Bulletin.txt:"Legal aid is so important for our community and country because
```

Thus, we can see that this command has parsed through all the files in the directory ``./technical/government/Media`` and returned the file name and the lines which contain instances of the phrase "Legal Aid"


Thus, through these two examples of using the command ``grep -r`` in different directories in ``./technical``, I am more clear about its use --> It prints the searched pattern in the given directory recursively in all the files [Source](https://www.geeksforgeeks.org/grep-command-in-unixlinux/). It is a powerful search tool that can be used for the following purposes:
* Searching for specific content in web pages - If you are working on a web development project and need to search for a specific piece of content in a large set of web pages.
* Searching for source code - If working on a large software development project, ``grep -r`` can be used to search for all instances of a particular function or variable in the project directory and subdirectories.

We have explored one use of ``grep``. Onto the next.

## **USE 2: TO DISPLAY THE COUNT OF NUMBER OF MATCHES OF A GIVEN PATTERN/STRING ``(grep -c)``**

I used ``grep -c`` in ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical``

### *EXAMPLE 1:*

COMMAND

```

```




