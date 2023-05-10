# **Lab Report 3 - Researching Commands**

## The Grep Command

### grep -i

##### Example 1

        $ grep There -i biomed/1468-6708-3-7.txt
        
        [ 1 ] . Prior to this publication, there had been no
        there has been a large body of literature dedicated to the
          frequently prescribed for hypertension, but there are few
          In this study of 14 hypertensive men, there was a
          period. There was no weight change in that study, but two
          Between 1966 and 2001, there were 188 published
          There are no case control, cohort, or other studies that
          occurrences in the chlorthalidone arm. Although there was
          secondary outcome of total mortality, there were small
        of hypertension, several questions remain. There is still a
        
##### Example 2
            
            $ grep Glow -i government/*/*
            government/Media/GreensburgDailyNews.txt:Perhaps the most glowing comments on Bailey's philanthropy came
            
### grep -v

##### Example 1


            $ grep  the -v 911report/preface.txt
            
            PREFACE
                Democrats chosen by elected leaders from our nation's capital at a time of great
                avoid such tragedy again?
                27, 2002).
            Our mandate was sweeping. The law directed us to investigate "facts and circumstances
                to intelligence agencies, law enforcement agencies, diplomacy, immigration issues
                reviewed more than 2.5 million pages of documents and interviewed more than 1,200
                current and previous administrations who had responsibility for topics covered in
                our mandate. We have sought to be independent, impartial, thorough, and nonpartisan.
                public testimony from 160 witnesses.
                learned.
            We learned about an enemy who is sophisticated, patient, disciplined, and lethal. The
                political grievances, but its hostility toward us and our values is limitless. Its
                and equal rights for women. It makes no distinction between military and civilian
                targets. Collateral damage is not in its lexicon.
                and national security did not understand how grave this threat could be, and did not
                fault lines within our government-between foreign and domestic intelligence, and
                sharing information across a large and unwieldy government that had been built in a
                different era to confront different dangers.
                positive-an America that is safer, stronger, and wiser. That September day, we came
                accountability.
            As we complete our final report, we want to begin by thanking our fellow
                Commissioners, whose dedication to this task has been profound. We have reasoned
                built. They have given good advice, and faithfully carried out our guidance. They
                have searched records and produced a multitude of documents for us. We thank
                This final report is only a summary of what we have done, citing only a fraction of
                issues and organizations, we are conscious of our limits. We have not interviewed
                every knowledgeable person or found every relevant piece of paper. New information
                inevitably will come to light. We present this report as a foundation for a better
            We have listened to scores of overwhelming personal tragedies and astounding acts of
                preparing to respond if it becomes necessary. We emerge from this investigation with
                this process with strong opinions about what would work. All of us have had to
                citizens to study, reflect-and act.
            Thomas H. Kean, chair
            Lee H. Hamilton, vice chair


##### Example 2

        $ grep a -v biomed/1468-6708-3-1.txt
        
        Introduction
        elderly [ 9 ] .


        
          Study




          ] .
          (for persons who were never in excellent, very good, or
          report results using only the simpler definition.
          findings.







        Results
        likely.
        from 25 to 29.9. The second column, which shows results
        under 20.
        groups.
        YOL or YHL.


        Discussion



          YHL.





        Conclusion
        'overweight' by the NHLBI guidelines. This suggests using


        Competing interests


        CESD Center for Epidemiologic Studies Depression
        poor?


### grep -l

##### Example 1
        
        $ grep Cancer -l plos/*
        plos/journal.pbio.0020214.txt
        plos/journal.pbio.0020439.txt
        plos/pmed.0010028.txt
        plos/pmed.0010069.txt
        plos/pmed.0020017.txt
        plos/pmed.0020055.txt
        plos/pmed.0020073.txt
        plos/pmed.0020075.txt
        
##### Example 2

        $ grep Animals -l plos/*
        plos/journal.pbio.0020101.txt
        plos/journal.pbio.0020147.txt
        plos/journal.pbio.0020439.txt
        plos/pmed.0020045.txt
        plos/pmed.0020120.txt
        plos/pmed.0020249.txt

### grep -c

##### Example 1

        $ grep Taliban -c 911report/*
        911report/chapter-1.txt:0
        911report/chapter-10.txt:26
        911report/chapter-11.txt:5
        911report/chapter-12.txt:13
        911report/chapter-13.1.txt:0
        911report/chapter-13.2.txt:0
        911report/chapter-13.3.txt:32
        911report/chapter-13.4.txt:28
        911report/chapter-13.5.txt:6
        911report/chapter-2.txt:16
        911report/chapter-3.txt:66
        911report/chapter-5.txt:11
        911report/chapter-6.txt:66
        911report/chapter-7.txt:12
        911report/chapter-8.txt:0
        911report/chapter-9.txt:0
        911report/preface.txt:0
       
##### Example 2

        $ grep Weapons -c 911report/*
        911report/chapter-1.txt:0
        911report/chapter-10.txt:0
        911report/chapter-11.txt:2
        911report/chapter-12.txt:1
        911report/chapter-13.1.txt:0
        911report/chapter-13.2.txt:3
        911report/chapter-13.3.txt:3
        911report/chapter-13.4.txt:1
        911report/chapter-13.5.txt:1
        911report/chapter-2.txt:0
        911report/chapter-3.txt:0
        911report/chapter-5.txt:0
        911report/chapter-6.txt:0
        911report/chapter-7.txt:0
        911report/chapter-8.txt:0
        911report/chapter-9.txt:0
        911report/preface.txt:0

