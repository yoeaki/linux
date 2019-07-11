# linux的常用命令集合
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
