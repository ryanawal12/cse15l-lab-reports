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

WORKING:

Thus, through these two examples of using the command ``grep -r`` in different directories in ``./technical``, I am more clear about its use that it prints the searched pattern in the given directory recursively in all the files [(source)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/). It is a powerful search tool that can be used for the following purposes:
* Searching for specific content in web pages - If you are working on a web development project and need to search for a specific piece of content in a large set of web pages.
* Searching for source code - If working on a large software development project, ``grep -r`` can be used to search for all instances of a particular function or variable in the project directory and subdirectories.

**We have explored one use of ``grep``. Onto the next.**

## **USE 2: TO DISPLAY THE COUNT OF NUMBER OF MATCHES OF A GIVEN PATTERN/STRING ``(grep -c)``**

I used ``grep -c`` in ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical``

### *EXAMPLE 1:*

COMMAND:

```
 grep -c "personnel" ./911report/chapter-1.txt
```

The above command counts and returns the number of times the string "personnel" appears in the file ``chapter-1.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/911report``

OUTPUT:

```
12
```

Hence, we can conclude that the string "personnel" has been used 12 times in ``chapter-1.txt``

### *EXAMPLE 2:*

COMMAND:

```
grep -c "personnel" ./911report/*.txt
```

The above command counts and returns the number of times the string "personnel" appears in the all files of the pattern ``*.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/911report``

OUTPUT:

```
./911report/chapter-1.txt:12
./911report/chapter-10.txt:4
./911report/chapter-11.txt:5
./911report/chapter-12.txt:1
./911report/chapter-13.1.txt:11
./911report/chapter-13.2.txt:8
./911report/chapter-13.3.txt:1
./911report/chapter-13.4.txt:4
./911report/chapter-13.5.txt:12
./911report/chapter-2.txt:1
./911report/chapter-3.txt:8
./911report/chapter-5.txt:2
./911report/chapter-6.txt:3
./911report/chapter-7.txt:1
./911report/chapter-8.txt:4
./911report/chapter-9.txt:47
./911report/preface.txt:0
```
Hence, we can conclude that the string "personnel" has been used multiple times across the files of the pattern ``*.txt``in ``./911report``

WORKING:

Thus, we can conclude that ``grep -c`` is used to find the number of lines that matches the given string/pattern [(source)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/). 
It can be useful to check the instance count of an important phrase, or to make sure it is not too repetitive in a project. The ``grep -c`` command can only be used on files and not directly on directories.

**Moving on to the next use for ``grep``**

## **USE 3: TO SHOW THE LINE NUMBER OF THE INSTANCE OF A PATTERN/STRING IN A FILE ``(grep -n)``**

I used `` grep -n `` in ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical``

### *EXAMPLE 1:*

COMMAND:

```
 grep -n "by" ./biomed/1471-2288-3-9.txt
```

The above command lists all instances of the string/pattern "by" in the file ``1471-2288-3-9.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/biomed``

OUTPUT:

```
19:        • Two states might create a "natural experiment" by
22:        could then be computed by enumeration and arithmetic.
36:        health by tracking the number of calls to hotlines.
48:        by ignoring uncorrected confounding, selection biases,
62:        few weeks turned out to be high by a factor of two, making
96:          higher by as much as 5%, only report 2.3. This can be
111:          by reporting 2.35).
119:          inadvertently recorded and reported by two different
132:          by the minimum possible, 1, the odds ratio would either
173:            uncertain, but this is inconsequential (by the above
177:            dwarfed by that of the numerator (on the order of 1
181:            precision implied by 2.76 percent - that we are fairly
186:            estimate is that the raw estimate is low by between 0
188:            distributed. The process by which they came to this
197:            with extremely high probability, be exceeded by the
205:            misclassification error was indeed dwarfed by the
275:          uncertainty, and that goal is not well served by claiming
328:          perform and to understand) are reduced by a few factors.
365:            But greater uncertainty is introduced by the
377:            extrapolation is off by as much as 25%. To fit these
406:            is described by the continuous approximation:
416:            probability for a given value, nothing is lost by this
431:            uncertain input that entered the equation other than by
470:          and represented by a histogram that approximates the
474:          approximates the answer by carrying out simple
490:          usable by any competent quantitative researcher.
504:          various input uncertainties - is partially ameliorated by
535:          represented by one observed case (in order to extrapolate
569:          foodborne disease incidence is illustrated by the
595:          samples from monitoring efforts. They are multiplied by a
597:          incidence of each disease is then multiplied by an
602:          calculated by estimating the total cases of
618:          by a normal distribution, with a mean of the point
746:          illness caused by one pathogen is attributable to
778:        expert witness by The Delaco Company in litigation related
```

