# Camunda Tasklist API Connector
[Camunda Platform](https://signup.camunda.com/accounts) is a SaaS offering for Process Automation from [Camunda](https://camunda.com).

This connector is provided by [BP3 Global](https://www.bp-3.com), a Camunda Platinum Partner offering Process Automation solutions. 
Please contact [support@bp-3.com](mailto:support@bp-3.com).

## API Description
Camunda Cloud SaaS is actually split into a number of separate components, e.g.

- Tasklist
- Operate

and thus the API is broken down in a similar way - so, you will typically need to use at least Tasklist and Operate 
API Connectors to develop a Camunda based solution.

## Prerequisites
You will need the following to proceed:

- A Microsoft Power Apps or Power Automate plan with custom connector feature
- Access to a [Camunda Platform account](https://signup.camunda.com/accounts)

## Supported Operations

### Form
- `getForm` Get the form details by form id and processDefinitionKey.

### Variables
- `getVariableById` Get the variable details by variable id.

### Task
  - `searchTaskVariables` Returns the list of task variables.
  - `searchTasks` Returns the list of tasks that satisfy search request params.
  - `unassignTask` Unassign the task with the provided id. Returns the task.
  - `completeTask` Complete a task with task id and optional variables. Returns the task. 
  - `assignTask` Assign a task with id to assignee. Returns the task.
  - `getTaskById` Get on task by id. Returns task or error when task does not exist.
