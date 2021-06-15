# GraphQl queries

</br>

```bash
query {
  # getAllPosts {
  #   id
  #   title
  #   description
  # }
  getPost(id: "60c92128a9325f3fd403a204") {
    title
    description
  }
}

# mutation {
#   createPost(post: {
#     title: "My second post"
#     description: "This is the description..."
#   }) {
#     id
#     title
#     description
#   }
# }
```
