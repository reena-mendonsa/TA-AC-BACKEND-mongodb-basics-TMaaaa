writeCode

Write code to:-

- create a database named `mountains`
- a collection inside that database named `himalayas`
- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`

- insert multiple document using insertMany command
- find all documents from mountains
- find a single document using name

var multiple = [
    {
        name: 'nathula', height: '4000 mtrs'
    },
    {
        name: 'Gurudongmar ', height: '6000 mtrs'
    }
]
use mountains
db.createCollection("himalayas")
db.himalayas.insert({name: 'Dhauldhar range', height: '4000 mtrs'})
db.himalayas.insertMany(multiple)
db.himalayas.find({name:"nathula"})
db.himalayas.findOne({name:"nathula"})
