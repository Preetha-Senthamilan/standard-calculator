# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.


### Step 2:
Change sttings.py file to allow request from all hosts.


### Step 3:
Use CSS for creating attractive colors


### Step 4:
Write Javascript program for implementing five different operations.


### Step 5:
Validate the HTML and CSS code

### Step 6:

Publish the website in the given URL


## PROGRAM :
'''
calc.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>SEC Demo on Calculator</title>
        <style>
        table{
            border: 10px solid maroon;
            margin-left: auto;
            margin-right: auto;
        }
        input[type="text"]{
            border: 5px solid goldenrod;
            padding: 20px 30px;
            font-size: 24px;
            font-weight: bold;
            border-radius: 2px;
        }


        input[type="button"]{
            width: 100%;
            padding: 20px 40px;
            background-color:salmon;
            border-radius: 2px;
        }
        </style>
    </head>
    <body>
        <form name="form1" onload="result.value=''">
            <h1 style="text-align: center;color:red;">Simple Calculator</h1>
        <table id="calc">
            <tr>
                <td colspan="4">
                    <input type="text" id="result">
                </td>
            </tr>
            <tr>
                <td><input type="button" value="1" onclick="result.value+='1'"></td>
                <td><input type="button" value="2" onclick="result.value+='2'"></td>
                <td><input type="button" value="3" onclick="result.value+='3'"></td>
                <td><input type="button" value="+" onclick="result.value+='+'"></td>
            </tr>
            <tr>
                <td><input type="button" value="4" onclick="result.value+='4'"></td>
                <td><input type="button" value="5" onclick="result.value+='5'"></td>
                <td><input type="button" value="6" onclick="result.value+='6'"></td>
                <td><input type="button" value="-" onclick="result.value+='-'"></td>
            </tr>
            <tr>
                <td><input type="button" value="7" onclick="result.value+='7'"></td>
                <td><input type="button" value="8" onclick="result.value+='8'"></td>
                <td><input type="button" value="9" onclick="result.value+='9'"></td>
                <td><input type="button" value="*" onclick="result.value+='*'"></td>
            </tr>
            <tr>
                <td><input type="button" value="/" onclick="result.value+='/'"></td>
                <td><input type="button" value="0" onclick="result.value+='0'"></td>
                <td><input type="button" value="." onclick="result.value+='.'"></td>
                <td><input type="button" value="=" onclick="result.value=eval(result.value)"></td>
            </tr>
            <tr>
                <td colspan="4">
                    <input type="button" value="C" id="clear" onclick="result.value=''">
                </td>
            </tr>
        </table>
        </form>
    </body>
</html>

index.js
let screen = document.getElementById('screen'); buttons = document.querySelectorAll('button'); let screenValue = ''; for (item of buttons) { item.addEventListener('click', (e) => { buttonText = e.target.innerText; console.log('Button text is ', buttonText); if (buttonText == 'X') { buttonText = '*'; screenValue += buttonText; screen.value = screenValue; } else if (buttonText == 'C') { screenValue = ""; screen.value = screenValue; } else if (buttonText == '=') { screen.value = eval(screenValue); } else { screenValue += buttonText; screen.value = screenValue; }

})
}

style.css

styles.css

.container{ text-align: center; margin-top:23px }

table{ margin: auto; }

input{ border-radius: 21px; border: 5px solid #244624; font-size:34px; height: 65px; width: 456px; }

button{ border-radius: 20px; font-size: 40px; background:lightblue; width: 102px; height: 90px; margin: 6px; }

.calculator{ border: 4px solid #13695d; background-color: blue; padding: 23px; border-radius: 53px; display: inline-block;

}

h1{ font-size: 28px; font-family: 'Courier New', Courier, monospace; }
'''


## OUTPUT:
![OUTPT](./out.png)

## HTML VALIDATOR:
![HTML VALIDATOR](./valid.png)

## Result:
The Program for designing a simple calculator using javascript is executed successfully.

