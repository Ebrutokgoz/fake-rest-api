### Creating FAKE REST API using the json-server npm package

1. Run **npm init** command to create a package.json file.
2. Run **npm i json-server** command to download the json-server package.
3. Update package.json

```
   "scripts": {
   "start:server": "json-server --watch students.json"
   },
```

4. Use **npm run start:server** command to run Fake Api.

Request examples:

- Get all students - GET : http://localhost:3000/students
- Get a student with id - GET : http://localhost:3000/students/:student_id
- Students - Department relation - GET : http://localhost:3000/students?\_expand=department
- Add a student - POST : http://localhost:3000/students
- Update a student - PATCH(PUT) : http://localhost:3000/students/:student_id
- Delete a student - DELETE : http://localhost:3000/students/:student_id

We may need dummy or fake APIs

- to test an application with a ready frontend.
- to create a prototype for a backend work we are considering.
- to make requests for different HTTP methods on an API platform like Postman.
