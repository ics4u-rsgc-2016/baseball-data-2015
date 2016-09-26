# 2015 Major League Baseball Data

This repository exists to make distribution of data to my class more convenient.

Please visit the original source, [Sean Lahman's site](http://www.seanlahman.com/baseball-archive/statistics/) to obtain the data and further information.

# Installation

1. Open your Cloud9 workspace.
2. Open a Terminal prompt in Cloud 9.
3. Run the following command:
    git clone https://github.com/ics4u-rsgc-2016/baseball-data-2015.git
4. Switch to the newly created directory:
    cd baseball-data-2015/
5. Start MySQL:
    mysql-ctl cli
6. Import the data:
    source ~/workspace/baseball-data-2015/stats.sql
7. Show the list of databases:
    show databases;
8. Use the **stats** database:
    use stats;
9. See what tables you have to work with:
    show tables;
10. Get more information about a table:
    describe teams;
11. For example, get information about the local favourite:
    SELECT yearID, teamID, name, W, L 
    FROM teams 
    WHERE teamID = 'TOR'; 
