
# distructured-lab1
MongoDB Lab Assignment 1


Q1. Create a database and switch to it
use db_AYANTIKA_004

Q2. Create students collection
db.createCollection("db_AYANTIKA_004")

Q3. Insert one document
db.db_AYANTIKA_004.insertOne({
  name: "Ayantika Gangopadhyay",
  rollNo: 004,
  department: "CSE",
  age: 20
})


Q4. Insert four more documents
db.db_AYANTIKA_004.insertMany([
  { name: "Rahul", rollNo: 102, department: "ECE", age: 21 },
  { name: "Sneha", rollNo: 103, department: "CSE", age: 19 },
  { name: "Amit", rollNo: 104, department: "ME", age: 22 },
  { name: "Priya", rollNo: 105, department: "IT", age: 20 }
])


Q5. Display all documents
db.db_AYANTIKA_004.find()



Q6. Display CSE students
db.db_AYANTIKA_004.find({ department: "CSE" })



Q7. Update age of one student
db.db_AYANTIKA_004.updateOne(
  { name: "Ayantika Gangopadhyay" },
  { $set: { age: 21 } }
)


Q8. Delete one document
db.db_AYANTIKA_004.deleteOne({ rollNo: 104 })


