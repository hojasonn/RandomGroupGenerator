# RandomGroupGenerator

I developed this in Mathematica because I wanted a transparent way to form random groups in a classroom setting; this way, students can be sure that groups are completely (pseudo)random. Mathematica is an easy choice because I know the students have previous experience using the program, and it allows visualization of the random groups for quickly facilitating collaborative work.
The few variables that need to be changed for any specific scenario are at the top of RandomGroupGenerator.nb:
```
students = Get[ToString[NotebookDirectory[]] <> "studentList.m"];
groupSize = 6;
className = "PHYS371";
```
  - Change "studentList.m" to whatever file contains a classlist of names. A sample file is provided.
  - **groupSize** will change depending on how big you want your groups.
  - **className** is a string that describes the context of the groups you're forming.
  
  That's it. The output should be a TreePlot diagram, like this:
  ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")
