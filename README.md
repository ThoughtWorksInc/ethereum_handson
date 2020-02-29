# Setup

docker-compose up -d

Setup has major three services:
1. Quorum - Three instances of quorums are running, more details are given below
2. Spring boot REST API - REST API to talk to Quorum nodes.
3. Web - Simple HTML/JS based web app to talk to rest API

# About Application
This is a sample Voting Application, this app takes care for casting the vote from the desired pod and Election commision will take care of counting these votes.

We have 2 Booths which will cast the votes and 1 Election commision which will count the votes.

## POD TYPES ##

The application has three pods, these pods are of two types:
1. <b>Election Comission</b>: Election commision knows everything about votes, all the participants and all the Booths will involve Election Commision in every transaction. Because EC knows everything about the votes, so it is EC's responsibility for getting the result for election.
2. <b>Booth</b>: Booth pods are responsible for casting the votes. Just for the sake of usage every booth has 2 hard coded users in it.

## USERS ##

Although there is no authentication for the application, there are 5 main users of the application. Two users belong to Booth1 (), two users belong to Booth2 (), and the final election commision user which will count the votes.


Feedback Link :https://forms.gle/uXBtCg2tK4EzckARA
