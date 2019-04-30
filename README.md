# MongoDB Exercises

# Special offers inside,

## Some Assembly Required

# Author - Michel Roberts JR.

# Modified by Travis Ripley, \* Started Tuesday April 30th, 2019 15:30

## Right after this commercial break:

MongoDB Exercise in mongo shell

Connect to a running mongo instance, use a database named `mongo_exercises`.

Document all your queries in a javascript file to use as a reference.

1. Clone the repository from [github](https://github.com/SanDiegoCodeSchool/db200-mongodb-exercises)

## Insert Documents

Insert the following documents into a `movies` collection.

```
title : Star Wars
writer : George Lucas
year : 1977
actors : [
  Mark Hamill
  Harison Ford
  Carrie Fisher
  Peter Chushing
  James Earl Jones
]
```
```
title : Raiders of the Lost Ark
writer : George Lucas
year : 1981
actors : [
  Harrison Ford
]
```
```
title : Fight Club
writer : Chuck Palahniuk
year : 1999
actors : [
  Brad Pitt
  Edward Norton
]
```
```
title : Pulp Fiction
writer : Quentin Tarantino
year : 1994
actors : [
  John Travolta
  Uma Thurman
]
```
```
title : Inglorious Basterds
writer : Quentin Tarantino
year : 2009
actors : [
  Brad Pitt
  Diane Kruger
  Eli Roth
]
```
```
title : The Hobbit: An Unexpected Journey
writer : J.R.R. Tolkein
year : 2012
franchise : The Hobbit
```
```
title : The Hobbit: The Desolation of Smaug
writer : J.R.R. Tolkein
year : 2013
franchise : The Hobbit
```
```
title : The Hobbit: The Battle of the Five Armies
writer : J.R.R. Tolkein
year : 2012
franchise : The Hobbit
synopsis : Bilbo and Company are forced to engage in a war against an array of combatants and keep the Lonely Mountain from falling into the hands of a rising darkness.
```
```
title : Pee Wee Herman's Big Adventure
writer: Phil Hartman
year: 1985
```
```
title : Avatar
```

## Query / Find Documents

query the `movies` collection to

1. get all documents
1. get all documents with `writer` set to "Quentin Tarantino"
1. get all documents where `actors` include "Brad Pitt"
1. get all documents with `franchise` set to "The Hobbit"
1. get all movies released in the 90s
1. get all movies released before the year 2000 or after 2010

## Update Documents

1. add a synopsis to "The Hobbit: An Unexpected Journey" : "A reluctant hobbit, Bilbo Baggins, sets out to the Lonely Mountain with a spirited group of dwarves to reclaim their mountain home - and the gold within it - from the dragon Smaug."
1. add a synopsis to "The Hobbit: The Desolation of Smaug" : "The dwarves, along with Bilbo Baggins and Gandalf the Grey, continue their quest to reclaim Erebor, their homeland, from Smaug. Bilbo Baggins is in possession of a mysterious and magical ring."
1. add an actor named "Samuel L. Jackson" to the movie "Pulp Fiction"

## Text Search

1. find all movies that have a synopsis that contains the word "Bilbo"
1. find all movies that have a synopsis that contains the word "Gandalf"
1. find all movies that have a synopsis that contains the word "Bilbo" and not the word "Gandalf"
1. find all movies that have a synopsis that contains the word "dwarves" or "hobbit"
1. find all movies that have a synopsis that contains the word "gold" and "dragon"

## Delete Documents

1. delete the movie "Pee Wee Herman's Big Adventure"
1. delete the movie "Avatar"

## Relationships

### Insert the following documents into a `users` collection

```
username : SallySmith
first_name : "Sally"
last_name : "Smith"
```
```
username : JimmyHagen
full_name :
  first : "Jimmy"
  last : "Hagen"

```

### Insert the following documents into a `posts` collection

```
username : SallySmith
title : Passes out at party
body : Wakes up early and cleans house
```

```
username : SallySmith
title : Buys a House
body : Living in a new neighborhood now
```

```
username : SallySmith
title : Reports a bug in your code
body : Sends you a Pull Request
```

```
username : JimmyHagen
title : Borrows something
body : Returns it when he is done
```

```
username : JimmyHagen
title : Borrows everything
body : The end
```

```
username : JimmyHagen
title : Forks your repo on github
body : Sets to private
```


### Insert the following documents into a `comments` collection

```
username : SallySmith
comment : Hope you got a good deal!
post : [post_obj_id]
```
where [post_obj_id] is the ObjectId of the `posts` document: "Borrows something"

```
username : SallySmith
comment : What's mine is yours!
post : [post_obj_id]
```
where [post_obj_id] is the ObjectId of the `posts` document: "Borrows everything"

```
username : SallySmith
comment : Don't violate the licensing agreement!
post : [post_obj_id]
```
where [post_obj_id] is the ObjectId of the `posts` document: "Forks your repo on github

```
username : JimmyHagen
comment : It still isn't clean
post : [post_obj_id]
```
where [post_obj_id] is the ObjectId of the `posts` document: "Passes out at party"

```
username : JimmyHagen
comment : Denied your PR cause I found a hack
post : [post_obj_id]
```
where [post_obj_id] is the ObjectId of the `posts` document: "Reports a bug in your code"


## Querying related collections

1. find all users
1. find all posts
1. find all posts that was authored by "SallySmith"
1. find all posts that was authored by "JimmyHagen"
1. find all comments
1. find all comments that was authored by "SallySmith"
1. find all comments that was authored by "JimmyHagen"
1. find all comments belonging to the post "Reports a bug in your code"

There is no need to publish this to now.sh and you can provide the github url only for this project submission. [Submit your project](https://goo.gl/forms/wx8DLSus7s88lk043) 

##
#Thank you for taking the time to look at my projects,

#Also please follow my progress on youtube:
https://www.youtube.com/channel/UCXv4p-lDYeWXPlnoRFYCSUg