# HTTP Server and Client using Linux TCP Sockets in C


This repository contains two programs: HTTP Server and Client, which are using HTTP 1.0 version to communicate with each other and also with the web.


## HTTP Client
- Takes server's IP and Port number, along with request type and file name as command-line  arguments.
> Usage: client **IP PORT GET/PUT filename**
> Example: ./a.out 127.0.0.1 8541 GET index.html

- Also supports sending GET and PUT request to general servers on the web
> Example: ./a.out www.google.co.in 80 GET /index.html
- Stores the retrived file as a local copy also.

## HTTP Server
- Takes Port number as command-line argument.
> Usage: server **PORT**
> Example: ./a.out 8541
- Handles both GET and PUT request.
- Stores the data sent after PUT request in the file specified in PUT request.
- Sends HTTP error codes if something goes wrong.

## About Project

This project is carried out as a part of Network Programming Lab Assignment at MNNIT Allahabad.
The description and requirements are mentioned in **question.pdf** file. updated readme
