# Customer-Survey-Form
Customer Survey Form is built using HTML,CSS,Javascript

<!DOCTYPE html>
<html>
<head>
  <title>Survey Form </title>
  <link rel="stylesheet" href="surveyform.css">
</head>
  <body>  
    <div class="group">
      <header class="header">
        <h1 id="title" class="text-center">Customer Survey Form</h1>
      </header>
      <form id="survey-form">
        
               <div class="form-group col-md-12">
                <table>
                  <tr>
                    <td>
                      <strong>
                        <label id="name-label" for="name">Name:</label>
                      </strong> 
                      <input class="col-xs-6" type="text" name="name" id="name"  placeholder="Enter your name" required/>
                    </td>
                   
                  <td>
                    <strong>
                     <label id="email-label"  for="email">Email:</label>
                    </strong> 
                     <input class="col-xs-6" type="email" name="email" id="email" placeholder="Enter your Email" required/>
                    </tr>   
                  </td> 
                </table>    
            </div>
      
    

        <div class="form-group"><strong>
              <label id="number-label" for="number">Age <span class="clue">(optional)</span></label><br></br></strong>
            <input type="number" name="age" id="number" min="10" max="99" class="form-control" placeholder="Age"/>
        </div>
        <div class="form-group">
          <p>Which option describes your current role?</p>
          <select id="dropdown" name="role" class="form-control" required>
            <option>Select current role</option>
            <option value="Student">Student</option>
            <option value="Working">Working</option>
            <option value="Bussiness">Bussiness</option>
            <option value="Home maker">Home maker</option>
            <option value="Other">Other</option>
          </select>
        </div>
        <div class="form-group">
          <p>Select your gender?</p>
          <label>
            <input type="radio" name="gender" value="Male" class="input-radio"/>Male</label><br></br>
            <label>
              <input type="radio" name="gender" value="Female" class="input-radio"/>Female</label><br></br>
            <label>
              <input type="radio" name="gender" value="Other" class="input-radio"/>Other</label>
        </div>
        <div class="form-group">
          <p> Would you recommend this product to others?</p>
            <label>
            <input type="radio" name="user-recommend" value="Definitely" class="input-radio"/>
               Definitely</label>
            <br></br>
            <label>
              <input type="radio" name="user-recommend" value="Maybe" class="input-radio"/>Maybe</label>
              <br></br>
            <label>
              <input type="radio" name="user-recommend" value="Not sure" class="input-radio"/>Not sure
            </label>
        </div>
        <div class="form-group">
          <p>What made you to buy this product?<span class="clue">(Check all that apply)</span></p>
          <label>
            <input name="prefer" value="Talcum powder" type="checkbox" class="input-checkbox"/>Talcum powder</label><br></br>
          <label>
            <input name="prefer" value="Perfume" type="checkbox" class="input-checkbox"/>Perfume</label><br></br>
          <label>
            <input name="prefer" value="Bathing soap" type="checkbox" class="input-checkbox"/>Bathing soap</label><br></br>
          <label>
            <input name="prefer" value="Washing soap" type="checkbox" class="input-checkbox"/>Washing soap</label><br></br>
          <label>
            <input name="prefer" value="sanitizer" type="checkbox" class="input-checkbox"/>Sanitizer
            </label><br></br>
          <label>
            <input name="prefer" value="Shampoo" type="checkbox" class="input-checkbox"/>Shampoo</label><br></br>
          <label>
            <input name="prefer" value="face-wash" type="checkbox" class="input-checkbox"/>Face-wash</label><br></br>
        </div>
        <div class="form-group">
            <p>Any comments or suggestions?</p>
                <textarea id="comments" class="input-textarea" name="comment" placeholder="Enter your comment here..."></textarea>
        </div>
        <button type="submit" id="submit" value="submit" class="submit-button">Reset</button>
        <span class="close-popup" id="closePopup"></span>

        <button type="submit"  value="submit" class="submit-button" id=" submit submission-message">Submit</button>

    </form>
