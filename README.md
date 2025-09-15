# Experiment-10

### Name : SRIVATSAN G
### Reg no. : 212223230216

## Test plan document for library application
The Library Management System is an online application for assisting a librarian in managing a book library in a university. The system would provide basic set of features to add/update clients, add/update books, search for books, and manage check-in / checkout processes. Our test group tested the system based on the requirement specification. 

# INTRODUCTION
This test report is the result for testing in the LMS. It mainly focuses on two problems: what we will test and how we will test. 

## GUI test 
Pass criteria: librarians could use this GUI to interface with the backend library database without any difficulties 
Result: pass 

## Database test 

Pass criteria: 

Results of all basic and advanced operations are normal (refer to section 4) 
Result: pass

## Basic function test Add a student Pass criteria: 

Each customer/student should have following attributes: Student ID/SSN (unique), Name, Address and Phone number. 
Result: pass 

The retrieved customer information by viewing customer detail should contain the four attributes. 
Result: pass 

## Update/delete student Pass criteria: 

The record would be selected using the student ID 
Result: pass 

Updates can be made on full. Items only: Name, Address, Phone number 
Result: pass 

The record can be deleted if there are no books issued by user. 
Result: Partially pass.

When no books issued by user, he can be deleted. But when there are books Issued by this user, he was also deleted. It is wrong. The updated values would be reflected if the same customer's ID/SSN is called for. 
Result: pass 

If customer were deleted, it would not appear in further search queries. 
Result: pass 

## Add a book 
Pass criteria: 

Each book shall have following attributes: Call Number, ISBN, Title, Author name. 
Result: pass 

The retrieved book information should contain the four attributes. 
Result: pass 

## Update/delete book 
Pass criteria: 

The book item can be retrieved using the call number 
Result: did not pass. Cannot redrive using the call number 

The data items which can be updated are: ISBN, Title, Author name 
Result: pass 

The book can be deleted only if no user has issued it. 
Result: partially pass. 

When no user has issued it, pass. When there are user having issued it, did not pass The updated values would be reflected if the same call number is called for 
Result: pass 

If book were deleted, it would not appear in further search queries.
Result: pass 

## Search for Book
Pass criteria: 

The product shall let Librarian query books„ detail information by their ISBN number or Author or Title. 
Result: pass 

The search results would produce a list of books, which match the search parameters with following Details: Call number, ISBN number, Title, Author 
Result: pass 

The display would also provide the number of copies which is available for issue 
Result: pass 

The display shall provide a means to select one or more rows to a user-list 
Result: pass 

A detailed view of each book should provide information about check- in/check out status, with the borrower’s information. 
Result: pass 

The search display will be restricted to 20 results per page and there would be means to navigate from sets of search results. 
Result: pass 

The user can perform multiple searches before finally selecting a set of books for check in or checkout. These should be stored across searches. 
Result: pass 

A book may have more than one copy. But every copy with the same ISBN number should have same detail information. 
Result: pass 

The borrower’s list should agree with the data in student’s account 
Result: pass

## Check-in book 
Pass criteria: 

Librarians can check in a book using its call number 
Result: pass 

The check-in can be initiated from a previous search operation where user has selected a set of books. 
Result: pass 

The return date would automatically reflect the current system date. 
Result: did not pass. 

Any late fees would be computed as difference between due date and return date at rate of 10 cents a day. 
Result: did not pass 

A book, which has been checked in once, should not be checked in again 
Result: pass  

## Check-out book 
Pass criteria: 

Librarians can check out a book using its call number 
Result: pass 

The checkout can be initiated from a previous search operation where user has selected a set of books. 
Result: pass 

The student ID who is issuing the book would be entered 
Result: pass 

The issue date would automatically reflect the current system date. 
Result: did not pass 

The due date would automatically be stamped as 5 days from current date. 
Result: did not pass 

A book, which has been checked out once, should not be checked out again 
Result: pass 

A student who has books due should not be allowed to check out any books 
Result: did not pass 

The max. No of books that can be issued to a customer would be 10. The system should not allow checkout of books beyond this limit. 
Result: pass View book detail Pass criteria: 

This view would display details about a selected book from search operation 
Result: pass 

The details to be displayed are: Call number, IBN, Title, Author, Issue status (In library or checked out), If book is checked out it would display, User ID & Name, Checkout date, Due date 
Result: for checkout date and due date, did not pass 

Books checked in should not display user summary 
Result: pass 
 
Books checked out should display correct user details. 
Result: pass 

## View student detail Pass criteria: 
□ Librarians can select a user record for detailed view Result: pass 

□ The detail view should show: 
a. User name, ID, Address & Phone number Result: pass 
b. The books issued by user with issue date, due date, call number, title Result: did not pass 
c. Late fees & Fines summary and total Result: did not pass 

□ The display should match existing user profile Result: pass 

□ The books checked out should have their statuses marked Result: pass 

□ The book search query should show the user id correctly. Result: pass 
 
#### Network test 
Pass criteria: Results of operations (ping, ftp and ODBC connectivity check) are normal 

### Result
Thus, did not test this item, because no enough machines and no available environment. 

# Result
Thus, the Test cases for library application is implemented and output is verified successfully.
