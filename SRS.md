# Title
## Introduction
#### Purpose
The goal of this document is to present a description of the Library Services System. It will detail the purpose and the features of the system, its interfaces, what the system will do and the constraints under which it should operate. This document is intended for the stakeholders and the developers of the system.
#### Scope
The software system will be developed for the "Test Library". It is a web application that will allow the librarian in charge to manage the registration of new clients, registration of new books, borrowed books and the consultation of available books. This software will also serve as a tool for the clients of the library, allowing them to check through the collection of books available. Libra
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

##### Librarian Application
Section | Description
---------|-----------
Login | This is the first window that will pop up once the application is running. The employee must input their username and password to gain access to the system.
Main menu | This window will pop up once the librarian got access. They will have an array of options to choose from: Register Employee, Register Customer, Register/Delete Book, Consult Book, Lend Book and Borrowed Books.
Register/Delete Employee | The librarian will be able to register a new employee. The information requested will be: Name, Telephone number, Email, Username and Password. Also, only the librarian will be able to delete the information of an ex-employee.
Register Customer | In this window the librarian will be able to register the information of a new customer, with the goal of giving them a membership, so they are allow to borrow any books. The information needed is: Name, Telephone Number and Email.
Register/Delete Book | Here, the librarian can register the information of a new book in stock. Also, they will be able to delete the information of a book that is no longer available. To register a book, the librarian should input the next information: Name of the book, Author, Publisher, Year of publication, Pages and a Short review of the book.
Lend Book | Once the customer has the book the want to borrow, in this window the librarian will register the name of the book, the date and the information of the customer.
Search Book | In this window, the librarian will be able to help the customer to find a book. There will be a search bar that will allow to find a book by: Name, Author, Publisher, Year of publication and Pages.
Borrowed Books | This window will show the librarian what books were borrowed, which customer has it and the date it was borrowed.

##### Customer Application
Section | Description
---------|-----------
Main menu (Search Book) | This is the only screen of the customer software application. Here, customer will be able to look through in the database of the library, to search for a determined book. They can search a book by: Name, Author, Publisher, Year of publication and Pages. Once the query is done, the information of the book or any book related will be printed on the screen for the customer. The data printed will be: Name, Author, Publisher, Year of publication Pages, Short Review of the Book and the section of the library where they can find the book.
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
What are the processes of this library? | There are several processes that occur daily here on the library. To begin with, we check what books are available to the clients. We also check what are the books we have lent, who was the client that has it, and what is the date on which they must return it. If the date has passed, the client has to pay a fine. As a librarian, I also have to register any new books we get. We also have to register our new clients in order for them to be able to borrow books. Sometimes, there are clients that need to print their documents...

