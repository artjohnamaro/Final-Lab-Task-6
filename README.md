# Finals Task 6. MOngoDBCRUD

This portfolio shows about my knowledge in MongoDB CRUD operations, which stands for Create, Read, Update, and Delete. These are the basic operations used to manage data in a MongoDB database. Through this section, I demonstrate how to perform each of these operations using MongoDB’s methods like insertOne(), find(), updateOne(), and deleteOne(). I also showcase examples using MongoDB with Node.js and explain how data is stored as documents in collections. This reflects my understanding of how MongoDB works in real-world applications, especially for backend development.

## Step-By-Step Process
1. Create a Database

- Start by creating or switching to a specific database.

- The selected database becomes the active workspace for all upcoming operations.

2. Insert Documents

- Within the database, a collection is created.

- Multiple documents are inserted into the collection, each containing structured data fields such as name, age, or address.

3. FIND Documents

- Display all documents stored in the collection.

- Use filters to find specific documents based on certain values like name or ID.

4. UPDATE Documents

- Locate the document that needs modification using a condition (e.g., name or ID).

- Specify the field(s) to be changed and apply the update.

- Confirm the update by checking the document again.

5. SEARCH Documents

- Use specific criteria to locate documents that match particular conditions (e.g., age greater than a value or status equals a specific string).

- Review the matched results for accuracy.

6. DELETE Documents
    
- Identify the document(s) to be removed using a condition.

- Remove the document(s) from the collection.

- Verify deletion by checking the collection contents.

7. RELATIONSHIP

- Insert the following documents into a `users` collection

- Insert the following documents into a `posts` collection

- Insert the following documents into a `comments` collection

8. QUERYING related collections 

## OUTPUTS
1. Create Database

