
import axios from 'axios';
import { useEffect, useState } from 'react';
import './App.css';



function App() {

  axios.get('https://')
.then(res => console.log(res.data)) 
.catch(err => console.log(err))

  const postdata = async () => {
    axios.post('https:com/users', {
    address : '56789065e',
    name: "Anon",
    job: "web3 Developer",
   })
    .then(res => console.log(res)) 
    .catch(err => console.log(err))
  }

  const putdata = async () => {
      axios.put('https://' {
      name: "Anon",
      job: "Web Developer",
  })

  const deldata = async () => {
    axios.delete('https')
  .then(res => console.log(res)) 
  .catch(err => console.log(err))
  }
  
  return (
    <div className="App">
      <header className="App-header">
        <button onClick={putdata}>post data</button>
      </header>
    </div>
  );
}

export default App;
