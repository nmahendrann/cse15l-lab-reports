ssh nmahendran@ieng6.ucsd.edu

git clone [the ssh link]

cd into lab7

javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples

nano ListExamples.java

[fix the index1 into index 2]

control x, then enter to leave the nano

javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples

git add ListExamples.java

git commit -m “fixed”gr

git push
