A Perl script to indent a lousily indented or indentless SAS script.

Example: 
indsas xxx.sas 
or 
indsas xxx.sas > new_xxx.sas 


NOTE: 
1) indsas assumes the following SAS scripting(indenting) styles for input and merge statements: 

==INPUT=== 
data a1; 
    infile 'xxxx.txt'; 
    input 
         var1 $ 
         var2 $ 
         ....... 
    ; 
run; 

==MERGE=== 
data new; 
       merge 
            dat1(in=a) 
            dat2(in=b) 
       ; 
run; 

2) indsas also assumes the following scripting style: 
   *PROC and DATA statements are always accompanied with RUN; 
   *DO,IF xxx THEN DO and ELSE DO should be closed by END; 
   *PROC SQL should be closed by QUIT; 

3) This script is still very primitive and does not account for all other eccentric scripting styles. 

4) indsas does not handle "cards" or "datalines" correctly. Please manually adjust those lines. 

5) indsas was only tested in the unix/linux environment. 




 
install details
download and move indsas to whatever folder you like. Add that folder to your $PATH variable if you haven't done that yet.
 

