# `find` Command Examples

1) `find -size` finds files matching the size\
> To get an understanding of how big the files are I used:\
input: `find . -size -1k`\
output:\
`.
./government
./government/About_LSC
./government/Env_Prot_Agen
./government/Alcohol_Problems
./government/Post_Rate_Comm
./plos/pmed.0020191.txt
./plos/pmed.0020226.txt
./911report`

  
2)  `find -name` finds files matching the name
3)  `find -type` finds directories or files based on syntax:

> In order to get all directories in `technical`:
input: `$ find . -type d`
output:
`.
./government
./government/About_LSC
./government/Env_Prot_Agen
./government/Alcohol_Problems
./government/Gen_Account_Office
./government/Post_Rate_Comm
./government/Media
./plos
./biomed
./911report`

> To get all the files in `government/Alcohol_Problems`:
input: `$ find . -type f`
output: 
`./Session2-PDF.txt
./Session3-PDF.txt
./DraftRecom-PDF.txt
./Session4-PDF.txt`

4)  `find -empty` find empty files or directories in the directory
