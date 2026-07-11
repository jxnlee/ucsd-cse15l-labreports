# Lab Report 3: Researching Commands

---

## Chosen Command: grep

## 1. Command Option 1: `-r`

### This command option can be applied in the format of `grep -r <string-pattern>` and allows the `grep` command to recursively read through files in directories for the given string pattern. The output for this command lists all of the files and all of the lines contained in those files that contain the specified string pattern. Below are a few examples:

For this example I recursively searched through all the directories in the `technical` directory for the word `"everyone"` by writing `grep -r "everyone"`, this allows the command to scan through each of the files in each directory and search for lines that contain the given word `"everyone"` before outputting the line and filepath that contains the word. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:112$ grep -r "everyone"
911report/chapter-1.txt:    UAL 175: Yeah. We figured we'd wait to go to your center. Ah, we heard a suspicious transmission on our departure out of Boston, ah, with someone, ah, it sounded like someone keyed the mikes and said ah everyone ah stay in your seats.
911report/chapter-1.txt:    When they learned a second plane had struck the World Trade Center, nearly everyone in the White House told us, they immediately knew it was not an accident. The Secret Service initiated a number of security enhancements around the White House complex. The officials who issued these orders did not know that there were additional hijacked aircraft, or that one such aircraft was en route to Washington. These measures were precautionary steps taken because of the strikes in New York.
911report/chapter-11.txt:                is that everyone had the job. The CIA's deputy director for operations, James
911report/chapter-11.txt:            Headquarters tended to support and facilitate, trying to make sure everyone was in
911report/chapter-11.txt:            Why was this so? Most obviously, it was because everyone was already on edge with the
911report/chapter-13.2.txt:                after takeoff,"like someone keyed the mike and said everyone stay in your seats."
911report/chapter-13.5.txt:                those that everyone assumes somebody else is taking care of. It includes
911report/chapter-3.txt:                the FBI field offices in the United States, everyone in the Directorate of
911report/chapter-3.txt:                last sighting of Bin Ladin and that this persuaded everyone that the chance of
911report/chapter-3.txt:                dangerous, and it played more to their skills and experience. But everyone knew that
911report/chapter-3.txt:                QAEDA'S INITIAL ASSAULTS 135 and do something that everyone would later regret.
911report/chapter-5.txt:                insisted that everyone he had selected receive the training.
911report/chapter-7.txt:                Although Khallad claims not to recall everyone from this group who was later chosen
911report/chapter-8.txt:                said, it could not "get any worse." Not everyone was
911report/chapter-8.txt:            It is now clear that everyone involved was confused about the rules governing the
911report/chapter-9.txt:                channel and repeated it to everyone they came across. The chief on the 23rd floor
biomed/1472-6947-2-7.txt:            everyone can talk as long as they speak English).
biomed/1475-2875-1-14.txt:          everyone in the household sleeps under a bednet every
biomed/1475-2875-1-14.txt:        everyone in a household sleeps under a bednet indicates
biomed/1475-2875-1-14.txt:        methods of protection or whether everyone in the house
government/About_LSC/ONTARIO_LEGAL_AID_SERIES.txt:halls of justice must always stand wide open and everyone must be
government/Alcohol_Problems/DraftRecom-PDF.txt:However, in emergency medicine, everyone gets a referral-to primary
government/Alcohol_Problems/Session3-PDF.txt:work for everyone.
government/Alcohol_Problems/Session3-PDF.txt:percentage of hazardous drinkers, it is not effective for everyone
government/Alcohol_Problems/Session3-PDF.txt:everyone, she responds to patients who request help. However,
government/Gen_Account_Office/May1998_ai98068.txt:The groups focused their efforts on increasing everyone's
government/Gen_Account_Office/Sept14-2002_d011070.txt:organization so that everyone understands what the organization is
government/Gen_Account_Office/Sept14-2002_d011070.txt:performance information provided everyone with a focus to work
government/Gen_Account_Office/Sept14-2002_d011070.txt:changes because everyone has a stake in helping to shape and
government/Gen_Account_Office/ai9868.txt:The groups focused their efforts on increasing everyone's
government/Gen_Account_Office/d01591sp.txt:Not everyone behaves like a life-cycle saver. Many people plan
government/Gen_Account_Office/d0269g.txt:everyone from program managers to staff performing day-to-day
government/Gen_Account_Office/d0269g.txt:management becomes the business of everyone in the
government/Gen_Account_Office/d0269g.txt:engaging everyone in the organization in the risk management
government/Gen_Account_Office/d0269g.txt:"Control activities will not be fully effective until everyone,
government/Gen_Account_Office/pe1019.txt:Almost everyone in GAO probably has worked on a case study at
government/Media/Assuring_Underprivileged.txt:in making everyone in her courtroom at ease.
government/Media/Assuring_Underprivileged.txt:"She treats everyone, from victims to defendants to attorneys,
government/Media/Barnes_Volunteers.txt:lawyers have a responsibility to make sure that everyone,
government/Media/Coup_Reshapes_Legal_Aid.txt:everyone," a longtime observer of the public interest community
government/Media/Donald_Hilliker.txt:system for everyone, whether they have the ability to pay or not,"
government/Media/Good_guys_reward.txt:Allentown, a former law partner. ''He sees everyone as being
government/Media/GreensburgDailyNews.txt:judiciary] of the government is working for everyone. I'm so
government/Media/Legal-aid_chief.txt:Doug German's beliefs in treating everyone fairly and holding those
government/Media/Legal_Aid_campaign.txt:economy, and the elderly. It is important to guarantee everyone
government/Media/Lindsays_legacy.txt:"I think that's the kind of effect Jim Lindsay has on everyone
government/Media/Raising_the_Bar.txt:per lawyer to make up for the shortfall. Just about everyone came
government/Media/Volunteers_Step_Up.txt:everyone, and even the least powerful can seek justice, against the
government/Media/Volunteers_Step_Up.txt:under law for everyone.
government/Media/families_saved.txt:everyone."
government/Media/man_on_national_team.txt:made a great impression on everyone at the meetings.
government/Media/not_accessible_to_disabled.txt:condominiums as everyone else," said Ralph F. Boyd Jr., assistant
government/Post_Rate_Comm/Gleiman_EMASpeech.txt:for additional revenue. As a result, almost everyone received a
government/Post_Rate_Comm/Gleiman_EMASpeech.txt:engine that enables everyone to word search these documents.
government/Post_Rate_Comm/Gleiman_gca2000.txt:when almost everyone else got a break?" There are usually a number
government/Post_Rate_Comm/Gleiman_gca2000.txt:it is important for everyone to understand the extent to which
government/Post_Rate_Comm/Gleiman_gca2000.txt:disaster for everyone up and down the chain from graphics and copy
government/Post_Rate_Comm/Gleiman_gca2000.txt:result could be a framework everyone can live with.
plos/journal.pbio.0020028.txt:        biotech companies have bet their futures on it, but not everyone is sanguine about the
plos/journal.pbio.0020052.txt:        R&D eventually benefit everyone. But granting a 20-year marketing monopoly on a
plos/journal.pbio.0020067.txt:        world's leading structural chemist into the race reawakened everyone to the centrality of
plos/journal.pbio.0020150.txt:        What everyone apparently already agrees on is the need for carefully designed
plos/journal.pbio.0020164.txt:        everyone's lips.
plos/journal.pbio.0020183.txt:        biological diversity has produced a semantic muddle among biologists—everyone who thinks
plos/journal.pbio.0020183.txt:        something often lacking in the field. Not everyone agrees that it makes sense to define the
plos/journal.pbio.0020183.txt:        them to mate with everyone except those belonging to the same “mating type” (this is
plos/journal.pbio.0020228.txt:        with students and faculty at elite Western universities, but with everyone who could use it
plos/pmed.0010010.txt:        delivery of prevention messages and life-saving medications to everyone in Africa—and
plos/pmed.0010039.txt:        an equitable, affordable system for everyone. Instead, the AMA has supported an agenda that
plos/pmed.0010039.txt:        low-income individuals, would be used to cover everyone else. Many simulation studies have
plos/pmed.0010039.txt:        shown that these approaches could be effective in covering almost everyone, but they are
plos/pmed.0010039.txt:        everyone, and that they are the least expensive models [14]. By integrating funding with
plos/pmed.0010039.txt:        Medicare and then using the program to cover everyone may be a concept that can gain
plos/pmed.0020035.txt:        strategic plan with everyone affected by the AIDS pandemic—that is, all of us—by publishing
plos/pmed.0020047.txt:        making it freely accessible to all and letting everyone redistribute it. I give a vote of
plos/pmed.0020050.txt:        everyone that could potentially benefit from ARVs will be able to access them. Many of the
plos/pmed.0020098.txt:        everyone early on who is at any increased risk by measure of the expanded risk factors
plos/pmed.0020102.txt:        everyone deserves to be treated with dignity—this is the tenet from which all other human
plos/pmed.0020102.txt:        Despite the acknowledged importance of counting everyone, only 57 of the 192 WHO member
plos/pmed.0020189.txt:        future. Not everyone has a heart attack but everyone ages, nor can we be sure who will be
plos/pmed.0020189.txt:        policies meant for masses. Shouldn't everyone with increased IMT at least be informed of
plos/pmed.0020238.txt:        damage (neuropathic pain) caused by the shingles. Not everyone who has had shingles
plos/pmed.0020246.txt:            1. The States Parties to the present Covenant recognize the right of everyone to
plos/pmed.0020247.txt:        of HIV-testing programs across sub-Saharan Africa, because in most villages everyone
plos/pmed.0020247.txt:        everyone [3].
plos/pmed.0020247.txt:        through casual contact, and outside they fear the gossip that can greatly affect everyone's
```

For this example I recursively searched through all the directories in the `technical` directory for the word `"apple"` by writing `grep -r "apple"`, this allows the command to scan through each of the files in each directory and search for lines that contain the given word `"apple"` before outputting the line and filepath that contains the word. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:114$ grep -r "apple"
911report/chapter-8.txt:                grappled with reports alleging plots in Yemen and Italy, as well as a report about a
biomed/1468-6708-3-10.txt:        questions requiring large sample sizes and to grapple with
biomed/1471-2105-3-12.txt:            This problem appears to lie in the JAVA applet included
biomed/1471-2105-3-12.txt:            applet-generated graph may be problematic due to an
biomed/1471-2105-3-12.txt:            applet incompatibility; capturing the graph as a
biomed/1471-2202-2-5.txt:            computer http://www.apple.com. If the criteria for
biomed/1471-2458-3-11.txt:        fresh-pressed apple cider [ 28 ] . Other foodborne
biomed/1472-6882-1-10.txt:          antibiotics and the ananase enzyme (from the pineapple
biomed/gb-2002-3-10-research0053.txt:          in pineapple (~70% to
biomed/gb-2002-3-12-research0077.txt:          the JAVA applet WebMol [ 35]. In this setting, the color
biomed/gb-2003-4-8-r51.txt:            visualized using QuickPDB, a Java applet developed by
government/About_LSC/commission_report.txt:apples (4,428), vegetable harvesting (4,822), and fruit harvesting
government/About_LSC/commission_report.txt:the October apple harvest, and then return to Mexico until the work
government/About_LSC/commission_report.txt:apple harvest. See April Comments at 101 (comment of Garry G.
government/Gen_Account_Office/Oct15-2001_d0224.txt:incidents has proven to be challenging as organizations grapple
government/Gen_Account_Office/Testimony_cg00010t.txt:Clearly, much has already changed as GAO has grappled with this
government/Gen_Account_Office/Testimony_cg00010t.txt:grapples with increasingly complex and contentious issues requiring
government/Media/Law_Schools.txt:government post. Here is how to grapple "in the service of
plos/pmed.0010013.txt:        easier to grapple with a difficult, but ultimately soluble, basic science question than to
```

This command option `-r` is useful as it allows one to identitify all of the lines and files in directories that contain a keyword. This can be used in situations where I am trying to collect all of the files that may contain information about something specific, rather than only being able to retrieve from a single file or a single directory, I can scan through multiple options of files and directories for the information one needs.

_Source: I found out about this grep option from [this article about grep commands](https://www.tutorialspoint.com/unix_commands/grep.htm) and through the command `grep --help` pages_

## 2. Command Option 2: `-l`

### This command option can be applied in the format of `grep -l <string-pattern> <filepath>` and allows the `grep` command to list all of the distinct files that contain the string matching to the given string-pattern. Below are a few examples:

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files that contain the string `"everyone"` by writing `grep -l "everyone" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and then return and output all of the distinct files that have the matching string value to the word `"everyone"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:104$ grep -l "everyone" 911report/*.txt
911report/chapter-1.txt
911report/chapter-11.txt
911report/chapter-13.2.txt
911report/chapter-13.5.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-7.txt
911report/chapter-8.txt
911report/chapter-9.txt
```

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files that contain the string `"fire"` by writing `grep -l "fire" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and then return and output all of the distinct files that have the matching string value to the word `"fire"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:105$ grep -l "fire" 911report/*.txt
911report/chapter-1.txt
911report/chapter-10.txt
911report/chapter-11.txt
911report/chapter-13.1.txt
911report/chapter-13.2.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-13.5.txt
911report/chapter-2.txt
911report/chapter-3.txt
911report/chapter-5.txt
911report/chapter-6.txt
911report/chapter-7.txt
911report/chapter-9.txt
```

This command option `-l` is useful as it allows one to identify all of the distinct files that contain the information they are looking for (through the given string pattern). If one were to look only for the files that contain the information, the grep command (along with some other options) additionally outputting the lines that contain the information would add unnecessary noise to the output, making it more confusing since some files may have multiple references to the string, and therefore one would not need to account for repetition in files and can find the distinct files with the desired information through this `grep` command option.

_Source: I found out about this grep option from [this article about grep commands](https://www.tutorialspoint.com/unix_commands/grep.htm) and through the command `grep --help` pages_

## 3. Command Option 3: `-L`

### This command option can be applied in the format of `grep -L <string-pattern> <filepath>` and allows the `grep` command to list all of the distinct files that do not contain the string matching to the given string-pattern. This funcitons similar to the `-l` option but in the opposite case where you want the files that do not match with the given string pattern. Below are a few examples:

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files that do not contain the string `"everyone"` by writing `grep -L "everyone" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and then return and output all of the distinct files that do not have the matching string value to the word `"everyone"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:110$ grep -L "everyone" 911report/*.txt
911report/chapter-10.txt
911report/chapter-12.txt
911report/chapter-13.1.txt
911report/chapter-13.3.txt
911report/chapter-13.4.txt
911report/chapter-2.txt
911report/chapter-6.txt
911report/preface.txt
```

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files that do not contain the string `"fire"` by writing `grep -L "fire" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and then return and output all of the distinct files that do not have the matching string value to the word `"fire"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:107$ grep -L "fire" 911report/*.txt
911report/chapter-12.txt
911report/chapter-8.txt
911report/preface.txt
```

This command option `-L` is useful as it functions similarly to teh `-l` command option but just the opposite as it allows one to identify all of the distinct files that do not contain information that one hopes to ignore (through the given string pattern). If one were to look only for the files that do not contain some information, the grep command (along with some other options) will make it difficult when you are trying to filter through files to search for specific information, and the lines that contain the information would add unnecessary noise to the output; all of this makes it more confusing. This `grep` command option allows one to better filter and sort through data when one knows what the files should not contain.

_Source: I found out about this grep option from [this article about grep commands](https://www.tutorialspoint.com/unix_commands/grep.htm) and through the command `grep --help` pages_

## 4. Command Option 4: `-c`

### This command option can be applied in the format of `grep -c <string-pattern> <filepath>` and allows the `grep` command to list all of the distinct files that contain matching string to the given string pattern along with the number of lines/times the given string occurs in the file. Below are a few examples:

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files and the lines in those files that contain the string `"everyone"` by writing `grep -c "everyone" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and their lines before returning and displaying their filepath that contains the word and the number of occurences of the string `"everyone"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:109$ grep -c "everyone" 911report/*.txt
911report/chapter-1.txt:2
911report/chapter-10.txt:0
911report/chapter-11.txt:3
911report/chapter-12.txt:0
911report/chapter-13.1.txt:0
911report/chapter-13.2.txt:1
911report/chapter-13.3.txt:0
911report/chapter-13.4.txt:0
911report/chapter-13.5.txt:1
911report/chapter-2.txt:0
911report/chapter-3.txt:4
911report/chapter-5.txt:1
911report/chapter-6.txt:0
911report/chapter-7.txt:1
911report/chapter-8.txt:2
911report/chapter-9.txt:1
911report/preface.txt:0
```

For this example I searched through all of the `txt` files in the `911report` directory in the `technical` directory for files and the lines in those files that contain the string `"fire"` by writing `grep -c "fire" 911report/*.txt`, this allows the command to scan through all of the `txt` files (given by the pattern `*.txt`) and their lines before returning and displaying their filepath that contains the word and the number of occurences of the string `"fire"`. Here is the resulting output in the terminal:

```
[cs15lsp23if@ieng6-202]:technical:106$ grep -c "fire" 911report/*.txt
911report/chapter-1.txt:1
911report/chapter-10.txt:1
911report/chapter-11.txt:1
911report/chapter-12.txt:0
911report/chapter-13.1.txt:4
911report/chapter-13.2.txt:3
911report/chapter-13.3.txt:1
911report/chapter-13.4.txt:2
911report/chapter-13.5.txt:57
911report/chapter-2.txt:1
911report/chapter-3.txt:6
911report/chapter-5.txt:1
911report/chapter-6.txt:4
911report/chapter-7.txt:1
911report/chapter-8.txt:0
911report/chapter-9.txt:145
911report/preface.txt:0
```

This command option `-c` is useful as it allows one to have a quick glance and understand the distribution of the occurence of the given string pattern throughout the given directory of files. With this command option, one can understand how frequently certain words occur in the files and better identify which files may be of better use if we hope to find information pertaining to a subject. This command is especially useful as it provides a cursory and comprehensive glance at all of the files and how they could relate to the given string pattern. Rather than outputting specific lines or only looking at the files that may or may not contain a certain word, this command option providesa information on which files contain the word and how often certain files use them.

_Source: I found out about this grep option from [this article about grep commands](https://www.tutorialspoint.com/unix_commands/grep.htm) and through the command `grep --help` pages_
