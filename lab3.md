# CSE 15L Lab Report 3

The command I am choosing is grep. 

The first command is grep -R: 
``` 
aj@Akhils-MacBook-Pro 911report % grep -R "Sally"        
./chapter-7.txt:                to "Sally"-a coded instruction to Binalshibh to send funds to Zacarias Moussaoui.
```
```
aj@Akhils-MacBook-Pro 911report % grep -R "views" preface.txt
preface.txt:                considered the views of others. We hope our report will encourage our fellow
```
The command grep -R recursively searches for text in all files in a directory and its subdirectories. 

The second command is grep -E:
```
aj@Akhils-MacBook-Pro 911report % grep -E "views|Sally" chapter-7.txt
                sympathetic to those extremist views. During a post-9/11 search of his possessions,
                to "Sally"-a coded instruction to Binalshibh to send funds to Zacarias Moussaoui.
```
```
aj@Akhils-MacBook-Pro 911report % grep -E "views|report" preface.txt
            We present the narrative of this report and the recommendations that flow from it to
                partisan division-have come together to present this report without dissent.
                We hope that the terrible losses chronicled in this report can create something
            As we complete our final report, we want to begin by thanking our fellow
                together over every page, and the report has benefited from this remarkable
                Philip Zelikow, has contributed innumerable hours to the completion of this report,
                & Company for helping to get this report to the broad public.
                This final report is only a summary of what we have done, citing only a fraction of
                inevitably will come to light. We present this report as a foundation for a better
                considered the views of others. We hope our report will encourage our fellow
```
The command grep -E is like the normal function but it allows you to look up two words and not only one. 

The third command is grep -c: 
```
aj@Akhils-MacBook-Pro 911report % grep -c "views" preface.txt
1
```
```
aj@Akhils-MacBook-Pro biomed % grep -c "of" 1471-2091-3-23.txt
117
```
The command grep -c displays only the count of matching lines and not the actual lines themselves. 

The fourth command is grep -B and grep -A: 
```
aj@Akhils-MacBook-Pro biomed % grep -B 3 -A 3 "Polymerase" 1471-2091-3-23.txt
        Proteins recognizing specific DNA sequences play an
        important role in the regulation of gene expression and in
        DNA replication. Nearly all eukaryotic genes transcribed by
        RNA Polymerase II for instance, contain the conserved TATA
        box which is present upstream of the transcription start
        site. The TATA-box binding protein, a ~30 kDa component of
        the TFIID complex binds specifically to the heptanucleotide
```
```
aj@Akhils-MacBook-Pro 911report % grep -B 2 -A 2 "agencies" preface.txt      
            Our mandate was sweeping. The law directed us to investigate "facts and circumstances
                relating to the terrorist attacks of September 11, 2001," including those relating
                to intelligence agencies, law enforcement agencies, diplomacy, immigration issues
                and border control, the flow of assets to terrorist organizations, commercial
                aviation, the role of congressional oversight and resource allocation, and other
--
                adjust their policies, plans, and practices to deter or defeat it. We learned of
                fault lines within our government-between foreign and domestic intelligence, and
                between and within agencies. We learned of the pervasive problems of managing and
                sharing information across a large and unwieldy government that had been built in a
                different era to confront different dangers.
--
                the same time protecting our country against future attacks. We have been forced to
                think about the way our government is organized. The massive departments and
                agencies that prevailed in the great struggles of the twentieth century must work
                together in new ways, so that all the instruments of national power can be combined.
                Congress needs dramatic change as well to strengthen oversight and focus
--
                They have conducted the exacting investigative work upon which the Commission has
                built. They have given good advice, and faithfully carried out our guidance. They
                have been superb. We thank the Congress and the President. Executive branch agencies
                have searched records and produced a multitude of documents for us. We thank
                officials, past and present, who were generous with their time and provided us with
```
The command grep -B and grep -A display lines before and after the matching lines. The number I chose are the lines it shows before and after.
So for the first example it was three and the second examples it was two. 


To find these commands I used chatGPT. 
