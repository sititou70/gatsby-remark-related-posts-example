# gatsby-remark-related-posts-example

The example blog repo of [gatsby-remark-related-posts](https://www.npmjs.com/package/gatsby-remark-related-posts)

try:

```
git clone [this repo's url]
cd gatsby-remark-related-posts-example
npm i
npm start
```

open `http://localhost:8000/___graphql` and then execute the following query.

```
// query
query {
  allMarkdownRemark {
    nodes {
      fileAbsolutePath
      fields {
        relatedFileAbsolutePaths
      }
    }
  }
}
```
