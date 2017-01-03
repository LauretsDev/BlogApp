# Blog App

A blog website where dog owners can post a photo and information about their dog. This application uses Node.js, Express, MongoDB, RESTful API, and Semantic UI.

**Routing chart**

| Name     | Path          | HTTP Verb  | Purpose                                          | Mongoose Method         |
| -------- | :------:      | :--------: | :-----------:                                    | :-------------------:   |
| Index    | /dogs         | GET        | List all dogs                                    | Dog.find()              |
| New      | /dogs/new     | GET        | Show new dog form                                | N/A                     |
| Create   | /dogs         | POST       | Create a new dog, then redirect somewhere        | Dog.create()            |
| Show     | /dogs/:id     | GET        | Show info about one specific dog                 | Dog.findById()          |
| Edit     | /dogs/:id/edit| GET        | Show edit form for one dog                       | Dog.findById()          |
| Update   | /dogs/:id     | PUT        | Update a particular dog, then redirect somewhere | Dog.findByIdAndUpdate() |
| Destroy  | /dogs/:id     | DELETE     | Delete a particular dog, then redirect somewhere | Dog.findByIdAndRemove() |
