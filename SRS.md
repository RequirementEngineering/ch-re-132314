# Title
## Introduction
#### Purpose
The goal of this document is to present a description of the (system). It will detail the purpose and the features of the system, its interfaces, what the system will do and the constraints under which it should operate. This document is intended for the stakeholders and the developers of the system.
#### Scope
The software system will be developed for the Test Library. It is a desktop application that will allow the librarian in charge to manage the registration of new clients, registration of new books, borrowed books and the consultation of available books. This software will also serve as a tool for the clients of the library, allowing them to check through the collection of books available.
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
This software system is a new product that will be implemented in the Test Library of certain town. It will be divided in two main parts, the software application for the librarian and the application for the customer. Both of this applications will be connected to a database designed for the purpose of this system.
#### Product functions
Librarian Desktop Application:
* Register a new customer.
* Register, update or delete the information of a book.
* Register the date and time of a borrowed book, its information and which customer got it.
* Consult what books are available in the library.

Customer Desktop Application:
* Consult what books are available in the library.
* Consult the information of an specific book.

#### User characteristics
User|Description
----|-----------
Librarian | Person in charge of the library. They help people find information and conduct research for personal and professional use. Their duties may change based on the type of library they work in.
Customer | Person who its looking for a book from the library. They may want to borrow a book for a certain amount of time.

#### Constraints
* The computers that will run the librarian and customer application should have Windows 7 up to Windows 10 as Operating System.
#### Assumptions and dependencies
* The librarian is accustomed to using a similar computer application.
* The customer should be registered in the system before borrowing a book.
## Specific requirements
