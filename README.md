
# distructured-lab1
MongoDB Lab Assignment 1


Q1. Create a database and switch to it
use collegeDB

Q2. Create students collection
db.createCollection("students")

Q3. Insert one document
db.students.insertOne({
  name: "Ayantika",
  rollNo: 101,
  department: "CSE",
  age: 20
})

Q4. Insert four more documents
db.students.insertMany([
  { name: "Rahul", rollNo: 102, department: "ECE", age: 21 },
  { name: "Sneha", rollNo: 103, department: "CSE", age: 19 },
  { name: "Amit", rollNo: 104, department: "ME", age: 22 },
  { name: "Priya", rollNo: 105, department: "IT", age: 20 }
])

Q5. Display all documents
db.students.find()


Q6. Display CSE students
db.students.find({ department: "CSE" })


Q7. Update age of one student
db.students.updateOne(
  { name: "Ayantika" },
  { $set: { age: 21 } }
)

Q8. Delete one document
db.students.deleteOne({ rollNo: 104 })

