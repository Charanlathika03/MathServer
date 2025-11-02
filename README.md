# Ex.05 Design a Website for Server Side Processing
## Date:02/11/25

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```html
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
   <meta charset="utf-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <title>Power of Lamp in Incandescent Bulb</title>
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <link rel="stylesheet" href="{% static 'app.css' %}">

</head>

<body>
   <div class="box">
       <h1>Power of Lamp in Incandescent Bulb</h1>

       <form method="POST">
           {% csrf_token %}
           <div>
               <span class="label">Intensity:</span>
               <input type="text" name="Intensity" value="{{ I }}" placeholder="Enter current (A)"> (in A)
           </div>

           <div>
               <span class="label">Resistance:</span>
               <input type="text" name="Resistence" value="{{ R }}" placeholder="Enter resistance (Ω)"> (in Ω)
           </div>

           <div>
               <span class="label">Power:</span>
               <input type="text" name="Power" value="{{ Power }}" readonly> W
           </div>

           <div>
               <input type="submit" value="Calculate">
           </div>
       </form>
   </div>
</body>

</html>
```
```css
body {
   font-family: 'Poppins', sans-serif;
   background: #e8f0fe;
   display: flex;
   justify-content: center;
   align-items: center;
   height: 100vh;
   margin: 0;
}

.box {
   width: 500px;
   min-height: 300px;
   font-size: 18px;
   background: #ffffff;
   border-radius: 15px;
   box-shadow: rgba(0, 0, 0, 0.2) 0px 5px 15px;
   padding: 25px;
   text-align: center;
}

h1 {
   color: #2c3e50;
   margin-bottom: 20px;
   font-family: 'Poppins', sans-serif;
}

input[type="text"] {
   width: 60%;
   padding: 8px;
   margin: 10px 0;
   border-radius: 6px;
   border: 1px solid #ccc;
   font-size: 16px;
   text-align: center;
   color: #2c3e50;
   background-color: #f9f9f9;
}

input[type="submit"] {
   margin-top: 15px;
   padding: 10px 25px;
   font-size: 16px;
   background-color: #3498db;
   border: none;
   border-radius: 8px;
   cursor: pointer;
   color: white;
   transition: 0.3s ease;
   font-weight: 500;
}

input[type="submit"]:hover {
   background-color: #2980b9;
}

.label {
   font-weight: bold;
   color: #34495e;
   font-family: 'Poppins', sans-serif;
}

```

    



## SERVER SIDE PROCESSING:
<img width="1640" height="504" alt="image" src="https://github.com/user-attachments/assets/8b997dc3-f81b-41b2-9e66-fe80043c84ff" />


## HOMEPAGE:
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/3113f743-e5e8-4ab6-a33b-1326e883315c" />


## RESULT:
The program for performing server side processing is completed successfully.
