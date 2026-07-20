<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>User Data Collection</title>
</head>
<body>
   <h1> User Information</h1>
   <div id="userData"></div> 
   <script src="app.js"></script>
</body>
</html>



// Task 1 : Collect user Information
let userName = prompt("Enter your name");
let userAge = prompt("Enter your age");
let userCity = prompt("Enter your city");
let userProfession = prompt("Enter your profession");
let userEmail = prompt("Enter your email");
let userPhonenumber = prompt("Enter your Phone number");
alert("Welcome, " + userName + "!");
console.log("Name:", userName);
console.log("Age:", userAge);
console.log("City:", userCity);
console.log("Profession:", userProfession);
console.log("Email:", userEmail);
console.log("Phone Number:", userPhonenumber);

//Task 2: Store Data
let user = {
    fullName: userName,
    age: userAge,
    city: userCity,
    profession: userProfession,
    email: userEmail,
    phone: userPhonenumber
};
let users = [];
let savedUsers = localStorage.getItem("users");
if (savedUsers) {
    users = JSON.parse(savedUsers);
}
users.push(user);
localStorage.setItem("users", JSON.stringify(users));
let displayUsers = JSON.parse(localStorage.getItem("users"));

// Task 3 = Display Data on the Web Page
let userData = document.getElementById("userData");
displayUsers.forEach(function(user) {
    userData.innerHTML += `
        <div class="card">
            <h3>${user.fullName}</h3>
            <p><strong>Age:</strong> ${user.age}</p>
            <p><strong>City:</strong> ${user.city}</p>
            <p><strong>Profession:</strong> ${user.profession}</p>
            <p><strong>Email:</strong> ${user.email}</p>
            <p><strong>Phone:</strong> ${user.phone}</p>
        </div>
    `;
});
