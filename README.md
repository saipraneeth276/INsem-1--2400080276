import React from 'react';


const Welcome = ({ name }) => {
  return <h1>Welcome, {name}!</h1>;
};


const App = () => {
  const students = ['Deepak', 'Maria', 'John'];

  return (
    <div>
      {students.map((student) => (
        <Welcome key={student} name={student} />
      ))}
    </div>
  );
};

export default App;
