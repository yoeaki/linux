# 1.linux的常用命令集合
## 1.目录的操作
### 1.1 change directory 
	1.Change directory command by cd
> + Enter designation directory：**cd fileName**  
> + Come back upper level directory：**cd ..**
> + Change directory by absolute：**cd /fileName**
> + Change upper level opration directory：**cd -**
### 1.2 directory(add,delete,update,select)
	1.make directory by mkdir
> + make dirctory: **mkdir fileName**  

	2.look over directory

> + look over directory：**ls**
> + look over detail info of directory: **ll**,eaquls **ls -l**

	3.find some directory by find
> + List current all directory and cdirectory: **find .**
> + List directory of absolute (/home or /home/demo) and start with .txt(ignore capitalization): **find /home/demo -iname \*.txt**
> + List current all directotry of .txt and .pdf: **find / -iname \*.txt -o -iname \*.pdf**

	3.move directory mv
> + Refactor directory Name : **mv oldName newName**
> + Move the directory to new place ： **mv fileName newPlace/null(newName)**

	4.copy directory cp
> + Copy directory to newPlace by recursive : **cp -r fileName newPalce**

	5.remove directory rm
> + Remove all directory/file/zip and so on.**rm -rf dirName**

### 1.3file (add,delete,update,select)
	1.create a file (touch)
> + create a file : **touch fileName**

	2.look over file content(cat/more/less/tail-10)
> + use comand of **cat** to look over the file info : **cat fileName**
> + use comand of **more** to look over the file info before 30% : **more 30% fileName**
> +  use comand of **less** to look over the file info which can use PgUp and PgDn to operate : **less fileName**
> + use comand of **tail-10** to look over the file info of top 10 line : **tail -10 fileName**

### 1.4 There are command of ping、fping、traceroute 
	ping : only can ping a host.
	fping : can ping host of specified range.
	traceroute : can show the host'route which next jump to end.  
<br>

	1.How to use **ping** and **ping'parameter**.
> + ping ip
> + -c  num    //ping a host on number
> + -w  time   //how much time to wait for a can't arrive host.
> + -i  time  //send a pakage to specified host of time interval

	2.fping ip
> + -a         //show some host of already passed
> + -A        //exeamle: fping -A www.baidu.com--->222.12.15.10
> + -c num   // ping numbers times every host when this host is alived.
> + -e      //Return the time required for ping of every host.
> + -f      //get the ip of file.
> + -i     //set TTL live.
> + -l     //loop to ping the host
> + -p    //set a time interval
> + -r num //if ping is failed,can ping num again.
> + -u   // show the host that failed to pass.

	3.traceroute 
> + -m num    //set the route jump number
> + -n        //show the ip of domain
> + -q num    //send num pakage to trace
> 
###1.5  instal  some application in different way
###1.5  instal  some application in different way
	1. yum 
>   + install -y pakageName  
>   

	2.wget  

 1. wget link
 2. tar zxvf fileName
 3. ./configure
 4. make
 5. make && make install

### 1.6 shell script
	command collection!
### 1.7 processes
+ ps -a(end all)、 -x(end to child)、  -e(all ps info)、  -f(complete info)
+ kill -9 pid
