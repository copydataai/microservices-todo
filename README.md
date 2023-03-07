# microservices-todo
**This Project isn't finish**
> This is a project to improve and reforce my knowledge in microservices

- I've been building this project like monorepo to scale with **DDD**


## Routes
### routes frontend
- `account.todo.copydataai.com`
  - `/` general dashboard
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
- **POST** `/tasks` create a project in format xxxform just for upload pictures 
- **PATCH/PUT** `/tasks{TaskID}` update a project
- **DELETE** `/tasks/{TaskID}` delete a project and continue to delete tasks

- **GET** `/tasks` List all tasks from a todo by query example: `by projects, priority, state`
- **GET** `/tasks/{TaskID}` Get a specific todo 
- **POST** `/tasks` create a task in format xxxform just for upload pictures 
- **PATCH/PUT** `/tasks{TaskID}` update a task
- **DELETE** `/tasks/{TaskID}` delete a task

### Stack 
**I've been choosing a database**
  - Go to use events with apiGateway
  - Stack Grafana support to OSS :)
  - S3 for manage all zip containers to deploy in microservices
  - S3 to manage assets
  - Docker to try in local before to use in terraform
  - PReact a light version from React
  - Tailwind to more confident with css 
  - Terraform for easy deploy 
  - use Github Actions like Pipeline 
  - Docker to build container and binary for deploy in AWS
