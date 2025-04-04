## Library Management System - Database Schema

# Overview

This project contains a relational database schema for managing a library system. It is designed to handle information about books, authors, members, and borrowing transactions.

# Features

* Tracks books and their availability.

* Stores author details.

* Manages library members and their borrowing history.

* Implements relationships using primary and foreign keys.

## Database Schema

The database consists of four main tables:

## Authors Table

Stores author information.

* author_id (Primary Key)

* first_name

* last_name

* nationality

* birth_date

# Books Table

Stores book details.

* book_id (Primary Key)

* title

* author_id (Foreign Key referencing Authors)

* genre

* publication_year

* available_copies

## Members Table

Stores library members' details.

* member_id (Primary Key)

* first_name

* last_name

* email

* phone_number

* join_date

## Borrowings Table

Tracks borrowing transactions.

* borrowing_id (Primary Key)

* member_id (Foreign Key referencing Members)

* book_id (Foreign Key referencing Books)

* borrow_date

* return_date


