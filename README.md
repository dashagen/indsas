# A Perl script to indent a SAS code

## Example: 
```bash
% indsas xxx.sas
```

## NOTE: 
1) **indsas** assumes the following SAS scripting(indenting) styles for input and merge statements: 

    ```sas
    /* INPUT */ 
    data a1; 
        infile 'xxxx.txt'; 
        input 
             var1 $ 
             var2 $ 
             ....... 
        ; 
    run; 

    /* MERGE */
    data new; 
           merge 
                dat1(in=a) 
                dat2(in=b) 
           ; 
    run; 
    ```
    
2) **indsas** also assumes the following scripting style: 
    - PROC and DATA statements always end with RUN;
    - DO,IF xxx THEN DO and ELSE DO should be closed by END;
    - PROC SQL should be closed by QUIT; 

3) This script takes on a simplistic approach and does not account for all other non standard scripting styles. 

