# Weather-Observation-Station-7

Problem

Query the list of CITY names ending with vowels (a, e, i, o, u) from STATION. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

            STATION

        Field	     Type
        ID                   NUMBER
        CITY                 VARCHAR2(21)
        STATE                VARCHAR2(2)
        LAT_N                NUMBER
        LONG_W	     NUMBER
                    
where LAT_N is the northern latitude and LONG_W is the western longitude.

SOLUTION IN MYSQL

    select distinct city from station where city like '%a' or city like '%e' or city like '%i' or city like '%o' or city like '%u';
