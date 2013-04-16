PHP MySQL Session Handler
========================

About
----------------------------

PHP sessions are awful, slow and don't scale; they also lock-up making page requests rediculously slow. That's why I use
MYSQL sessions. It's pretty transparent to install them using this nice plugin. When I found this plugin it was not
functional due to being based on an older version of PHP and a bit of careless programming; but now it works again! 


Installation
----------------------------

1. First you need to create a table in your database (you may want to make a new database).
- You can do this by pasting the following code into PHPMyAdmin or your MYSQL console. 

```
    CREATE TABLE `session_handler_table` (
    `id` varchar(255) NOT NULL,
    `data` mediumtext NOT NULL,
    `timestamp` int(255) NOT NULL,
    PRIMARY KEY (`id`)
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

Then have a look at example.php
Easy!
