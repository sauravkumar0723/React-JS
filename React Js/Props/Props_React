What are Props?
Props (short for "properties") are like function parameters. They allow you to pass data from one component to another (typically from parent to child).



User.jsx
function User(props) {
  return (
    <div>
      <h1>{props.name}</h1>
    </div>
  );
}

export default User;


App.jsx

import User from "./User";

function App() {
  return (
    <div>
      <h1>Props in React JS</h1>
      <User name="Anil Sidhu" />
    </div>
  );
}

export default App;


You can also use destructuring in the User component:

function User({ name }) {
  return <h1>{name}</h1>;
}


Passing Multiple Props
<User name="Anil Sidhu" age={29} email="anil@test.com" />


function User({ name, age, email }) {
  return (
    <div>
      <h2>{name}</h2>
      <h2>{age}</h2>
      <h2>{email}</h2>
    </div>
  );
}


Pass Props as Variables
let name = "Anil";
let age = 29;
let email = "anil@test.com";

<User name={name} age={age} email={email} />


Pass Props as Objects
let user = { name: "Anil", age: 29, email: "anil@test.com" };

<User user={user} />


function User({ user }) {
  return (
    <div>
      <h2>{user.name}</h2>
      <h2>{user.age}</h2>
      <h2>{user.email}</h2>
    </div>
  );
}


Pass Array Props
let colleges = ["IIT", "DU", "NIT"];
<College name={colleges[0]} />
<College name={colleges[1]} />
<College name={colleges[2]} />


function College({ name }) {
  return <h1>{name}</h1>;
}


Pass Props on Click (Dynamic Props)
import { useState } from "react";
import Student from "./Student";

function App() {
  const [student, setStudent] = useState();

  return (
    <div>
      <h1>Props in React JS</h1>
      {student && <Student name={student} />}
      <button onClick={() => setStudent("Bhaskar")}>Update Student</button>
    </div>
  );
}


function Student({ name }) {
  return <h1>Student Name: {name}</h1>;
}
