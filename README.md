# graphql-demo

## Sample queries:

Get all book names:

```
{
  books {
    name
  }
}

```
Get all book names with auther names

```
{
  books {
    name,
    author{
      name
    }
  }
}



```

Get all books by auther id:

```
{
  author(id : 1){
    name,
    books{
      name
    }
  }
}
```

Add new book
```
mutation {
  addBook(name: "new book", authorId: 1){
    name,
    id
  }
}
```
