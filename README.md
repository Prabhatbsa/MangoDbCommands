# MangoDbCommands
Main Commands

    1) Show Dbs
    2) Use <db name>
    3) db.createCollection("students")
    4) Db.dropDatabase() //Deletes an database.
    5) db.students.insertOne({name:"Prabhat", age:30, gpa:3.5})
    6) Db.students.insertMany([{name:"Prabhat", age:30, gpa:3.5}, {name:"Patrick", age:35, gpa:1.5}, {name:"Sandy", age:38, gpa:4.5}])
    7) db.students.find() // Similar to select * from blah blah
    8) Sorting
    db.students.find().sort({name:-1}) //1 for Ascending ,-1 for descending
    9) Limit // Fetch number of records
    db.students.find().sort({name:-1}).limit(1) //This will fetch the first record from records which are sorted by name in descending order.
    10) db.students.find({query}, {projection}) // e.g 
    
    Fetching with given parameters but with fetch only names as specified in the projection parameter.
    
    
    Make Id as false. It will Not bring the Object Id 
    
    Update
    Db.students.updateOne(filter,update)
    Using Set operator
    
    
    Using UnSet Operator
    
    
    UpdateMany
    
    // This will Update Many Documents where fullTime field don’t exist and bring field and set it as true.
    
    DELETE
    Use DeleteOne() or DeleteMany() operators
    
    
