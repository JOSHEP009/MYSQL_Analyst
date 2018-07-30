# MYSQL_Analyst

Prueba Técnica - Bquate
CHALLENGE 1
Recommendations:
1. Consistency and cohesion of the code
2. Following of available best practices for the language being used
3. Understanding of object oriented programming principles
4. Assets and UI/UX are implemented based on requirements
Write a program that prints all the numbers from 1 to 100. However, for multiples of 3, instead of the number, print "Multi". For multiples of 5 print "IT". For numbers which are multiples of both 3 and 5, print "Multipli".
But here's the catch: you can use only one `if`. No multiple branches, ternary operators or `else`.
Requirements
● 1 if
● You can't use `else`, `else if` or ternary
● Unit tests
● We are big fans of JS and Node.JS. Submission
You can create a public repository on your GitHub account and send the link to us, or just send us a zip file.
CHALLENGE 2
We have the following tables:
CITY COUNTRY CUSTOMER INVOICE
ID NUMBER ID NUMBER ID NUMBER ID NUMBER
NAME VARCHAR(17) COUNTRYCODE VARCHAR(3) CODE VARCHAR(10) CREATIONTIME TIMESTAMP
COUNTRYCODE VARCHAR(3) NAME VARCHAR(17) NAME VARCHAR(100) CUSTOMERID NUMBER
DISTRICT VARCHAR(20) CITYID NUMBER REFERENCE VARCHAR(50)
POPULATION NUMBER CREATIONTIME TIMESTAMP AMOUNT DECIMAL(10,2)
STATUS NUMBER STATUS NUMBER
So, respond to the next exercises:
● Query all columns for all Mexicans cities in CITY with populations larger than 100000. The CountryCode for Mexico is MX.
● Remove all rows which have population minor than 100, because its error.
● Update the rows which have the same district name, adding their countrycode to the same district
field.
district
---------------------------------
[district] ([countrycode])
● In which countries / cities do we have clients? In which countries do we not have clients?
● How many new customers we have by date in the last three months?
● Which are our top five countries/cities by total of customers?
● Which are our top five customers ordered by amount of sales, including the number and total amount of sales
● Which customers have more than three months without an invoice?
● What is the average amount of sales by country?
● Mark as inactive (STATUS = 0) all the customers with more than six months since its creation and without sales
● We need the number and amount of paid invoices (invoice STATUS = 2) and unpaid invoices (invoice STATUS = 1) by customer, for ALL the active customers (customer STATUS = 1)
● Add the country code of the customer to all the invoices reference
● Remove the cancelled invoices (invoice STATUS = 3) older than one year
CHALLENGE 3
Se tiene una instancia de mysql instalada en un servidor remoto con IP 192.168.217.131, que tiene configurado el uso del puerto 2222 para protocolo secure shell, además el servidor cuenta con tres usuarios de los cuales solo de dos se conocen sus credenciales, uno de ellos tiene accesos al comando mysql y el otro acceso remoto, el usuario con acceso a mysql de igual forma está registrado con acceso en la base de datos que se requiere tocar y puede listar nombre de tablas y nombres de columnas. La base de datos con el nombre online-music cuenta con una tabla donde se registran las pistas de audio cortas para su previsualización, por medio de una llave foránea se une con otra tabla que contiene el nombre y ruta de las pistas originales, se requiere encontrar la ubicación de los archivos originales de todas las pistas que se han previsualizado en el último mes a la fecha que pertenecen al artista Arjona. Se requiere tener este listado en un archivo en la ruta /data/queries/previews/arjona.csv el archivo debe tener permisos de lectura pero no de escritura ni de ejecución. Crear un diagrama ER que represente la base con las tablas y columnas que consideres necesarias. Plus, crear un archivo batch que cree el archivo final.
users
● root (?) se desconoce la contraseña
● admin (xyz1236) tiene acceso remoto pero no al comando mysql
● mysqlusr (lqsym) puede usar mysql pero no tiene acceso remoto
TODO:
1. Crear un archivo con el resultado de la búsqueda en mysql (describir el proceso y los
comandos necesarios) 2. Diagrama ER PLUS: Crear un archivo batch file
