# GraphQl queries

</br>

```bash
query {
  getAllPosts {
    id
    title
    description
  }
  getPost(id: "60c92128a9325f3fd403a204") {
    title
    description
  }
}

# The following will make description equal to null
# The above is now fixed via your resolvers updates logic!
mutation {
  updatePost(id: "60c920f8a9325f3fd403a202", post: {
    title: "First post title NEWEST"
  }) {
    id
    title
    description
  }
  
  createPost(post: {
    title: "My second post"
    description: "This is the description..."
  }) {
    id
    title
    description
  }
  deletePost(id: "60c92128a9325f3fd403a204")
}
```
