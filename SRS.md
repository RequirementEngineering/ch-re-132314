<h3 align='center'>
  Universidad Autónoma de Ciudad Juárez</br>
  División Multidisciplinaria de Ciudad Universitaria</br>
  Departamento de Ingeniería Electricidad y Computación</br>
</h3>
</br></br></br></br></br></br>
<p align='center'><img src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Escudo%20uacj%202015-color-sin%20fondo.png"  width="300" height="300" ></img></p>
</br></br></br></br></br></br>
<h3 align='right'>
Desarrollo de Requisitos de Software</br>
Library Services System</br>
Jonathan Arreola Peralta  132314</br>
</h3>



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
    - [Constraints](#Constraints)
    - [Assumptions and dependencies](#Assumptions-and-dependencies)
3. [Specific requirements](#Specific-requirements) 
    - [Functional requirements](#Functional-requirements)
    - [Non functional requirements](#Non-functional-requirements) 
4. [Appendixes](#Appendixes) 
   - [Elicitation process](#Elicitation-process)
   - [Bussiness Process Map](#Bussiness-Process-Map)

## Introduction
#### Purpose
The goal of this document is to present a description of the Library Services System. It will detail the purpose and the features of the system, its interfaces, what the system will do and the constraints under which it should operate. This document is intended for the stakeholders and the developers of the system.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Scope
The software system will be developed for the "Test Library". It is a web application that will allow the librarian in charge to manage the registration of new clients, registration of new books, borrowed books and the consultation of available books. This software will also serve as a tool for the clients of the library, allowing them to check through the collection of books available, request printing, pay fines. 

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Definitions, acronyms, and abbreviations
Term | Definition
-----|-----------
Software | Set of instructions, data or programs used to operate computers and execute specific tasks.
Hardware | Physical parts of a computer and related devices.
Application | Program, or group of programs, that is designed for the end user.
Database | Collection of informations organized in such way that a computer program can quicly select desired pieces of data.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### References
* SISTEMA INFORMATICO PARA LA BIBLIOTECA DE LA INSTITUCIÓN EDUCATIVA DEPARTAMENTAL ANTONIO NARIÑO: https://repository.uniminuto.edu/bitstream/handle/10656/4771/T.TI%20PENAGOS%20JIMENEZ%20GINA%20TATIANA%202014.pdf?sequence=1&isAllowed=y
* SISTEMA INFORMÁTICO PARA LA GESTIÓN DE LA INFORMACIÓN EN LAS BIBLIOTECAS: http://www.eumed.net/cursecon/ecolat/cu/2012/opah.html

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Overview
The next chapter, Overall description, will give an overview of the functionality of the system.
The third chapter, Specific requirements, will describe the details of the funcionality of the product. This chapter uses technical terms, so its mainly aimed for the use of developers.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

## Overall description
#### Product perspective
This web application will serve as a tool for both, the librarian and the clients. The librarian will be able to register new clients, new books, check for borrowed books and search in the book database. The client will be able to search books, borrow books pay their fines if the went over the time they had to return borrowed books and request the library to print their documents.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Product functions
Librarian Functions:
* Register a new employee.
* Register a new customer.
* Register, update or delete the information of a book.
* Register the date and time of a borrowed book, its information and which customer got it.
* Consult what books are available in the library.
* Order new books.

Customer Functions:
* Consult what books are available in the library.
* Consult the information of an specific book.
* Borrow book.
* Request printing.
* Pay fine.
* Buy books.

Accountant Functions:
* Review library invoices.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### User characteristics
User | Description
----|-----------
Librarian | Person in charge of the library. They help people find information and conduct research for personal and professional use. Their duties may change based on the type of library they work in.
Accountant | Person in charge of registering the earnings of the library.
Customer | Person who its looking for a book from the library. They may want to borrow a book for a certain amount of time.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Constraints
* An access to internet is required to use the web application.
#### Assumptions and dependencies
* The librarian is accustomed to using a similar web application.
* The client must be registered in the system before borrowing a book.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

## Specific requirements
This section will provide a description of the specific actions the system will do.
#### Functional requirements
##### General Use Case
![](images/General%20Use%20Case.png)

Name | Library Services System
---|---
Author | Jonathan Arreola Peralta
Brief Description | The application will allow the client to search for a book, borrow a book, pay a library fine and request printing. The librarian will be able to search for a book, register new clients and new books, check what books have they lent and order new books from the publishers. The accountant must have access to the earnings of the library to register them.
Actors | Librarian, accountant and client.
Preconditions | All the actors must be registered on the system.
Normal Flow | Librarian: Register client, register book search book. Client: Search book, borrow book, pay fine, request printing. Accountant: Register purchases/earnings.
Postconditions | Any information gathered must be saved.

##### Client registration Use Case
![](images/Use%20Case%20Diagram1%20-%20Register%20client.jpg)

Name | Client registration
---|---
Author | Jonathan Arreola Peralta
Brief Description | The librarian must register each new client in order for them to gain access to the web application.
Actors | Librarian.
Preconditions | The client must provide the librarian their information.
Normal Flow | Librarian: Collect client info, save client info, provide client with username and password, give client a library ID.
Postconditions | The client must confirm the information on their new library ID is correct.

* The system should allow the users to login via a screen asking them for their username and password.
* The librarian must be able to register the information of a new client.
* The librarian must be able to register the information of a new book.
* The system must allow the update or deletion of book's information.
* The librarian must be able to register the information of a borrowed book, as well as what client has it.
* The system will send a message to a client when they are about to pass the date when they should return any borrowed book.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

#### Non-functional requirements
* The system must be able to operate properly with up to 200 users at a time.
* Only the librarian will be able to update or delete any information about a client or a book.
* Any external communication between the client and the system must be encrypted.
* The system must have clear and user friendly interfaces.

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)

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

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)
#### Bussiness Process Map

###### Main diagram

<p align='center'><img src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Library%20BPM.jpg"></img></p>

##### Sub processes
###### Client registration
<p align='center'><img src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Client%20registration.jpg"></img></p>

###### Book registration
<p align='center'><img src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Register%20new%20book.jpg"></img></p>

###### Printing
<p align='center'><img src="https://github.com/RequirementEngineering/ch-re-132314/blob/master/images/Request%20printing.jpg"></img></p>

_Return to Table of Contents:_ [Table of Contents](#Table-of-Contents)
