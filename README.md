# PRISMA CRUD BOILERPLATE

This small project is meant to show how to perform a CRUD in Prisma for future references, to make one from scratch follow these steps:

- Create a folder with the name of your project and use the commands **npm init** then **git init**
- Create a folder called **src** and inside make an index.js file.
- On the root in your terminal **yarn add graphql-yoga prisma-client-lib nodemon**
- Create a prisma folder inside your root and add the datamodel.prisma of this project and for the prisma.yml:

```javascript
endpoint: ''

datamodel: datamodel.prisma

generate:
  - generator: javascript-client
    output: ../src/generated/prisma-client
```

- On the terminal use the command **prisma deploy** to setup your prisma ORM.
- Then use **prisma generate** to use the datamodel as reference to create the necesary data to connect to the database you chose when you deployed with prisma.
- And finally inside your index.js file in src folder you can simply copy paste the content.

You can always **git clone** this project as well and remove the EP and generated folder then make it your own with prisma deploy and prisma generate.

## Conclusion

Learning Prisma, Apollo and GraphQL were not that hard, but it's good to have a concise reference for everything you learn, in my case I'm not sure if I be using GraphQL or REST in the future, but both options are really good, although I'm more inclined to REST due to it being easier to read and write. I personally find resolvers too much of a pain to write and finding information about this setup is harder than with REST.

**Made by Eng Adrian Beria**
