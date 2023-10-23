<p align="center">
  <img src="https://user-images.githubusercontent.com/53148314/193017087-50462d66-4ef8-4d36-8107-453af542bb2b.png" height="100">
  <h3 align="center">Rent A Car Fake Backend</h3>
  <p align="center">
    Fake Backend service of Rent A Car project for frontend tutorials.
  </p>
</p>

## ⚙️ Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/ahmet-cetinkaya-instruction/rent-a-car-fake-backend.git
   ```
2. Change your directory in the terminal:
   ```sh
   cd rent-a-car-fake-backend
   ```
3. Install the required packages:
   ```sh
   npm install
   ```
4. Copy the `.env.example` file and rename it to `.env`.
5. Edit the `.env` file and set the value of the `JWT_SECRET_KEY` property to a random string of your choice.

## 🚀 Usage

### Start project

```sh
npm start
```

### 🔀 Routes

- **CRUD operations: [json-server routes](https://github.com/typicode/json-server/blob/master/README.md#routes)**

- **Auth operations:**

| Route           | Comment                                  | Body                                   | Header                                   | Return                                   |
| --------------- | ---------------------------------------- | -------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| auth/login      | Login process to authenticate users      | `{userName: string, password: string}` |                                          | `{success:boolean, access_token:string}` |
| auth/test       | Test the validity of your access token   |                                        | Authorization: `"Bearer <access_token>"` | `{success:boolean, message:string}`      |
| auth/test-admin | Test if your access token has admin role |                                        | Authorization: `"Bearer <access_token>"` | `{success:boolean, message:string}`      |
