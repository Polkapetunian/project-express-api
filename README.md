# Express API Project

The purpose of this project was to practise creating a RESTful API using Express.



## The problem

In the project we should add a dataset as a JSON . I got a dataset of nuclear plants in the world from https://www.kaggle.com/liananapalkova/nuclear-power-plants. It came in CSV format and was converted to JSON on https://csvjson.com/. 

## API Documentation
NUCLEAR POWER PLANTS API VERSION 1

This API provides data on nuclear plants and reactors in the world. Here is the description of the dataset from the creator Liana Napalkova: "This dataset combines information from a global dataset developed by Declan Butler of Nature News and the Power Reactor Information System (PRIS), an up-to-date database of nuclear reactors maintained by the International Atomic Energy Agency (IAEA). The locations of nuclear reactors around the world are represented as point features associated with reactor specification and performance history attributes as of March 2012."

Disclaimer: I cannot guarantee that the data is up-to-date. According to information on kaggle.com, the dataset was updated three years ago. This API is for practise purposes and will not be updated.
_____________________________________________________________________________________________________

### Endpoints

The API har several endpoints:

**List of endpoints**
https://nuclear-plants-api.herokuapp.com/

(Possible queries not included)

**All power plants and reactors**

https://nuclear-plants-api.herokuapp.com/nuclear-power-plants 

Displays the whole dataset, information on all nuclear power plants and reactors. 

Filter on country
Add your query like this:
/nuclear-power-plants/?country=finland
This query is not case sensitive and you can type part of the name of a country. Be aware that if you e.g. type "united", you will get results of both United Kingdom and the United States of America. 

**Power plants and reactors by ID**

https://nuclear-plants-api.herokuapp.com/:id
Displays one reactor/power plant that has the ID that matches the one inserted in the end of the URL. The ID is a number from 0 to 275.

## View it live

Use one of these endpoints:

https://nuclear-plants-api.herokuapp.com/nuclear-power-plants

https://nuclear-plants-api.herokuapp.com/nuclear-power-plants/{id}
