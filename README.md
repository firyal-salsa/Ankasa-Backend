<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="https://res.cloudinary.com/calvin-cloud/image/upload/v1631588597/Ankasa/Logo_Ankasa_cm4gp9.svg"  alt="LogoAnkasa">
  </a>
  
<p align="center"><img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634282728/arkademy_ufgxux.png" width="200px" alt="Arkademylogo.svg" /></p>

<p>Ankasa is booking ticket plane web application. The backend has a jwt (json web token) to secure accounts from other users, a bcrypt package to protect passwords, and other dependencies to complete the needs of the Ankasa application. To find out information about Ankasa please see below.</p>

## Build

<div class="d-flex">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634289445/tech%20stack/express_xmzka6.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1635367909/tech%20stack/yarn_ztjuf7.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225494/tech%20stack/postgresql_r813wd.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225451/tech%20stack/redis_agonqb.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225449/tech%20stack/nginx_sapsks.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225445/tech%20stack/aws-ec2_xkv0gc.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225443/tech%20stack/docker-icon_hamwmv.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1634225440/tech%20stack/jenkins_xhlzk0.svg" width="50px" height="50px">
<img src="https://res.cloudinary.com/dvehyvk3d/image/upload/v1635367893/tech%20stack/kubernetes_qyuz5v.svg" width="50px" height="50px">
</div>

## View Demo
https://ankasa.online/

## Frontend

https://github.com/firyal-salsa/Ankasa-Frontend

## Clone the repository

```bash

  git clone https://github.com/firyal-salsa/Ankasa-Backend
  
```

### Install dependencies
```bash

  yarn install
  
```

### run app
```bash

  cd back-ticketing

  yarn start
  
```

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn build`

```bash

  yarn run build
  
```
## for developer

### standar request login 
```bash
  {
    "email": "user",
    "password":"user1234"
  }
```

### standar request register
```bash
  {
    "name": "user",
    "email": "user@mail.com",
    "password": "user1234"
```

### standar response ticket API
```bash
  [
    { 
      "id" : "1",
      "uuid": "AB-221",
      "image": "img.jpg",
      "maskapai" : "Garuda Indonesia",
      "from": "Indonesi",
      "to": "Tokyo",
      "time": {
            "depature": "00:00",
            "arrived": "04:00",
            "transit": "1",
          },
       "price": {
            "idclass": 3,
            "class": "Economy",
            "adult": 1200000,
            "child": 800000,
          },
       "date": "Monday, 20 july 20",
       "chairsAmount": 108,
       "gate": 221,
       "terminal": "A",
    }
  ]
```

### standar request booking ticket
```bash
{
  "title": "Mr.",
  "name": "Budi",
  "nationallity": "Indonesia",
  "userId": 1,
  "idTicket": "AB-221",
  "Price": 3000000,
  "statusPay": false,
}
  
```

### standar response destination
```bash
[
  {
    "id": 1,
    "city": "Jakarta",
    "country": "Indonesia",
    "image": "image"
   }
]
```

### standar request booking ticket
```bash
[
  {
    "idSchedule": "A-212",
    "namePerson": "Mike Kowalski",
    "emailPerson": "mikekowalski@gmail.com",
    "phonePerson": "+62-819876563",
    "namePassenger": "Mike Kowalsky",
    "nationality": "indonesia",
    "totalPrice": 145,
    "insurance" false,
  }
]
```
