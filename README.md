# jenkins_workshop
Given at GetTaxi, Feb 19 2015

Given at SeekingAlpha, March 16 2015

Given at at Perion, October 13th, 2015

material for jenkins workshop

requirements:
Linux/MacOS laptop with Java6 or higher installed.

Git installed

Github user

Good internet connection.

Agenda:
5 minute intro - what is Jenkins and what people use it for

55 minutes hands on work. (part 1)

15 minute break

45 minutes hands on work, (part 2+3)

## Lets Install Jenkins on your computer
Step 1: Download Jenkins: http://jenkins-ci.org/

Step 2: start jenkins: 
java -jar jenkins.war

# Part 1: Basics

## Excercise 1: Hello World
echo Hello world!

## Excercise 2: Periodic Build
say hello world every minute! (cron expression for this is "* * * * *")

## Excercise 3: Am I online ?
create a jenkins job that checks if you are online every minute, and then disconnect the wifi.
(command to ping 3 times is for example "ping -c 3 host")

## Excercise 4: Choice Parameters
Create a job that passes or fails based on a choice in build parameter.

## Excercise 5: Send an Email
create a jenkins job that sends an email to yourself.
How to enable local smtp on mac os: https://www.phase2technology.com/blog/how-to-enable-local-smtp-server-postfix-on-os-x-leopard/

## Excercise 6: Create a job that triggers another job
create a job called "knock knock", which calls a another job that says "who's there?"

## Excercise 7: behind the scenes
create a job that would take a long time to run, and look at the actual script running

## Excercise 8: build queue
create a job that would take a long time to run, run it several times, what happens ?

# Part 2: Plugins, best practices, slaves.

## Excercise 9: Naginator Plugin
create a job that fails permanently, and use the naginator plugin to have it try again in increasing variable time

## Excercise 10: Git Plugin
repo URL: 

https://github.com/gilzellner/jenkins_workshop.git

create a job that triggers a clone based on pushed items to this repo

# Part 3: Continuous Delivery Pipeline.

## Excercise 11: Continuous Delivery Pipeline
create a build, test, deploy pipeline based on jenkins jobs
