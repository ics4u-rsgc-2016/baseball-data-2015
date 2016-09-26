# 2015 Major League Baseball Data

This repository exists to make distribution of data to my class more convenient.

Please visit the original source, [Sean Lahman's site](http://www.seanlahman.com/baseball-archive/statistics/) to obtain the data and further information.

# Installation

* Open your Cloud9 workspace.
* Open a Terminal prompt in Cloud 9.
* Run the following command:
```
    git clone https://github.com/rsgc-ics4u-2016/baseball-data-2015.git
```    
* Switch to the newly created directory:
```    
    cd baseball-data-2015/
```    
* Start MySQL:
```    
    mysql-ctl cli
```    
* Import the data:
```    
    source ~/workspace/baseball-data-2015/stats.sql
```    
* Show the list of databases:
```    
    show databases;
```    
* Use the **stats** database:
```    
    use stats;
```    
* See what tables you have to work with:
```    
    show tables;
```    
* Get more information about a table:
```    
    describe teams;
```    
* For example, get information about the local favourite:
```    
    SELECT yearID, teamID, name, W, L 
    FROM teams 
    WHERE teamID = 'TOR'; 
```    
