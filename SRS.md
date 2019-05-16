<p align='center'>
Universidad Autónoma de Ciudad Juárez</br>
División Multidisciplinaria de Ciudad Universitaria</br>
Departamento de Ingeniería Electricidad y Computación</br>
</p>
</br></br></br>
<p align="center">
<img width="300" height="300" 
  src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Escudo%20uacj%202015-color-sin%20fondo.png">
</p>
</br></br></br></br></br></br>
<p align='right'>
Desarrollo de Requisitos de Software</br>
Library Services System</br>
Jonathan Arreola Peralta</br>
</p>

## Table of Contents
1. [Introduction](#Introduction)
    - [Purpose](#Purpose)
    - [Scope](#Scope)
    - [Definitions, acronyms, and abbreviations](#Definitions-acronyms-and-abbreviations)
    - [References](#References)
    - [Overview](#Overview)

2. [Overrall description](#Overall-description)
    - [Product perspective](#Product-perspective)
    - [Product Functions](#Product-functions) 
    - [User characteristics](#User-characteristics)
    - [Constrains](#Constrains)
    - [Assumptions and dependencies](#Assumptions-and-depedencies)
3. [Specific requirements](#Specific-requirements) 
    - [External interfaces](#External-Interface)
    - [Requirements](#requirements)
       - [Functional requirements](#Functional-requirements)
       - [Non functional requirements](#Non-functional-requirements) 
4. [Appendixes](#Appendixes) 
   - [Elicitation process](#Elicitation-process)
   - [Bussiness Process Management](#Bussiness-Process-Management)

## Introduction
#### Purpose
The goal of this document is to present a description of the Library Services System. It will detail the purpose and the features of the system, its interfaces, what the system will do and the constraints under which it should operate. This document is intended for the stakeholders and the developers of the system.
#### Scope
The software system will be developed for the "Test Library". It is a web application that will allow the librarian in charge to manage the registration of new clients, registration of new books, borrowed books and the consultation of available books. This software will also serve as a tool for the clients of the library, allowing them to check through the collection of books available. 
#### Definitions, acronyms, and abbreviations
Term | Definition
-----|-----------
Software | Set of instructions, data or programs used to operate computers and execute specific tasks.
Hardware | Physical parts of a computer and related devices.
Application | Program, or group of programs, that is designed for the end user.
Database | Collection of informations organized in such way that a computer program can quicly select desired pieces of data.
#### References
#### Overview
The next chapter, Overall description, will give an overview of the functionality of the system.
The third chapter, Specific requirements, will describe the details of the funcionality of the product. This chapter uses technical terms, so its mainly aimed for the use of developers.
## Overall description
#### Product perspective
This software system is a new product that will be implemented in the Test Library. It will be divided in two main parts, the software application for the librarian and the application for the customer. Both of this applications will be connected to a database designed for the purpose of this system.
#### Product functions
Librarian Desktop Application:
* Register a new employee.
* Register a new customer.
* Register, update or delete the information of a book.
* Register the date and time of a borrowed book, its information and which customer got it.
* Consult what books are available in the library.

Customer Desktop Application:
* Consult what books are available in the library.
* Consult the information of an specific book.

#### User characteristics
User | Description
----|-----------
Librarian | Person in charge of the library. They help people find information and conduct research for personal and professional use. Their duties may change based on the type of library they work in.
Customer | Person who its looking for a book from the library. They may want to borrow a book for a certain amount of time.

#### Constraints
* The computers that will run the librarian and customer application should have Windows 7 up to Windows 10 as Operating System.
#### Assumptions and dependencies
* The librarian is accustomed to using a similar computer application.
* The customer should be registered in the system before borrowing a book.
## Specific requirements
This section will provide a description of the specific actions the system will do.
#### External interfaces
The both applications have visual elements that will be described in this section.

#### Functional requirements
#### General Use Case
![](images/General%20Use%20Case.png)
##### Librarian Application
* Login screen (Username and Password)
* Register/Delete employee info.
* Register Customer info.
* Register/Delete book info.
* Search Book.
* Register borrowed book information.
### Appendixes
#### Elicitation Process
The elicitation process was carried out by interviewing the librarian in charge. They explained that there were several processes that were vital in order for the library to function correctly. The next section shows how the interview went.

Question | Answer 
---------|---------
What are the processes of this library? | There are several processes that occur daily here on the library. To begin with, we check what books are available to the clients. We also check what are the books we have lent, who was the client that has it, and what is the date on which they must return them. If the date has passed, the client has to pay a fine. As a librarian, I also have to register any new books we get. We also have to register our new clients in order for them to be able to borrow books. Sometimes, there are clients that need to print their documents, so in order to make the process faster, maybe they could send their documents to us via this application and we could print it and have it ready for them when they arrive. We also sell a variety of books to our customers, so we check what books we have in stock and what books we need to buy directly from the publishing house.
What information do you register about your clients? | The usual. We begin with their first and last name, their telephone number and email. After we register them, we give the client a library ID.
What's the information you register about the books? | We register the book's name, autors' names, publishing house, year of publication, the general subject of the book, key words.
How do you keep track about what books have you lent? | Before they borrow the book, the client has to be registered in our library. We check their library ID to get their information faster. We keep track of whatever books they took, the date and for how long are they going to borrow the books. There are predefined times for how long they can keep the books: 3 days, 7 days or 14 days. They have to come and register the books they borrowed again after their time is over. If they are about to go over the time they can have the books, we'll send them and email to remind them they have to, either return the book or renew their time. Once they go over the established time, they'll have to pay a fine.
What do you think the web application should have for it to be the most useful for the library and its customers? | Well, having a way to search what books are available would be helpful for both the clients and us as librarians. The clients would be able to know what books without having to come here personally. And it would be helpful for us to keep track of the books we have. There should be a section for the client to know what books they have and when should they return them to avoid fines, and there should be a way for us to keep track of the books we've lent and all that information we talked about before. I guess we would have to need a login system, so each client will be able to access to their information. Because we also sell books, there should be a way to contact the publishing houses that grant us the books. When a certain book is about to run out of stock, we call the respective publishing house and they send to us more books. They take about a week to arrive, so we need to ask for them in advance. We have an accountant that keeps track of our purchases and earning. They will need a way to access the information of the books we've sold, the fines our clients have paid and the earnings we get for printing our clients' documents.

#### Bussiness Process Management



