# gatsby-starter-default
The default Gatsby starter.

For an overview of the project structure please refer to the [Gatsby documentation - Building with Components](https://www.gatsbyjs.org/docs/building-with-components/).

## Install

Make sure that you have the Gatsby CLI program installed:
```sh
npm install --global gatsby-cli
```

And run from your CLI:
```sh
gatsby new gatsby-example-site
```

Then you can run it by:
```sh
cd gatsby-example-site
npm run develop
```

## Deploy

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/gatsbyjs/gatsby-starter-default)

##Cheatsheet

###rfc + TAB
Create a functional based component (ES7)

###rcc + TAB
Class based component (ES7)

### Installed plugins:

npm i gatsby-source-filesystem - Needed for query our blogposts from filesystem

npm i gatsby-transformer-remark - Needed for transforming MD files into HTML rendered files

npm i gatsby-plugin-catch-links - intercept local links from MD and other unReact pages and push it, browser doesnt have to unload the pages

After install configure plugins in gatsby-config.js



##using GraphQL to grab markdown files

{
  allMarkdownRemark{
    edges{
      node{
        frontmatter{
          path
          title
          date
          author
        }
        excerpt
      }
    }
  }
}

