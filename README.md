# Ex.08 Design of a Standard Calculator
## Date:06/05/2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

## calc.html:
'''


    <html>
    <head>
        <title>Calculator</title>
        <link rel="stylesheet" href="cal.css">
    </head>
    <body>
        <div id="cal">
            <input  id="display" readonly>
            <div id="key">
                <button onclick="appendToDisplay('+')" class="operator-btn">+</button>
                <button onclick="appendToDisplay('7')" >7</button>
                <button onclick="appendToDisplay('8')" >8</button>
                <button onclick="appendToDisplay('9')" >9</button>


                <button onclick="appendToDisplay('-')" class="operator-btn">-</button>
                <button onclick="appendToDisplay('4')" >4</button>
                <button onclick="appendToDisplay('5')" >5</button>
                <button onclick="appendToDisplay('6')" >6</button>


                <button onclick="appendToDisplay('')" class="operator-btn"></button>
                <button onclick="appendToDisplay('1')" >1</button>
                <button onclick="appendToDisplay('2')" >2</button>
                <button onclick="appendToDisplay('3')" >3</button>

                <button onclick="appendToDisplay('/')" class="operator-btn">/</button>
                <button onclick="appendToDisplay('0')" >0</button>
                <button onclick="appendToDisplay('.')" >.</button>
                <button onclick="calculate()" >=</button>

                <button onclick="clearDisplay()" class="operator-btn">C</button>
                
            </div>
        </div>
        <script src="cal.js"></script>
    </body>
    </html>
'''
## cal.css:
'''

     button
    {
        width: 100px;
        height: 100px;
        border-radius: 50px;
        border: none;
        background-color: hsl(0, 0%,30%);
        color: white;
        font-size: 3rem;
        font-weight: bold;
        cursor: pointer;
    }
    button:hover
    {
        background-color:orangered;
        transition: 2s;
    }
    button:active{
        background-color: red;
    }
    #key
    {
        display: grid;
        grid-template-columns: repeat(4,1fr);
        gap: 10px;
        padding: 25px;
    }
    #cal
    {
        font-family: 'Times New Roman';
        background-color: red;
        border-radius: 20px;
        max-width: 470px;
        overflow: hidden;
        color: black;
    
    
    }
    #display
    {
        width: 100%; 
        padding: 20px; 
        font-size: 5rem; 
        text-align: left; 
        border: none; 
        background-color:hsl(0, 0%,20%);
        color: rgb(121, 42, 42);
    }
    body
    {
        margin: 0; 
        display: flex; 
        justify-content: center; 
        align-items: center; 
        height: 100vh; 
        background-color:white
        ;
    }
    .operator-btn{ 
        background-color: hsl(39,100%,50%);
    }
    .operator-btn:hover{ 
        background-color: hsl(39,100%,65%);
    }
    .operator-btn:active{ 
        background-color: hsl(39,100%,75%);
    }
'''
## cal.js:
'''
    
    var display=document.getElementById("display")
    
    function appendToDisplay(input)
    {
        display.value+=input
    }
    function cleardisplay()
    {
        display.value="";
    }
    function calculate()
    {
        try{
            display.value=eval(display.value);
        }
        catch(error)
        {
            display.value="Error";
        }
    }
'''

## OUTPUT:
![WhatsApp Image 2024-05-14 at 10 55 34_d9162c84](https://github.com/vinnush147/Calc/assets/147139234/40834c0c-b54f-4b60-a88f-f5af24f1b698)

![WhatsApp Image 2024-05-14 at 10 55 46_04baeecc](https://github.com/vinnush147/Calc/assets/147139234/106cbba9-1f8a-4113-9cde-5e0fb5352479)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
