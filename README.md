# CODSOFT_TASK2

Project Summary: This is the task of the IRIS FLOWER dataset consists of three species: setosa, versicolor, and virginica. These species can be distinguished based on their measurements. Now, imagine that you have the measurements of Iris flowers categorized by their respective species. Your objective is to train a machine learning model that can learn from these measurements and accurately classify the Iris flowers into their respective species.


TOOL USED: SQL Server Management Studio (Transact-SQL)

CREATE DATABASE CODSOFT command is as follow:

    create database CODSOFT


CREATE TABLE IRIS command as follow:

    Create table IRIS
    (
    sepal_length float not null,
    sepal_width float not null,
    petal_length float not null,
    petal_width float not null,
    species varchar(20) not null
    )



INSERTING VALUES INTO IRIS TABLE, command as follow:


    INSERT INTO IRIS (sepal_length, sepal_width, petal_length, petal_width, species)
    VALUES
    (5.1, 3.5, 1.4, 0.2, 'Iris-setosa'),
    (4.9, 3, 1.4, 0.2, 'Iris-setosa'),
    (4.7, 3.2, 1.3, 0.2, 'Iris-setosa'),
    (4.6, 3.1, 1.5, 0.2, 'Iris-setosa'),
    (5, 3.6, 1.4, 0.2, 'Iris-setosa'),
    (5.4, 3.9, 1.7, 0.4, 'Iris-setosa'),
    (4.6, 3.4, 1.4, 0.3, 'Iris-setosa'),
    (5, 3.4, 1.5, 0.2, 'Iris-setosa'),
    (4.4, 2.9, 1.4, 0.2, 'Iris-setosa'),
    (4.9, 3.1, 1.5, 0.1, 'Iris-setosa'),
    (5.4, 3.7, 1.5, 0.2, 'Iris-setosa'),
    (4.8, 3.4, 1.6, 0.2, 'Iris-setosa'),
    (4.8, 3, 1.4, 0.1, 'Iris-setosa'),
    (4.3, 3, 1.1, 0.1, 'Iris-setosa'),
    (5.8, 4, 1.2, 0.2, 'Iris-setosa'),
    (5.7, 4.4, 1.5, 0.4, 'Iris-setosa'),
    (5.4, 3.9, 1.3, 0.4, 'Iris-setosa'),
    (5.1, 3.5, 1.4, 0.3, 'Iris-setosa'),
    (5.7, 3.8, 1.7, 0.3, 'Iris-setosa'),
    (5.1, 3.8, 1.5, 0.3, 'Iris-setosa'),
    (5.4, 3.4, 1.7, 0.2, 'Iris-setosa'),
    (5.1, 3.7, 1.5, 0.4, 'Iris-setosa'),
    (4.6, 3.6, 1, 0.2, 'Iris-setosa'),
    (5.1, 3.3, 1.7, 0.5, 'Iris-setosa'),
    (4.8, 3.4, 1.9, 0.2, 'Iris-setosa'),
    (5, 3, 1.6, 0.2, 'Iris-setosa'),
    (5, 3.4, 1.6, 0.4, 'Iris-setosa'),
    (5.2, 3.5, 1.5, 0.2, 'Iris-setosa'),
    (5.2, 3.4, 1.4, 0.2, 'Iris-setosa'),
    (4.7, 3.2, 1.6, 0.2, 'Iris-setosa'),
    (4.8, 3.1, 1.6, 0.2, 'Iris-setosa'),
    (5.4, 3.4, 1.5, 0.4, 'Iris-setosa'),
    (5.2, 4.1, 1.5, 0.1, 'Iris-setosa'),
    (5.5, 4.2, 1.4, 0.2, 'Iris-setosa'),
    (4.9, 3.1, 1.5, 0.1, 'Iris-setosa'),
    (5, 3.2, 1.2, 0.2, 'Iris-setosa'),
    (5.5, 3.5, 1.3, 0.2, 'Iris-setosa'),
    (4.9, 3.1, 1.5, 0.1, 'Iris-setosa'),
    (4.4, 3, 1.3, 0.2, 'Iris-setosa'),
    (5.1, 3.4, 1.5, 0.2, 'Iris-setosa'),
    (5, 3.5, 1.3, 0.3, 'Iris-setosa'),
    (4.5, 2.3, 1.3, 0.3, 'Iris-setosa'),
    (4.4, 3.2, 1.3, 0.2, 'Iris-setosa'),
    (5, 3.5, 1.6, 0.6, 'Iris-setosa'),
    (5.1, 3.8, 1.9, 0.4, 'Iris-setosa'),
    (4.8, 3, 1.4, 0.3, 'Iris-setosa'),
    (5.1, 3.8, 1.6, 0.2, 'Iris-setosa'),
    (4.6, 3.2, 1.4, 0.2, 'Iris-setosa'),
    (5.3, 3.7, 1.5, 0.2, 'Iris-setosa'),
    (5, 3.3, 1.4, 0.2, 'Iris-setosa'),
    (7, 3.2, 4.7, 1.4, 'Iris-versicolor'),
    (6.4, 3.2, 4.5, 1.5, 'Iris-versicolor'),
    (6.9, 3.1, 4.9, 1.5, 'Iris-versicolor'),
    (5.5, 2.3, 4, 1.3, 'Iris-versicolor'),
    (6.5, 2.8, 4.6, 1.5, 'Iris-versicolor'),
    (5.7, 2.8, 4.5, 1.3, 'Iris-versicolor'),
    (6.3, 3.3, 4.7, 1.6, 'Iris-versicolor'),
    (4.9, 2.4, 3.3, 1, 'Iris-versicolor'),
    (6.6, 2.9, 4.6, 1.3, 'Iris-versicolor'),
    (5.2, 2.7, 3.9, 1.4, 'Iris-versicolor'),
    (5, 2, 3.5, 1, 'Iris-versicolor'),
    (5.9, 3, 4.2, 1.5, 'Iris-versicolor'),
    (6, 2.2, 4, 1, 'Iris-versicolor'),
    (6.1, 2.9, 4.7, 1.4, 'Iris-versicolor'),
    (5.6, 2.9, 3.6, 1.3, 'Iris-versicolor'),
    (6.7, 3.1, 4.4, 1.4, 'Iris-versicolor'),
    (5.6, 3, 4.5, 1.5, 'Iris-versicolor'),
    (5.8, 2.7, 4.1, 1, 'Iris-versicolor'),
    (6.2, 2.2, 4.5, 1.5, 'Iris-versicolor'),
    (5.6, 2.5, 3.9, 1.1, 'Iris-versicolor'),
    (5.9, 3.2, 4.8, 1.8, 'Iris-versicolor'),
    (6.1, 2.8, 4, 1.3, 'Iris-versicolor'),
    (6.3, 2.5, 4.9, 1.5, 'Iris-versicolor'),
    (6.1, 2.8, 4.7, 1.2, 'Iris-versicolor'),
    (6.4, 2.9, 4.3, 1.3, 'Iris-versicolor'),
    (6.6, 3, 4.4, 1.4, 'Iris-versicolor'),
    (6.8, 2.8, 4.8, 1.4, 'Iris-versicolor'),
    (6.7, 3, 5, 1.7, 'Iris-versicolor'),
    (6, 2.9, 4.5, 1.5, 'Iris-versicolor'),
    (5.7, 2.6, 3.5, 1, 'Iris-versicolor'),
    (5.5, 2.4, 3.8, 1.1, 'Iris-versicolor'),
    (5.5, 2.4, 3.7, 1, 'Iris-versicolor'),
    (5.8, 2.7, 3.9, 1.2, 'Iris-versicolor'),
    (6, 2.7, 5.1, 1.6, 'Iris-versicolor'),
    (5.4, 3, 4.5, 1.5, 'Iris-versicolor'),
    (6, 3.4, 4.5, 1.6, 'Iris-versicolor'),
    (6.7, 3.1, 4.7, 1.5, 'Iris-versicolor'),
    (6.3, 2.3, 4.4, 1.3, 'Iris-versicolor'),
    (5.6, 3, 4.1, 1.3, 'Iris-versicolor'),
    (5.5, 2.5, 4, 1.3, 'Iris-versicolor'),
    (5.5, 2.6, 4.4, 1.2, 'Iris-versicolor'),
    (6.1, 3, 4.6, 1.4, 'Iris-versicolor'),
    (5.8, 2.6, 4, 1.2, 'Iris-versicolor'),
    (5, 2.3, 3.3, 1, 'Iris-versicolor'),
    (5.6, 2.7, 4.2, 1.3, 'Iris-versicolor'),
    (5.7, 3, 4.2, 1.2, 'Iris-versicolor'),
    (5.7, 2.9, 4.2, 1.3, 'Iris-versicolor'),
    (6.2, 2.9, 4.3, 1.3, 'Iris-versicolor'),
    (5.1, 2.5, 3, 1.1, 'Iris-versicolor'),
    (5.7, 2.8, 4.1, 1.3, 'Iris-versicolor'),
    (6.3, 3.3, 6, 2.5, 'Iris-virginica'),
    (5.8, 2.7, 5.1, 1.9, 'Iris-virginica'),
    (7.1, 3, 5.9, 2.1, 'Iris-virginica'),
    (6.3, 2.9, 5.6, 1.8, 'Iris-virginica'),
    (6.5, 3, 5.8, 2.2, 'Iris-virginica'),
    (7.6, 3, 6.6, 2.1, 'Iris-virginica'),
    (4.9, 2.5, 4.5, 1.7, 'Iris-virginica'),
    (7.3, 2.9, 6.3, 1.8, 'Iris-virginica'),
    (6.7, 2.5, 5.8, 1.8, 'Iris-virginica'),
    (7.2, 3.6, 6.1, 2.5, 'Iris-virginica'),
    (6.5, 3.2, 5.1, 2, 'Iris-virginica'),
    (6.4, 2.7, 5.3, 1.9, 'Iris-virginica'),
    (6.8, 3, 5.5, 2.1, 'Iris-virginica'),
    (5.7, 2.5, 5, 2, 'Iris-virginica'),
    (5.8, 2.8, 5.1, 2.4, 'Iris-virginica'),
    (6.4, 3.2, 5.3, 2.3, 'Iris-virginica'),
    (6.5, 3, 5.5, 1.8, 'Iris-virginica'),
    (7.7, 3.8, 6.7, 2.2, 'Iris-virginica'),
    (7.7, 2.6, 6.9, 2.3, 'Iris-virginica'),
    (6, 2.2, 5, 1.5, 'Iris-virginica'),
    (6.9, 3.2, 5.7, 2.3, 'Iris-virginica'),
    (5.6, 2.8, 4.9, 2, 'Iris-virginica'),
    (7.7, 2.8, 6.7, 2, 'Iris-virginica'),
    (6.3, 2.7, 4.9, 1.8, 'Iris-virginica'),
    (6.7, 3.3, 5.7, 2.1, 'Iris-virginica'),
    (7.2, 3.2, 6, 1.8, 'Iris-virginica'),
    (6.2, 2.8, 4.8, 1.8, 'Iris-virginica'),
    (6.1, 3, 4.9, 1.8, 'Iris-virginica'),
    (6.4, 2.8, 5.6, 2.1, 'Iris-virginica'),
    (7.2, 3, 5.8, 1.6, 'Iris-virginica'),
    (7.4, 2.8, 6.1, 1.9, 'Iris-virginica'),
    (7.9, 3.8, 6.4, 2, 'Iris-virginica'),
    (6.4, 2.8, 5.6, 2.2, 'Iris-virginica'),
    (6.3, 2.8, 5.1, 1.5, 'Iris-virginica'),
    (6.1, 2.6, 5.6, 1.4, 'Iris-virginica'),
    (7.7, 3, 6.1, 2.3, 'Iris-virginica'),
    (6.3, 3.4, 5.6, 2.4, 'Iris-virginica'),
    (6.4, 3.1, 5.5, 1.8, 'Iris-virginica'),
    (6, 3, 4.8, 1.8, 'Iris-virginica'),
    (6.9, 3.1, 5.4, 2.1, 'Iris-virginica'),
    (6.7, 3.1, 5.6, 2.4, 'Iris-virginica'),
    (6.9, 3.1, 5.1, 2.3, 'Iris-virginica'),
    (5.8, 2.7, 5.1, 1.9, 'Iris-virginica'),
    (6.8, 3.2, 5.9, 2.3, 'Iris-virginica'),
    (6.7, 3.3, 5.7, 2.5, 'Iris-virginica'),
    (6.7, 3, 5.2, 2.3, 'Iris-virginica'),
    (6.3, 2.5, 5, 1.9, 'Iris-virginica'),
    (6.5, 3, 5.2, 2, 'Iris-virginica'),
    (6.2, 3.4, 5.4, 2.3, 'Iris-virginica'),
    (5.9, 3, 5.1, 1.8, 'Iris-virginica');

    

