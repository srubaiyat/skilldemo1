# skill demo 1 notes

ssh __account-name__@ieng6.ucsd.com

git clone https://github.com/ucsd-cse15l-w23/skill-demo1-server

*Mac*

javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java

java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore  __Tests__

*Windows*

javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java

java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore __Tests__

git clone https://github.com/ucsd-cse15l-w23/skill-demo1-data

cd skill-demo1-data

find written_2 > find-results.txt
grep ".txt" find-results.txt > grep-results.txt
wc grep-results.txt

xargs grep "Lucayans" < grep-results.txt

cd ../skill-demo1-server

java FileServer __port__ ../skill-demo1-data/

ieng6-202@ucsd.edu:__port__/search?q=Bahamas-History.txt

ieng6-202@ucsd.edu:__port__/search?q=ch1.txt

