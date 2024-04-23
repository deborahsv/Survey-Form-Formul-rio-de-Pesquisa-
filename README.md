```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Hello Kitty Form</title>
  <link rel="stylesheet" href="surveyformstyles.css">
</head>
<body>
  <fieldset>
    <div class="title1">
      <h1 id="title">Hello Kitty Form</h1>
      <p id="description">Thanks for waiting, Hello Kitty! Please rate us.</p>
    </div>
  </fieldset>
  <form id="survey-form" method="post" action='https://register-demo.freecodecamp.org'>
    <fieldset>
      <div class="form-group1">
        <label id="name-label" for="name">Name: <input placeholder="Enter your name" id="name" required name="name" type="text" required /></label>
      </div>

      <div class="form-group1">
        <label id="email-label" for="email">E-mail: <input placeholder="Enter your e-mail" id="email" required name="email"type="email" /></label>
      </div>

      <div class="form-group1">
        <label id="number-label" for="number">Age (optional): <input placeholder="Enter your age" id="number" name="age" type="number" min="10" max="120" /></label>
      </div>

      <fieldset>
        <legend>What is your favorite character of Hello Kitty and Friends Supercute Adventures?</legend>
        <label for="dropdown">
          <select id="dropdown" name="dropdown">
            <option value="">Select an option</option>
            <option value="1">Hello Kitty</option>
            <option value="2">My Melody</option>
            <option value="3">Badtz-Maru</option>
            <option value="4">Keroppi</option>
            <option value="5">Cinnamonroll</option>
            <option value="6">Kuromi</option>
            <option value="7">Chococat</option>
            <option value="8">Pochacco</option>
          </select>
        </label>
      </fieldset>

      <fieldset>
        <legend>Would you recommend Hello Kitty and Friends Supercute Adventures to a friend?</legend>
        <label for="definitely"><input id="definitely" type="radio" value="recommendation"
        name="recommendation" class="inline" checked /> Definitely</label>
        <label for="maybe"><input id="maybe" type="radio" value="recommendation"
        name="recommendation" class="inline" /> Maybe</label>
        <label for="not-sure"><input id="not-sure" type="radio" value="recommendation"
        name="recommendation" class="inline"  /> Not sure</label>
      </fieldset>

      <fieldset>
        <legend>What do you like most about this series? (Check all that apply)</legend>
        <label for="characters"><input id="characters" type="checkbox" value="1" name="improved" class="inline" /> Characters</label>
        <label for="characters"><input id="characters" type="checkbox" value="2" name="improved" class="inline" /> Friendship</label>
        <label for="characters"><input id="characters" type="checkbox" value="3" name="improved" class="inline" /> The adventures</label>
        <label for="characters"><input id="characters" type="checkbox" value="4" name="improved" class="inline" /> The aesthetics</label>
      </fieldset>

      <fieldset>
        <legend>Any comments or suggestions?</legend>
        <label for="comments">
          <textarea id="comments" name="comments" rows="4" cols="30" placeholder="Your comment here :)"></textarea>
        </label>
      </fieldset>
      <input type="submit" id="submit" value="Submit" />
    </fieldset>
  </form>
</body>
</html>

```css

body {
background-image: url(https://i.pinimg.com/564x/e5/ca/7c/e5ca7c1a77ac20f2e5ac2806559c1112.jpg);
    background-size: cover; 
    background-position: center; 
}

.form-group1 {
display: inline-block;
width: 400px; 
height: 35px;
}

input[type="text"],
input[type="email"],
input[type="number"], select, textarea {
width: 250px;
height: 25px;
padding: auto;
box-sizing: border-box;
}

label {
font-weight: bold;
}


input[type="maybe"]{
  margin: 10px 10px 10px 0;
  width: 100%;
  height: 30px;
}

.textarea {
  margin: 0;
  width: 10%;
  height: 30px;
}

.select {
  margin: 10px 10px 10px 0;
  width: 100%;
  height: 30px;
}

h1, p {             
margin: 20px 10px;  
text-align: center;
box-sizing: border-box;
}

.title1 {
 background-color: rgb(202, 10, 46);
    padding: 0; 
    margin: 0; 
    color: white;
    border: 1px solid black;
    letter-spacing: 5px; 
    font-size: 16px; 
    text-shadow: -1px -1px 0 black, 1px -1px 0 black, -1px 1px 0 black, 1px 1px 0 black; 
    outline: none; 
}
label {
    font-weight: bold;
    border: none; /* Adiciona esta linha para remover a borda automática do label */
}
.bordered-text {
    border: 1px solid black;
    padding: 5px;
}


form {
  margin-top: 60px; 
  margin-left: auto; 
  margin-right: auto; 
  width: 80%; 
  background-color: rgb(202, 10, 46);
  box-sizing: border-box;
  padding: 20px;
  max-width: 500px;
  border: 2px solid black;
  color: white;
  text-shadow: -1px -1px 0 black, 1px -1px 0 black, -1px 1px 0 black, 1px 1px 0 black; 
}

input[type="submit"] {
    background-color: rgb(10, 33, 185); 
    color: white; 
    padding: 5px 20px; 
    font-size: 16px; 
    display: block; 
    margin: 10px auto; 
}
