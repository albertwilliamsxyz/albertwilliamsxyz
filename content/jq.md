INCOMPLETE

# JQ: A JSON Query language

Today I want to talk a little about a CLI utility that I find pretty useful when dealing with data serialized as JSON, it is `jq`. This utility is both CLI JSON processor and a domain-specific language available for GNU/Linux, Mac OS and even Windows. The reason why it is useful is because it lets you apply transformations on data with a language that is easy-to-use but at the same time extremely powerful and designed specifically for that purpose, and since it is a CLI utility, you can pipe it with different utilities to build a pipeline with the ability to process JSON objects on the fly.

The best way to visualize how useful it is is through a little example. Let's assume that you have a REST API that lets you request information about movies, and that it has an endpoint to list all the movies in the database. The response from that endpoint is an object that contains a many fields that may or may not be important for you. That response could look like (this)[https://gist.githubusercontent.com/albertwilliamsxyz/d70130caaca350beed3dda9d77850069/raw/a9d4a275285ca88238a7236d3beed660e89ac3c8/movies.json]. As you can see, this JSON is too big, and it is hard to visualize due to its size. The reason why you are querying the list of movies is because you want to know if there are movies

