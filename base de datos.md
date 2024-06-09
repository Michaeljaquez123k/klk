create database actividad3;

use actividad3;

create table actividad3(
id int primary key, 
nombre varchar (255),
edad int);

create table actividad3(
id int primary key auto_increment,
nombre varchar (50),
edad int);

create table padre(
id  int primary key,
nombre varchar(50)
);

create table hija(
id int primary key,
nombre varchar(255),
tabla_padre_id INT,
 FOREIGN KEY (tabla_padre_id) REFERENCES tabla_padre(id)
);
