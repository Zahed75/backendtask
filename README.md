# Welcome Backend-focused Product Task By Syscomatic

```
TIMEBOX:    Deadline 3days. We mean it! Set at timer and hard-stop at 4 hours ⏱
LANGUAGES:  Python, Javascript
FRAMEWORKS: Django, Flask, NodeJS, etc (Exercise MongoDD or MySQL)
TESTS:      nice to have, but not mandatory
DOCS:       nice to have, but not mandatory
```

## Overview

This exercise is to implement the best possible solution to one of the exercises below in the time alloted. We're evaluating your ability to take a set of requirements and spike a holistic solution that demonstrates craftsmanship, thoughtfulness and good architectural design. This is **NOT** a test of how well you know Node.js/Python/Django/Flask/SQL, nor should you try to impress us with overly clever and obtuse solutions. If you want to impress us, build something that is beautiful, intuitive and easy to debug/test/extend :smiley: .

Ideally your solution would have some way to run locally and test the results so we can fully analyze your efforts.


```
You Have to install MongoDB Compass and create a Database 
as your preferred name then import all off the Json files

[/Dabases/example.json]

```


```
ROLE BASED ACCESS CONTROL:(RBCA)
role: {
      type: String,
      //  ACO -> Account Owner
      // BM -> Brand Manager
      // OM -> Outlet Manager
      //SA -> Super Admin
      enum: ['ACO', 'BM', 'OM', 'SA'],
      require: [true, 'Role must be selected'],
    }

      orderStatus: {
      type: Number,
      [0 cancelled, 1 pending, 2 confirmed, 3 rider confimed, 4 waiting,
      5 on the way(Dispatch)
      ]
      enum: [0, 1, 2, 3, 4, 5],
      default: 1,
    }

```




## RAPID API:COMPLETE TWO TASK

---

> :rotating_light: :exclamation: :point_right: **Please import the all json format data into your MongoDB compass [CLOUD-KITCHEN]** :point_left: :exclamation: :rotating_light:


### Exercise A: Expose an API for querying some Statical Data


The goal of this exercise is to design a read-only API (REST) that returns one or more records from static set of compensation data.

#### User Story: As a developer I want to

* list compensation data via API `GET` request

  * Get Outlet Based On Heat and show(API)-Permission only (SUPER ADMIN)

  * Make and EndPoint Outlet Heat Average(API)-Permission only (SUPER ADMIN,ACCOUNT OWNER)




* fetch a single record via GET request

  * **Stretch Goal**:  Return Total Order By Outlet(API)-Permission only (SUPER ADMIN,ACCOUNT OWNER)

  * **Stretch Goal**: Get Cutomer History By Brand(API)--Permission only (SUPER ADMIN,ACCOUNT OWNER)


### A few quick notes on submitting Exercise A

* Don't worry about any web application concerns other than serializing JSON and returning via a GET request.
* The example above (`/Database`...) is not a contract. Feel free to design the URL structure and JSON schema that you believe creates the best client/consumer experience

---

## Exercise B: Database Design Exercise - Storing Compensation Data

* search Discount by Brand
* Get Top Performing Brands

---

## Submit your Task with Proper Documentation and Github Repo Link Postman Public webview at this mail tech.syscomatic@gmail.com



