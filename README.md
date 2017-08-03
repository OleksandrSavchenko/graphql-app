# GraphQL App

## To run server and json-server use:
    npm run server
    npm run json:server

## Flow on GraphiQL
    Go to http://localhost:4000/graphql

    To get all customers use:
        query {
          customers {
            id,
            name,
            email,
            age
          }
        }

    To get customer with id "id" use:
        query {
          customer(id: "id") {
            name,
            email,
            age
          }
        }

    To create new customer with name "name", email "email", and age number use:
        mutation {
          addCustomer(name: "name", email: "email", age: number) {
            id,
            name,
            email,
            age
          }
        }
    To remove customer with id "id" use:
        mutation {
          deleteCustomer(id: "id") {
            id
          }
        }
    To edit customer use:
        mutation {
          addCustomer(id: "id", name: "name", email: "email", age: number) {
            id,
            name,
            email,
            age
          }
        }