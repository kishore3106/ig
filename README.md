# Ex.08 Design of Interactive Image Gallery
## Date: 14.12.2024

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
    <head>
<style>
    body{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: radial-gradient(violet,darkblue);
    }
    h1{
        margin: 50;
        font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        font-size: 70px;
    }
    .main{
        display: flex;
        flex-wrap: wrap;
        border: 2px solid black;
        border-radius: 40px;
        background: radial-gradient(purple,darkblue);
        width: 70%;
        height: 70%;
        justify-content: center;
        align-items: center;
        margin: auto;
    }
    .n{
        
        border-radius: 20px;
        width: 27%;
        height: 30%;
        margin: auto;
        transition: transform 0.3s ease; 
        cursor: pointer;
    }
    .n:hover{
        transform: scale(1.1);
    }

    .f{
        border-radius: 40px;
        position: relative;
        top: 0%;
        bottom: 50%;
        width: 940px;
        height: 528px;
    }
    .hidden {
        display: none;
    }
</style>

    </head>
    <title>Thamizh Gallery</title>
    <body >
        <h1 align="center">THAMIZH GALLERY</h1>
        <div class="main">
            <img src="v.webp" alt="Vijay" class="n" id="ni">
            <img src="a1.webp" alt="Ajith" class="n" id="ni">
            <img src="s.webp" alt="Surya" class="n" id="ni">
            <img src="r.jpg" alt="Rajini" class="n" id="ni">
            <img src="vi.jpg" alt="Vishal" class="n" id="ni">
            <img src="vik.webp" alt="Vikram" class="n" id="ni">
        </div>
        <script type="text/javascript">
            const images = document.querySelectorAll('.n');
        
            images.forEach(function(img) {
                img.addEventListener("click", function() {
                    
                    images.forEach(function(image) {
                        if (image !== img) {
                            image.classList.add('hidden');
                        }
                    });
                    
                    img.classList.add('f');
                });
        
                img.addEventListener("dblclick", function() {
                    
                    images.forEach(function(image) {
                        image.classList.remove('hidden', 'f');
                    });
                });
            });
        </script>
    </body>
</html>
```
## OUTPUT:

![alt text](1.png)
![alt text](2.png)
![alt text](3.png)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
