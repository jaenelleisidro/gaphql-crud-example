# gaphql-crud-example
a simple graphql code that will be used as reference for future projects



this code is available on git https://github.com/jaenelleisidro/gaphql-crud-example

this is created by following this tutorial
https://codingshiksha.com/javascript/build-a-graphql-server-crud-api-in-node-js-and-express-using-express-graphql-library-full-project-for-beginners/

there is a video version of that tutorial will leave it here in case you prefer a video
https://www.youtube.com/watch?v=PpCF8yRtd_A



# Let's begin

well just follow the tutorial, the only mistakes are 

GraphQLNonNull(GraphQLInt) should be new GraphQLNonNull(GraphQLInt)

and it forgot to include the schema on the middleware

app.use('/graphql', graphqlHTTP({graphiql: true})); 
should be
app.use('/graphql', graphqlHTTP({schema,graphiql: true}));