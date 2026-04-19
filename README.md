<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>CE Campus Admin Dashboard</title>

<style>
body{
font-family:Arial;
margin:0;
background:#141e30;
color:white;
}

.header{
background:#00c9ff;
padding:15px;
text-align:center;
font-size:22px;
font-weight:bold;
color:black;
}

.container{
padding:20px;
}

input{
width:100%;
padding:10px;
margin-bottom:15px;
border-radius:5px;
border:none;
}

table{
width:100%;
border-collapse:collapse;
background:white;
color:black;
}

th,td{
padding:10px;
border:1px solid #ccc;
text-align:center;
}

th{
background:#00c9ff;
}

button{
padding:5px 10px;
border:none;
border-radius:5px;
cursor:pointer;
}

.delete{
background:red;
color:white;
}

.print{
background:green;
color:white;
margin-bottom:10px;
}
</style>
</head>

<body>

<div class="header">🎓 CE Campus Admin Dashboard</div>

<div class="container">

<input type="text" id="search" placeholder="Search student...">

<button class="print" onclick="window.print()">🖨️ Print List</button>

<table id="table">
<thead>
<tr>
<th>Name</th>
<th>Father</th>
<th>Mobile</th>
<th>Class</th>
<th>Stream</th>
<th>Subject</th>
<th>Action</th>
</tr>
</thead>
<tbody></tbody>
</table>

</div>

<script>

let students = JSON.parse(localStorage.getItem("students") || "[]");

function loadTable(data){
let tbody=document.querySelector("tbody");
tbody.innerHTML="";

data.forEach((s,i)=>{
let row=`
<tr>
<td>${s.Name}</td>
<td>${s.Father}</td>
<td>${s.Mobile}</td>
<td>${s.Class}</td>
<td>${s.Stream}</td>
<td>${s.Subject}</td>
<td><button class="delete" onclick="deleteStudent(${i})">Delete</button></td>
</tr>`;
tbody.innerHTML+=row;
});
}

loadTable(students);

/* SEARCH */
document.getElementById("search").addEventListener("input",function(){
let val=this.value.toLowerCase();

let filtered=students.filter(s=>
s.Name.toLowerCase().includes(val) ||
s.Mobile.includes(val)
);

loadTable(filtered);
});

/* DELETE */
function deleteStudent(index){
if(confirm("Delete student?")){
students.splice(index,1);
localStorage.setItem("students",JSON.stringify(students));
loadTable(students);
}
}

</script>

</body>
</html>
