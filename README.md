# Planche

![planche logo](http://www.makewebapp.net/planche-master/resources/images/logo.jpg)

Javascript MySQL GUI Client Tool

The Planche is MySQL GUI client tool. This tool has a flexible structure to use. Basically, the operation through the tunneling.
The current version is under development. So it may not work properly. The project has been developed, including the following JavaScript frameworks.

- [CodeMirror](http://codemirror.net/)
- [Sencha ExtJS 4.2](http://www.sencha.com/products/extjs/)

![Planche Preview](http://extjs.makewebapp.net/wp-content/uploads/2015/01/01.png)

## Demo

- [Planche Demo](http://www.makewebapp.net/planche-master)


## Required environment

1. Need php or nodejs environment for execute tunneling file.
2. Apache Web Server(optional) -> Tunneling file has its own web server.


## Current features

- Execute Query : like a desktop application
- Query Editor : like a desktop application
- Query Alignment : Yet it acts like a fool.
- Support delimiter
- Table schema view
- Auto query result paging(by limit)
- Create Procedure
- Create View
- Create Function
- Create Event
- Create Trigger
- Create, Alter, Drop Database
- Create, Alter, Drop, Truncate Table
- Query tokenize.
- Process Manager
- Scheme Edit Window
- Show Variables Window
- Show Status Window


## Install

1. Download planche-master.zip on your PC
2. Extract the zip file
3. Add host's information on the "resources/config/host.js" file

```javascript
Planche.config = {
    hosts : [
        {
            hostName    : 'My Host',
            tunnelingURL: 'http://localhost:8888',
            requestType : 'jsonp',
            host        : 'localhost',
            user        : 'user',
            pass        : 'password',
            charset     : 'utf8',
            port        : 3306,
            dbms        : 'mysql'
        }
    ]
}

```
4. Run the index.html file on your browser.
   (Yet recommend Chrome. I did not test other browsers. You can break your head.)

## Install - Run Tunneling

Run the "tunneling file" at CLI mode.
(Attention) When exposed tunneling uploaded files. Security issues may arise. I hope you remember this problem for the database server.

- PHP Environment
```
[user@localhost ~]$ php resources/tunneling/php/planche_tnl.php
```

- nodeJS Environment
```
[user@localhost ~]$ node resources/tunneling/nodejs/planche_tnl.js
```

## Watch the video

http://www.youtube.com/embed/WCnXJXDRlYs

## Official Website

http://plancheproject.github.io

## License

This content is released under the GPL v3