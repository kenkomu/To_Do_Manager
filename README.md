# Todo List Manager


The application will allow users to add tasks, mark them as completed, and view their list of tasks. I am using Cartesi, and the results can be fetched using the GraphQL interface.

Features:

1. Add Task: Users can add a task to their todo list.
2. Complete Task: Users can mark a task as completed.
3. List Tasks: Users can view all tasks, with an indication of whether they are completed or not.


# Installation instructions
([]https://docs.cartesi.io/cartesi-rollups/1.3/development/installation/)

# Steps
1. Clone the repository
2. Run cd User_Sentence_Management
3. Run cartesi build
4. Run cartesi run
5. Run cartesi send on a new terminal tab and send a generic input to the application using foundry following the necessary steps.
6. visit the graphql endpoint ([]http://localhost:8080/graphql) on the browser.
```
query notices {
  notices {
    edges {
      node {
        index
        input {
          index
        }
        payload
      }
    }
  }
}
```
7. Inspect a request of the transactions count on the browser using this ([]http://localhost:8080/inspect)