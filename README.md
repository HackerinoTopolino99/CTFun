# CTFun

## 1 Software requirement Specifications
### 1.1 Introduction
#### 1.1.1 Aim of the document
The main focus of this document is to describe the steps of the design of this system, named CTFun.
#### 1.1.2 Overview of the defined system
The system here described is an application that provides a training platform for players of Capture The Flag, with some features for competition, like a scoreboard accessible from all players that can encourage competitiveness between players.
#### 1.1.3 Hardware and Software requirements
The hardware requirements for this platform to work properly are an Internet connection and enough resources for manage multiple HTTP connections. Also will require a good amount of free disks for upload the challenges on the machine that will host this software. It is not required to use an external server for hosting a DBMS.
For software requirements it will be required to have a working JRE (21 at least) correctly installed on the host. For the DB, the application will initialize it with SQLite by default so it won't be necessary to install DBMS server.
#### 1.1.4 Related Systems, Pros and Cons
The other systems related to CTFun are:
- Google
- Facebook

Since this two system have the same function with CTFun, their pros and cons of this two will be described together. The pros are that a user (player or admin) won't have to create an account for login in the platform, so basically for him is just a password less to memorize. The cons are Google and Facebook are not trustworthy in matter of privacy and this will add more code to write for implement their API.
### 1.2 User Stories
* As a player, I want to read the description of a challenge, so i can search for external material to study on for solve the challenge
* As a player, I want to see a global scoreboard, so i can measure myself with other players on the platform
* As an admin, I want to be able to change the flag of a challenge
\end{itemize
### 1.3 Function Requirements
* The system shall provide a scoreboard accessible by all players
* The system shall provide a login for non registered players
* The system shall provide a description and a link for every attachment of the challenge when a player selects it
\end{itemize
### 1.4 Use Cases
#### 1.4.1 Overview Diagram
![Use Case Diagram](/diagrams/Use%20Case%20Diagram.jpg)
#### 1.4.2 Internal Steps
##### Name: Play CTF
1. The player selects a challenge.
2. The system shows a description of the challenge and a blank box for the flag.
3. The player submits the flag.
4. The system checks the correctness of the flag.
5. The system adds the points to player's score.
6. The system shows a link for the solution of the challenge's author.
7. The player clicks the link.
8. The system shows the official write up.
##### Extensions
- 1a. _The challenge is not available at the moment_: The system notifies the player and terminates the use case.
- 2a. _The challenge has one or more attacchemnts_: The system shows a link for download the attachments.
- 4a. _The flag is not correct_: The system notifies the player that the flag is not correct.
## 2. Storyboards
## 3. Design
### 3.1 Class Diagram
#### 3.1.1 VOPC
#### 3.1.2 Design-Level Diagram
### 3.2 Design Patterns
### 3.3 Activity Diagram
### 3.4 Sequence Diagram
### 3.5 State Diagram
## 4 Testing
## 5 Exceptions
## 6 Persistence
## 7 Sonar Cloud