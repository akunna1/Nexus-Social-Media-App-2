## Backend structure featuring some codes

###### Goals
- Allow users signup and login
- Allow users to like posts
- Allow user post comments
- Allow users follow each other
- Allow users update profiles

###### My SQL Structure
- Nexus schema --> Create new table under Tables i.e users ---> user contains (firstname, lastname, age, location, coverPic, profilePic, id, password, email, description)
- foreign key 1: userid, reference column: id
- - foreign key 2: postid, reference column: id