Thus, all instances of the phrase "by" are listed with their line numbers as they appear in ``1471-2288-3-9.txt``

### *EXAMPLE 2:*

COMMAND:

```
grep -n "emissions" ./government/Env_Prot_Agen/final.txt
```

The above command lists all instances of the string/pattern "emissions" in the file ``final.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/government/Env_Prot_Agen``

OUTPUT:

```
14:significantly reduce and cap NOx, SO2 and mercury emissions from
22:establish reduction targets for emissions of SO2, NOx and
39:provide market-based incentives, such as emissions
43:Nationwide reductions of the three emissions, SO2, NOx and
74:emissions that cause acid deposition and translated the emission
75:reduction goal into a nationwide cap on emissions from electric
79:certainty that the emissions reductions would be achieved and
83:accounting of their emissions through continuous monitoring and
86:for limiting SO2 emissions and to be responsible for achieving
91:emissions from power generation dropping 4.5 million tons from 1990
92:levels and NOx emissions down 1.5 million tons from 1990 levels
94:during the first Phase of the program (1995-1999), SO2 emissions
101:projected the cost of full implementation of the SO2 emissions
110:permanently caps NOx and SO2 emissions from older power plants in
120:power plant based on 1997 emissions using a formula that does not
136:significantly reduces emissions of SO2, NOx and mercury, we can
144:reductions in air emissions from electric power generation. These
146:address a variety of emissions including SO2, NOx, CO, PM10, and a
158:to adopt emissions control requirements in the form of State
163:interstate transport of NOx emissions to downwind ozone
166:19 states and the District of Columbia (whose emissions
168:to revise their SIPs to control summertime NOx emissions. In
170:focus on reducing power plant emissions. In a separate action aimed
174:rule, EPA found that emissions from large electric generating units
178:sources to control their summertime NOx emissions under the Federal
186:for example, adopted a NOx and SO2 emissions trading program
189:NOx emissions trading program (the Ozone Transport Commission NOx
191:lead to further regulation of power plant SO2 emissions (a
192:precursor to ambient PM2.5) and NOx emissions (both for PM2.5 and
199:emissions increase -- they include state-of-the-art air pollution
215:sources and major modifications must offset their emissions
228:power generators to reduce SO2 and NOx emissions either through the
234:EPA is developing a rule to limit mercury emissions from
237:can reasonably be expected to occur as a result of emissions of
246:mercury emissions.
247:The utility industry is also required to reduce SO2 emissions
250:reduce their emissions through emissions limits, which EPA
257:and limiting NOx, SO2 and mercury emissions, we can provide the
273:emissions: sulfur dioxide (SO2), nitrogen oxide (NOx), and mercury
275:successful tool in reducing these emissions. However, while we are
278:mercury. (Power generation has other emissions, such as carbon
279:monoxide and coarse particles, but the level of these emissions
282:share of these key emissions is that significant emissions
285:before federal laws limiting emissions of CO, NOx and volatile
290:pollution control equipment for some emissions.
296:SO2 and NOx emissions from power generation react in the atmosphere
299:emissions from a variety of sources.) A source emitting NOx and SO2
317:SO2 and NOx emissions. Sulfates and nitrates that form in the
318:atmosphere from SO2 and NOx emissions are significant contributors
332:many urban areas, NOx emissions from cars, trucks, and power plants
354:harsh weather). Since NOx emissions result in formation of
355:ground-level ozone, reducing NOx emissions will reduce ozone levels
363:reducing mercury air emissions. Mercury is highly toxic in small
387:emissions.
396:of annual SO2 emissions and 25 percent of NOx emissions are
401:response to reduced SO2 emissions. In sensitive areas such as the
409:declined, nitrogen emissions have not changed substantially
419:bodies by reducing NOx emissions. Some air emissions of NOx from
430:soil acidification and aluminum mobility, increased emissions from
454:synergistic effects. Beyond their impacts as separate emissions,
457:environment. In certain cases, synergies exist between emissions
459:imperative that efforts to reduce risk address all three emissions
468:large sulfur loadings over the years. Both emissions count in
474:accompanying the downward trend in emissions. However, there are
478:improving, and at best are constant. Logically, if emissions
493:U.S. man-made greenhouse gas emissions. Power generators, which
494:emit CO2, contribute abut 29% of the total emissions of all U.S.
518:determine what levels of greenhouse gas emissions need to be
520:To address global climate change and greenhouse gas emissions,
538:achieve emissions reductions most flexibly and costeffectively in
552:the emissions that cause such serious public health and
563:reduce significantly the SO2, NOx and mercury emissions from power
```