![Image](https://github.com/user-attachments/assets/e23d4aa0-7ba9-4afc-83a3-313fa22a7651)

2. Insert Document

![Image](https://github.com/user-attachments/assets/3a326750-10c6-4f63-81e4-86cb2b8bc0d7)   

3. Query/ Find Document
- Get all documents

![Image](https://github.com/user-attachments/assets/9e2701dd-b9ca-46a1-bba8-bf782d53424c)

- Get all documents with `writer` set to &quot;Quentin Tarantino&quot;

![Image](https://github.com/user-attachments/assets/ce4ac565-4745-4190-a584-11190d93d299)


- Get all documents where `actors` include &quot;Brad Pitt&quot;

![Image](https://github.com/user-attachments/assets/75341b45-d320-485e-81c8-b817c4776dfd)


- Get all documents with `franchise` set to &quot;The Hobbit&quot;

![Image](https://github.com/user-attachments/assets/d94833a3-0c58-44df-8d5d-a1adc5829a30)

- Get all movies released in the 90s

![Image](https://github.com/user-attachments/assets/d6dbbfaa-d742-43da-9372-ea61cfd31a3e)


- Get all movies released before the year 2000 or after 2010

![Image](https://github.com/user-attachments/assets/d3175a67-713b-4a5a-b306-d655516dfd02)


4. Update Documents

- ![Image](https://github.com/user-attachments/assets/2fc859ae-a387-42b9-9888-34955c508b11)

- ![Image](https://github.com/user-attachments/assets/60c67fa9-9770-4ad3-bd35-33272b76a3c0)

- ![Image](https://github.com/user-attachments/assets/67f56b9b-306d-4f0e-bd2c-2094dc1b2f75)

5. Text Search

- Find all movies that have a synopsis that contains the word &quot;Bilbo&quot;

![Image](https://github.com/user-attachments/assets/5520df72-fc62-4e91-a6ab-d381a86e009b)

- Find all movies that have a synopsis that contains the word &quot;Gandalf&quot;

![Image](https://github.com/user-attachments/assets/f921f7a0-a0c6-4ac9-b59b-f4e35d4923f1)

- Find all movies that have a synopsis that contains the word &quot;Bilbo&quot; and not the word &quot;Gandalf&quot;

![Image](https://github.com/user-attachments/assets/d6430403-0517-4370-8b0c-648e3f597a03)

- Find all movies that have a synopsis that contains the word &quot;dwarves&quot; or &quot;hobbit&quot;

![Image](https://github.com/user-attachments/assets/cd89e61c-f49e-45b9-9a0a-66b2a2236453)

- Find all movies that have a synopsis that contains the word &quot;gold&quot; and &quot;dragon&quot;

![Image](https://github.com/user-attachments/assets/286e7285-0c34-4d25-b278-ffa624d3a58b)

6. Delete

- Delete the movie &quot;Pee Wee Herman&#39;s Big Adventure&quot;

![Image](https://github.com/user-attachments/assets/7bdef650-614e-45ea-9b45-7de27ffb9065)

- Delete the movie &quot;Avatar&quot;

![Image](https://github.com/user-attachments/assets/3424ecb6-f291-4688-8ff4-357a696c3f44)

7. Relationship

- Insert the following documents into a `users` collection

  1. db.users.insert({_id:1,username:"GoodGuyGreg", first_name:"Good Guy", last_name:"Greg"})
  
  -  ![Image](https://github.com/user-attachments/assets/aee9adf8-382b-48bf-b469-5135fd83ad56)
 
  2. db.users.insert({_id:2, username:"ScumbagSteve", fullname:{first: "Scumbag", last:"Steve"}})
  
  -    ![Image](https://github.com/user-attachments/assets/81ca51f4-fc32-417b-8f6a-36fb168d346c)
 
- Insert the following documents into a `posts` collection

  1. db.posts.insert({username:"GoodGuyGreg", title:"Passes out at Party", body:"Raises your credit score"})
     
  - ![Image](https://github.com/user-attachments/assets/69bc4911-0136-41b4-94e3-d5ac3d88381c)
 
  2. db.posts.insert({ username:"GoodGuyGreg", title:"Steals your identity", body:"Raises your credit score"})

  - ![Image](https://github.com/user-attachments/assets/dc3e220e-fab8-46dc-9f88-a75aac36bffe)
 
  3. db.posts.insert({username:"GoodGuyGreg", title:"Reports a bug in your code", body:"Sends you a pull request"})
 
  - ![Image](https://github.com/user-attachments/assets/2218f9d2-4158-4548-90e2-bad3a4a17d66)
 
  4. db.posts.insert({ username:"ScumbagSteve", title:"Borrows something", body:"Sells it"})
 
  - ![Image](https://github.com/user-attachments/assets/a5feec42-63c0-4e70-9a55-75148cc26100)
 
  5. db.posts.insert({ username:"ScumbagSteve", title:"Borrows everything", body:"The end"})
 
  - ![Image](https://github.com/user-attachments/assets/3b85d743-e792-4f3b-a8dd-c2998d1fb906)
 
  6. db.posts.insert({username:"ScumbagSteve", title:"Forks your repo on github", body:"Sets to private"})
 
  - ![Image](https://github.com/user-attachments/assets/8eadf8d3-bd4e-4604-b2c9-b7218ca77573)

- Insert the following documents into a `comments` collection
  
  1. db.comments.insert({ username:"GoodGuyGreg", comment:"Hope you got a good deal!", post:ObjectId("5ca0b7e96435f98b5901f463")})
     
  - ![Image](https://github.com/user-attachments/assets/aecdcf58-3550-4093-a4c9-c7f4ffe5cd32)
 
  2. where [post_obj_id] is the ObjectId of the `posts` document: "Borrows everything"
db.comments.insert({username:"GoodGuyGreg", comment:"What's mine is yours!", post:ObjectId("5ca0b9706435f98b5901f46a")})

  - ![Image](https://github.com/user-attachments/assets/2e515d97-0b7a-4875-ad1d-7e7536cc9e09)
 
  3. where [post_obj_id] is the ObjectId of the `posts` document: "Forks your repo on github
db.comments.insert({username:"GoodGuyGreg", comment:"Don't violate the licensing agreement!", post:ObjectId("5ca0b8766435f98b5901f467")})

  - ![Image](https://github.com/user-attachments/assets/0b0e3121-ba92-4136-8c0f-619d9a76ce4d)
 
  4. where [post_obj_id] is the ObjectId of the `posts` document: "Passes out at party"
db.comments.insert({username:"ScumbagSteve", comment:"It still isn't clean", post:ObjectId("5ca0b8546435f98b5901f466")})

  - ![Image](https://github.com/user-attachments/assets/f6128a89-b166-410e-af0f-e7a6b14c5ad0)
 
  5. where [post_obj_id] is the ObjectId of the `posts` document: "Reports a bug in your code" db.comments.insert({username:"ScumbagSteve", comment:"Denied your PR cause I found a hack", post:ObjectId("5ca0b9256435f98b5901f469")})

8. QUERYING related collections

   - Find all users
     
     ![Image](https://github.com/user-attachments/assets/5251afd7-1e34-4fab-85c2-0666e3dfb657)

   - Find all posts
     
     ![Image](https://github.com/user-attachments/assets/406fda81-fd90-4e85-a599-a9ba4c316628)

   - Find all posts that was authored by "GoodGuyGreg"
     
     ![Image](https://github.com/user-attachments/assets/1bcde38e-ba3a-4423-b95e-3e19b3e588a7)

   - Find all posts that was authored by "ScumbagSteve"
     
     ![Image](https://github.com/user-attachments/assets/1601df09-2a3b-4c19-b734-9fd9e8519580)

   - Find all comments
  
     ![Image](https://github.com/user-attachments/assets/b417142e-472a-4ed4-a1db-35ced339777c)

   - Find all comments that was authored by "GoodGuyGreg"
  
     ![Image](https://github.com/user-attachments/assets/d59170e5-1e1d-4bc7-93cd-b98439d031ac)

   - Find all comments that was authored by "ScumbagSteve"
  
     ![Image](https://github.com/user-attachments/assets/eea52da1-97ca-446b-b84f-15ca395031dc)

   - Find all comments belonging to the post "Reports a bug in your code"




 


  
