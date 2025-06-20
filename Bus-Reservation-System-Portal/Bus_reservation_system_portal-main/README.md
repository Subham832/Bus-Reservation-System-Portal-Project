# REST API for Bus Reservation System Portal 

* Developed this REST API for a Bus Reservation System Portal Application. This API performs all the fundamental CRUD operations of any Bus Reservation Application platform with user validation at every step.
 
## Tech Stack

* Java
* Spring Framework
* Spring Boot
* Spring Data JPA
* Hibernate
* MySQL

## Modules

* Login, Logout Module
* Admin Module
* User Module
* Route Module
* Bus Module
* Reservation Module
* Feedback Module

## Features

* User and Admin authentication & validation with session uuid.
* Admin Features:
    * Administrator Role of the entire application
    * Only registered admins with valid session token can add/update/delete route and bus from main database
    * Admin can access the details of different users and reservations.
* User Features:
    * Registering themselves with application, and logging in to get the valid session token
    * Viewing list of available buses and booking a reservation
    * Only logged in user can access his reservations, profile updation and other features.

## Installation & Run

* Before running the API server, you should update the database config inside the [application.properties](https://github.com/Subham832/Bus-Reservation-System-Portal-Project/
blob/4264b3beff0c004e9a69af3ed2eeaa82d351805c/Bus-Reservation-System-Portal
/Bus_reservation_system_portal-main/Bus_Reservation_System_Portal/src/main/resources
/application.properties) file. 
* Update the port number, username and password as per your local database config.

```
    server.port=8888

    spring.datasource.url=jdbc:mysql://localhost:3306/sb201db
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    spring.datasource.username=root
    spring.datasource.password=admin

```

## API Root Endpoint

`https://localhost:8888/`

`http://localhost:8888/swagger-ui/`


## API Module Endpoints

### Login Module

* `POST //login/admin` : Admin can login with mobile number and password provided at the time of registation
<!--
### User Module


* `POST /customer/login` : Logging in customer with valid mobile number & password
* `GET /customer/availablecabs` : Getting the list of all the available cabs
* `GET /customers/cabs` : Getting All the cabs
* `GET /customers/checkhistory` : Getting the history of completed tr
* `PUT /customer/update/{mobile}` : Updates customer details based on mobile number
* `PATCH /customer/updatepassword/{mobile}` : Updates customer's password based on the given mobile number
* `POST /customer/booktrip` : Customer can book a cab
* `POST /customer/updatetrip` : Customer can modify or update the trip
* `POST /customer/logout` : Logging out customer based on session token
* `DELETE /customer/delete` : Deletes logged in user 
* `DELETE /customer/complete/{tripid}` : Completed the trip with the given tripid 
* `DELETE /customer/canceltrip` : Cancel the trip with the given tripid   


### Admin Module

* `POST /admin/register` : Register a new admin with proper data validation and admin session
* `POST /admin/login` : Admin can login with mobile number and password provided at the time of registation
* `GET /admin/logout` : Logging out admin based on session token
* `GET /admin/listoftripsbycustomer` : Get list of trips of by a customer id
* `GET /admin/listoftrips` : Get list of trips of all the trips
* `GET /admin/listocustomers` : Get list of all the customers
* `GET /admin/listodrivers` : Get list of all the drivers
* `PUT /admin/update/{username}` : Updates admin detaisl by passed user name
* `DELETE /admin/delete` : Deletes the admin with passed id   -->


### Sample API Response for Admin Login

`POST   localhost:8888/login/admin`

* Request Body

```
    {
        "mobileNo": "73x85y60a4",
        "password": "Subham@832"
    }
```

* Response

```
   CurrentAdminSession( adminId=10, uuid=ZaVLaK,localDatetime=2022-10-01 12:29:52.376508)
   

# THANK YOU EVERYONE FOR VISITING MY PROJECT

---
