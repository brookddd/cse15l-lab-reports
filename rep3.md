# `find` Command Examples

1) `find -size` finds files matching the size
> To find the files and directories __less__ than 1 Kilobyte I used:\
input:\
`find . -size -1k`\
output:\
`.`\
`./government`\
`./government/About_LSC`\
`./government/Env_Prot_Agen`\
`./government/Alcohol_Problems`\
`./government/Post_Rate_Comm`\
`./plos/pmed.0020191.txt`\
`./plos/pmed.0020226.txt`\
`./911report`

> To find the files and directories __more__ than 200 Kilobytes I used:\
input:\
`$ find . -size +200k`\
output:\
`./government/About_LSC/commission_report.txt`\
`./government/Env_Prot_Agen/bill.txt`\
`./government/Gen_Account_Office/GovernmentAuditingStandards_yb2002ed.txt`\
`./government/Gen_Account_Office/Statements_Feb28-1997_volume.txt`\
`./government/Gen_Account_Office/d01591sp.txt`\
`./911report/chapter-13.4.txt`\
`./911report/chapter-13.5.txt`\
`./911report/chapter-3.txt`\

2)  `find -type` finds directories or files based on syntax:
> In order to get all directories in `technical`:\
input:\
`$ find . -type d`\
output:\
`.`\
`./government`\
`./government/About_LSC`\
`./government/Env_Prot_Agen`\
`./government/Alcohol_Problems`\
`./government/Gen_Account_Office`\
`./government/Post_Rate_Comm`\
`./government/Media`\
`./plos`\
`./biomed`\
`./911report`

> To get all the files in `government/Alcohol_Problems`:\
input:\
`$ find . -type f`\
output: \
`./Session2-PDF.txt`\
`./Session3-PDF.txt`\
`./DraftRecom-PDF.txt`\
`./Session4-PDF.txt`

3)  `find -name` finds files matching the name:
> Let's say I don't know where in the `technical` file diversity_priorities is. Then I can input:\
`find . -name diversity_priorities.txt`\
and the output will be:\
`./government/About_LSC/diversity_priorities.txt`\

> Combining this with my knowledge of searching by type, I can find the location of the Media folder:\
input:\
`find . -type d -name Media`\
output:\
`./government/Media`\

4)  `find -empty` finds empty directories in the directory:\
> In the directory `technical`, there are no empty ones. Therefore when I input:\
`find . -empty`\
The output was empty.
> 
