mkdir 

cd

git init
# Sets up the necessary Git files
# Initialized empty Git repository in /Users/Lokeshwaric/apple/.git/

touch README


git add README

git commit -m 'first commit'

git remote add origin https://github.com/Lokeshwaric/apple.git

git push origin master


to open a file frm directory

f=open("d:/python/note.txt","r")
str=f.read()
print(str)

print(f.name) 
print(f.mode)
print(f.closed)
f.read(10)
f.seek(5,0)-->change the initial position of file.
f.tell()-->it shows position.
f.readline()-->it reads a line frm file.

r+=read &write mode
append=it overlaps
write=at end it writes.


f=open("d:/python/note.txt","r")
f.read(10)   \\ reads the 10 letters frm file//
o/p-
'a=eval(inp'

to change file name
import os
os.rename("d:/python/note.txt",d:/python/nt.txt") 

to remove a file
import os
os.remove("d:/python/re.txt")
print(os.getcwd()) //it shows curnt folder//

to chang frm 1 folder to another fol
import os
os.chdir("d:/note.txt")-->change the crnt dir
os.rmdir("d:/note.txt")-->remove the fol





6/7/14,mon

try: zero division error,exceptions.
 c=2/0 :d="a"/0 
except(zerodivisionerror):,,,,except(Type
 print("divided by zero")
else:
 print("No Error")
finally:
 
print("Program executed")



types of error

ioerror
floaterror

d="a"/0   is a type error

to create a class

class student:
    name="loki"
    mark=100
    def display(self):
        print("student name is{0} \n student name is{1}".format(self.name,self.mark))
 s=student()
s.name="sam"
s.mark=100
s.display()



to declare obj in java
student obj=new student()

in python
obj=student()


over riding;
two class having the same function name to overwrirte a class.

class student:
    name="loki"
    mark=100
    def display(self):
        print("student name is {0} \n {0} mark is {1}".format(self.name,self.mark))
s=student()
#s.display()
s1=student()
#s1.display()
#s.name="sam"
#s.mark=100
class sports(student):
    game="cricket"
    rank=2
    def display(self):
        print("plays the game",self.game)
        print("Rank",self.rank)
s=sports()
s.display()
s.display

o/p--
plays the game cricket
Rank 2

class student:
    name="loki"
    mark=100
    def __init__(self,a,b):
      self.name=a
      self.mark=b
      print("constructor called")
    def display(self):
        print("student name is {0} \n {0} mark is {1}".format(self.name,self.mark))
s=student('raj',100)
s1=student('loki',90)
s2=student('jo',80)
#s.name="sam"
#s.mark=100
class sports(student):
    game="cricket"
    rank=2
    def  __init__(self,c,d):
     self.game=c
     self.rank=d
    def play(self):
        print(" plays the game",self.game)
        print("rank",self.rank)
sp=sports('cricket',2)
sp1=sports('badmitton',3)
sp2=sports('skipping',4)
s.display()
sp.play()
s1.display()
sp1.play()
s2.display()
sp2.play()

o/p--

constructor called
constructor called
constructor called
student name is raj 
 raj mark is 100
 plays the game cricket
rank 2
student name is loki 
 loki mark is 90
 plays the game badmitton
rank 3
student name is jo 
 jo mark is 80
 plays the game skipping
rank 4

plays the game cricket
Rank 2

installing mysql server

in cmd
type following

show databases;
create database stu;
show databases;
use stu;
create table mark(Reg_no int(5),name char(10),m1 int(5),m2 int(5));

mysql.connector
 
import mysql.connector
cn=mysql.connector connect(user='root',database='stu',password='root')
cn=cn.cursor()
cr.execute("select from mark")
for(r,n,m,rs) in cr:
print("{0<5}|{1:^20}|{2:<5}|{3:>10}}|
format{r,n,m,rs}
cr.close();
cn.close();

to print a star

for i in range(6):
 for j in range (6):
  print(" *")
print()

