writeCode

Write command to

- List collections from a database.
show collections
- create a new collection in your country database which you created recently.
db.createCollection("delhi") 

Write code to:-

db.createCollection("temperature",{capped:true,size:3,max:3})

db.temperature.insert({"location":"bangalore"})

db.temperature.insert({"time":"night"})

db.temperature.insert({"status":"cold"})

db.temperature.insert({"response":"ok"})

create a simple collection named humidity db.createCollection("humidity")
check whether temperature collection is capped or not ? db.temperature.isCapped()
Delete humidity collection and then the entire database(weather). db.humidity.drop() db.dropDatabase()