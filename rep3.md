* `find` Command Examples



1) `find -size` finds files matching the size
  a)
  b)
2) `find -name` finds files matching the name
3) `find -type` finds directories or files based on syntax:

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

> To get all the files in `government/Alcohol_Problems` I typed:
input: `$ find . -type f`
output: 
`./Session2-PDF.txt
./Session3-PDF.txt
./DraftRecom-PDF.txt
./Session4-PDF.txt`

5) `find -empty` find empty files or directories in the directory
