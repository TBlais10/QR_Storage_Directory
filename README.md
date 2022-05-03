
# QR Storage

QR Storage is an application built based on personal experiences of working in several 
different warehouses with several different programs. This program is made for the 
everyday hobbiest to the enterprize company who needs to track their massive inventories
across several locations and sites. QR codes would be uniquely created for each item and
those codes would be recieved and processed into each location and site respectively
through a user's phone or company phone, eliminating the middle man of an RF scanner or
other pieces of hardware.


## Java Backend Install

Clone the project

```bash
  git clone https://github.com/TBlais10/QR_Storage
```

Go to the project directory

```bash
  cd QR_Storage
```
Run Springboot in of your IDE (Intelij Idea Recommended)

## Installation

Install my-project with npm

Clone the project

```bash
git clone https://github.com/TBlais10/QR_StorageReact
```

```bash
  npm install qr_storage
  cd qr_storage
```

To run the application

```bash
npm start
```
## API Reference

#### Create an account

```http
  POST /api/auth/signup
```

| Parameter  | Type     | Description                            |
| :--------- | :------- | :------------------------------------- |
| `username` | `string` | **Required**. Give us an email address |
| `password` | `string` | **Required**. Create a unique password |

#### Login to the system

```http
  POST /api/auth/signin
```

| Parameter  | Type     | Description                            |
| :--------- | :------- | :------------------------------------- |
| `username` | `string` | **Required**. Use your email address   |
| `password` | `string` | **Required**. Create a unique password |


#### Create an item

```http
  POST /api/items/
```

| Parameter     | Type     | Description                         |
| :------------ | :----------- | :---------------------------------- |
| `name`        | `string`     | **Required**. Item must have a name |
| `description` | `string`     | What the item is                    |
| `cond`        | `string`     | What condition is the item in       |
| `tags`        | `string`     | What are the tags you want to assign to this item` |
| `status`      | `string`     | **Required**. What is the condition of the item in |
| `color`       | `string`     | What is the color of the item |
| `serialNumber`| `string`     | Does this item have a Serial Number |
| `price`       | `BigDecimal` | What is the price of this item |

Returns the newly created Item in a JSON Body




## Links to Project Repos

### Java Backend

https://github.com/TBlais10/QR_Storage

### React Frontend

https://github.com/TBlais10/QR_StorageReact

