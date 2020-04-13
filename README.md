# Playing with scala - ReST

Source code for https://plippe.github.io/blog/2020/04/01/playing-with-scala-rest.html

```sh
-> curl localhost:9000/pets curl
[]

-> curl localhost:9000/pets -d '{"name": "dog"}' -H 'Content-Type: application/json'
{"id":"4d1a1036-b4ff-4c5f-8f80-6ed6bd20c865","name":"dog"}

-> curl localhost:9000/pets
[{"id":"4d1a1036-b4ff-4c5f-8f80-6ed6bd20c865","name":"dog"}]

-> curl localhost:9000/pets/4d1a1036-b4ff-4c5f-8f80-6ed6bd20c865 -X DELETE

-> curl localhost:9000/pets
[]
```
