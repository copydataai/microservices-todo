# microservices-todo

**This Project isn't finish**

> This is a project to improve and reforce my knowledge in microservices

- I've been building this project like monorepo to scale with **DDD**

## Routes

### routes frontend

- `todo.copydataai.com`
  - `/` general dashboard
- `account.todo.copydataai.com`
  > Using aws cognito
  - `/login`
  - `/signup`
- `app.todo.copydataai.com`
  - `/` list all projects
  - `/{project_name}` get project with all tasks
    - create a modal to modify tasks like jira

### API endpoints

`api.todo.copydataai.com`

- **GET** `/todos` List all todos
- **GET** `/todos/{TodoID}` Get todo specific
- **POST** `/todos` create a project in format xxxform just for upload pictures
- **PATCH/PUT** `/todos{TodoID}` update a project
- **DELETE** `/tasks/{TodoID}` delete a project and continue to delete tasks

- **GET** `/tasks` List all tasks from a todo by query example: `by projects, priority, state`
- **GET** `/tasks/{TaskID}` Get a specific todo
- **POST** `/tasks` create a task in format xxxform just for upload pictures
- **PATCH/PUT** `/tasks{TaskID}` update a task
- **DELETE** `/tasks/{TaskID}` delete a task

### Stack

- MongoDB for multi pooling and horizontal scale
- Go like main language in microservices
- TurboRepo with PNPM for deploy multiple apps
- Stack Grafana support to OSS :)
- S3 for manage all zip containers to deploy in microservices
- Docker to try in local before to use in terraform
- PReact a light version from React
- Terraform for easy deploy and use like CDK(Cloud Developer Kit)
- use Github Actions like Pipeline

### License

MIT License
You can create your own todo oriented to microservices from free.