</div>
</body>
</html>      
:root{
        --color-white: #f3f3f3;
        --color-fuchsia: #fbfbff;
        --color-darkblue-alpha: rgba(27,27,50,0.8);
        --color-green: #37af65;
      }
      body{
        font-family: 'Poppins',sans-serif;
        font-size: 1rem;
        line-height: 1.4;
        margin: 0;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        background-color: rgb(90, 127, 238);
      }
      h1{
        font-weight: 400;
        line-height: 1.2;
      }
      p{
        font-size: 1.125rem;
        font-weight: bold;
      }
      h1,p{
        margin-top: 0;
        margin-bottom: 0.9rem;
      }
      label{
        font-size: 1.125rem;
        margin-bottom: 0.5rem;
        padding-bottom: 10px; 
      }
      
      input,button,select,textarea{
        margin: 0;
        font-family: inherit;
        font-size: inherit;
        line-height: inherit;
      }
      button{
        border: none;
      }
      .group{
        width: 100%;
        margin: 3.125rem auto 0 auto;
      }
      @media(min-width: 576px){
        .group{
          max-width: 540px;
        }
      }
      @media(min-width: 768px){
        .group{
          max-width: 720px;
        }
      }
      .header{
        padding: 0 0.625rem;
        margin-bottom: 1.875rem;
      }
      
      .clue{
        margin-left: 0.25rem;
        font-size: 0.9rem;
        color: #e4e4e4;
      }
      .text-center{
        text-align: center;
        letter-spacing: 0.4em;
        color:whitesmoke;
        text-shadow: #37af65;
        text-shadow: 2px 2px 4px rgba(5, 238, 75, 0.5);

      }
      form{
        background: var(--color-fuchsia);
        padding: 2.5rem 0.625rem;
        border-radius: 0.25rem;
        margin-bottom: 50px;
        display: inline-block;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
      }
      @media(min-width: 480px){
        form{
          padding: 2.5rem;
        }
      }
      .form-group{
        margin: 0 auto 1.25rem auto;
        padding: 0.25rem;
        width: 700px;
        position: center;
        
      }
      .form-row {
        margin-bottom: 100px; /* Adjust the value as needed for the desired spacing */
      }
      
      .form-control{
        display: block;
        width: 100%;
        height: 2.375rem;
        padding: 0.375rem 0.75rem;
        color: #495057;
        background-color: #fff;
        border-radius: 0.25rem;
        transition: border-color 0.15s ease-in-out;
        box-shadow: 0.15s ease-in-out;
      }
      .form-control:focus{
        border-color: #0d77e9;
        outline: 0;
        box-shadow: 0 0 0 0.2rem rgba(0,123,255,0.25);
      }
      .input-radio,.input checkbox{
        display: inline-block;
        margin-right: 0.625rem;
        min-height: 1.25rem;
        min-width: 1.25rem;
      }
      .input-textarea{
        min-height: 120px;
        width: 600px;
        padding: 0.625rem;
        resize: vertical;
        border-radius: 5px;
      }
      .submit-button{
        display: block;
        width: 100px;
        padding: 0.75rem;
        background: #3c64e7;
        color: white;
        border-radius: 2px;
        cursor: pointer;
        font-weight: 600;
        float: right;
        margin-right: 7px;
      }
      
      #name,#email{
        display:block;
        width: 300px;
        margin-right: 20px;
        height: 2.375rem;
        padding: 0.375rem 0.75rem;
        color: #495057;
        background-color: #fff;
        border-radius: 0.25rem;
        box-shadow: 0.15s ease-in-out;
        transition: border-color 0.15s ease-in-out;

      }

      document.addEventListener("DOMContentLoaded", function() {
      const form = document.getElementById("survey-form");
      const submitButton = document.getElementById("submit"); // Unique ID for submit button
      const resetButton = document.getElementById("submit submission-message"); // Unique ID for reset button

      // Function to handle form submission
      function handleSubmit(event) {
        event.preventDefault(); 
        alert("Form submitted successfully!"); // Example alert
      }

      // Function to handle form reset
      function handleReset() {
        form.reset(); // Reset the form fields to their initial values
      }

      // Add event listeners
      submitButton.addEventListener("click", handleSubmit);
      resetButton.addEventListener("click", handleReset);
    });
  