Retrive all rows from the IRIS table

    select * from IRIS


Retrieve specific columns from the IRIS table

    SELECT sepal_length, species 
    FROM IRIS


Retrieve rows that meet specific conditions. For instance, to select all rows where sepal_length is greater than 6.0

    SELECT sepal_length, species
    FROM IRIS 
    WHERE sepal_length > 6.0


Sort the data based on a specific column. To retrieve all rows sorted by petal_length in ascending order

    SELECT petal_length, species 
    FROM IRIS 
    ORDER BY petal_length 


To find the average sepal_length for each species:

    SELECT species, AVG(sepal_length) AS avg_sepal_length
    FROM IRIS
    GROUP BY species


Count the number of rows that meet specific conditions. To count the rows where species is 'Iris-setosa':

    SELECT species, COUNT(*) AS TotalSpecies
    FROM IRIS
    WHERE species = 'Iris-setosa'
    GROUP BY species


To count the rows where species is 'Iris-versicolor':

    SELECT species, COUNT(*) AS TotalSpecies
    FROM IRIS
    WHERE species = 'Iris-versicolor'
    GROUP BY species


To count the rows where species is 'Iris-virginica':

    SELECT species, COUNT(*) AS TotalSpecies
    FROM IRIS
    WHERE species = 'IRIS-virginica'
    GROUP BY species


To retrive Minimum Value for Sepal_Length:

    SELECT MIN(sepal_length) AS min_sepal_length 
    FROM IRIS


To retrive Maximum Value for Petal_Length:

    SELECT MAX(petal_length) AS max_petal_length 
    FROM IRIS
    
