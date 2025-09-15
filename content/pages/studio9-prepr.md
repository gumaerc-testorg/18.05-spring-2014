---
content_type: page
description: Extra files used for preparation or analysis.
draft: false
title: studio9-prep.r
uid: b87b80ff-dc93-45a7-90e4-622d903aa82e
---
\# --------------------- #  
#Data for hiring level  
set.seed(77)  
group1 = rmultinom(1, 60, c(25,30,30,15))  
group2 = rmultinom(1, 60, c(12,34,34,20))  
economy = c(24,31,31,14)/100

\# Write data to file  
col.names = c("group1", "group2","economyProportions")  
row.names = c("Level1", "Level2", "Level3", "Level4")

hiringdata = cbind(group1,group2,economy)   
rownames(hiringdata) = row.names  
colnames(hiringdata) = col.names  
hiringdata

\# Comment out because only need to write once.  
#write.table(hiringdata,'studio9Data.tbl', row.names=T, col.names=T)  
y = read.table('studio9Data.tbl')  
print(y)