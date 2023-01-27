## Design of a Standard Calculator

## AIM:
To design a web application for a standard calculator.


## DESIGN STEPS:

## Step 1:
Create a new Django project using "django-admin startproject",get into the project terminal and use "python3 manage.py startapp" command.

## Step 2:
Define urls.py and views.py for the website .Allow host access and add the app name under installed

## Step 3:
Create a templates folder under the app folder followed by a folder under templates with the app name followed by html file named calculator.html

## Step 4:
Write HTML and CSS code in the file save it and run the app using python manage.py makemigrations and python manage.py migrate commands .Run the Server using "python3 manage.py runserver 0:80" command.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

## PROGRAM :

<div class="calculator">
        <input type="text" name="screen" id="screen">
        <table>
            <tr>
                <td><button>(</button></td>
                <td><button>)</button></td>
                <td><button>C</button></td>
                <td><button>%</button></td>
            </tr>
            <tr>
                <td><button>7</button></td>
                <td><button>8</button></td>
                <td><button>9</button></td>
                <td><button>X</button></td>
            </tr>
            <tr>
                <td><button>4</button></td>
                <td><button>5</button></td>
                <td><button>6</button></td>
                <td><button>-</button></td>
            </tr>
            <tr>
                <td><button>1</button></td>
                <td><button>2</button></td>
                <td><button>3</button></td>
                <td><button>+</button></td>
            </tr>
            <tr>
                <td><button>0</button></td>
                <td><button>.</button></td>
                <td><button>/</button></td>
                <td><button>=</button></td>
            </tr>
        </table>
    </div>
</div>
<script src="/static/JS/index.js"></script>
index.js

let screen = document.getElementById('screen'); buttons = document.querySelectorAll('button'); let screenValue = ''; for (item of buttons) { item.addEventListener('click', (e) => { buttonText = e.target.innerText; console.log('Button text is ', buttonText); if (buttonText == 'X') { buttonText = '*'; screenValue += buttonText; screen.value = screenValue; } else if (buttonText == 'C') { screenValue = ""; screen.value = screenValue; } else if (buttonText == '=') { screen.value = eval(screenValue); } else { screenValue += buttonText; screen.value = screenValue; }

})
}

style.css .container{ text-align: center; margin-top:23px }

table{ margin: auto; }

input{ border-radius: 21px; border: 5px solid #244624; font-size:34px; height: 65px; width: 456px; }

button{ border-radius: 20px; font-size: 40px; background: #978fa0; width: 102px; height: 90px; margin: 6px; }

.calculator{ border: 4px solid #13695d; background-color: #ff99f7; padding: 23px; border-radius: 53px; display: inline-block;

}

h1{ font-size: 28px; font-family: 'Courier New', Courier, monospace; }

## OUTPUT:
![image](https://user-images.githubusercontent.com/118706984/215159217-f077a580-7a82-4243-b1b5-11339cadc8f7.png)

## HTML VALIDATOR:
![image](https://user-images.githubusercontent.com/118706984/215159403-57b1438f-781c-437e-a4b1-d5ec859bf7a3.png)

## RESULT:
The program for designing calculator using javascript is sucessfully executed.



   
        
