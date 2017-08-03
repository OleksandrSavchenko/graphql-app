# GraphQL App

## To run server and json-server use:
    npm run server
    npm run json:server

## Flow on GraphiQL
    Go to http://localhost:4000/graphql
    ### To get all customers use:
        query {
          customers {
            id,
            name,
            email,
            age
          }
        }