Thus, all instances of the phrase "emissions" are listed with their line numbers as they appear in ``final.txt``

WORKING:

Hence, we have seen that ``grep -n`` is used to show the line number of file with the line matched [(source)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/). This command can be useful in a variety of situations including:
* Debugging code - all instances of a faulty line/variable can be found in a roject directory to quickly correct mistakes
* Editing large files - if a particular line needs correction, the command helps you find it easily.

**And we go onto the next use for ``grep`` (Last one for the purposes of this lab report)**

## **USE 4: TO PRINT N SPECIFIC LINES FROM A FILE ``(grep -A)`` ``(grep -B)`` ``(grep -C)``**

I used ``grep -A`` ``(grep -B)`` ``(grep -C)``  in ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical``
To illustrate the uses for all 3, I shall give three examples instead of two.

### *EXAMPLE 1: ``grep -A``*

COMMAND:

```
grep -A4 "In a separate action aimed" ./government/Env_Prot_Agen/final.txt
```

The above command prints the line in which the searched pattern exists in the path given, and 4 lines after it. The 4 after ``grep -A`` refers to the number of lines to be printed after the search term line. 

OUTPUT:

```
focus on reducing power plant emissions. In a separate action aimed
at the same interstate NOx transport problem, in January 2000, EPA
finalized a rule which was issued in response to petitions from
several northeastern states under section 126 of the CAA. In this
rule, EPA found that emissions from large electric generating units

```

Thus, the command has printed the line in which the phrase "In a separate action aimed" exists, and 4 lines after it that exist in ``final.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/government/Env_Prot_Agen``

### *EXAMPLE 2: ``grep -B``*

COMMAND:

```
grep -B10 "Our aim has not been to assign individual blame." ./911report/preface.txt
```

The above command prints the line in which the searched pattern exists in the path given, and 10 lines before it. The 10 after ``grep -B`` refers to the number of lines to be printed before the search term line. 

OUTPUT:

```
and border control, the flow of assets to terrorist organizations, commercial
                aviation, the role of congressional oversight and resource allocation, and other
                areas determined relevant by the Commission. In pursuing our mandate, we have
                reviewed more than 2.5 million pages of documents and interviewed more than 1,200
                individuals in ten countries. This included nearly every senior official from the
                current and previous administrations who had responsibility for topics covered in
                our mandate. We have sought to be independent, impartial, thorough, and nonpartisan.
                From the outset, we have been committed to share as much of our investigation as we
                can with the American people. To that end, we held 19 days of hearings and took
                public testimony from 160 witnesses.
            Our aim has not been to assign individual blame. Our aim has been to provide the

```

Thus, the command has printed the line in which the phrase "Our aim has not been to assign individual blame." exists, and 10 lines before it that exist in ``preface.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/911report``

### *EXAMPLE 3: ``grep -C``*

COMMAND:

```
grep -C3 "Before national implementation of the Nursing Home" ./biomed/1471-2318-3-2.txt
```

The above command prints the line in which the searched pattern exists in the path given, and 3 lines before and after it. The 3 after ``grep -C`` refers to the number of lines to be printed before the search term line. 

OUTPUT:

```
community-based quality improvement assistance programs to
        nursing home providers seeking to improve their performance
        on the Quality Measures.
        Before national implementation of the Nursing Home
        Quality Initiative in November 2002, CMS conducted a pilot
        in six states: Colorado, Florida, Maryland, Ohio, Rhode
        Island, and Washington. QIO quality improvement activities
```

Thus, the command has printed the line in which the phrase "Before national implementation of the Nursing Home" exists, and 3 lines before and after it that exist in ``1471-2318-3-2.txt`` in the directory ``/home/linux/ieng6/cs15lsp23/cs15lsp23hh/stringsearch/stringsearch-data/technical/biomed``

WORKING:

Hence we have explored the uses of this group of commands - ``grep -A`` ``grep -B`` ``grep -C``
While ``grep -A`` prints the searched line in the given file and n lines after it, ``grep -B`` does the same but prints n lines that exist before it and ``grep -C`` prints both - n lines before and after it [(source)](https://www.geeksforgeeks.org/grep-command-in-unixlinux/).
Some practical uses for these commands would include situations where one is parsing a lot of files and can get a short summary/ context of what each file is right on the terminal. It can also be useful while going through errors and warnings in code, as the erroneous code before warnings or the error message after the code can be brought to the terminal. They are also especially great to work with when parsing log files.



**Thus we have explored 4 different uses for ``grep``. I look forward to understanding other commands and their alternate uses as well. They really help ease workload when working with software**
