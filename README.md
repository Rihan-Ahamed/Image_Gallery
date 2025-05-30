# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Image Gallery</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: url('https://i.pinimg.com/736x/d7/6b/c3/d76bc39b92ecdb9ad5c1c7227b5695c4.jpg') no-repeat center center/cover;
      height: 100vh;
      overflow: auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      color: white;
      position: relative;
      padding-top: 50px;
    }

    h1 {
      font-size: 1.8em;
      text-shadow: 2px 2px 4px black;
      font-weight: normal;
      margin-bottom: 30px;
    }

    .gallery-container {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
      align-items: center;
      padding: 20px;
      max-width: 95%;
    }

    .gallery-container img {
      width: 200px;
      height: auto;
      object-fit: cover;
      border-radius: 10px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .gallery-container img:hover {
      transform: scale(1.05);
    }

    #modal {
      display: none;
      position: fixed;
      z-index: 1000;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.8);
    }

    #modal img {
      margin: auto;
      display: block;
      max-width: 80%;
      max-height: 80%;
      position: relative;
      top: 10%;
    }

    #close {
      position: absolute;
      top: 20px;
      right: 30px;
      color: white;
      font-size: 2em;
      cursor: pointer;
    }

    footer {
      position: relative;
      bottom: 10px;
      right: 10px;
      color: #ddd;
      font-size: 1em;
      margin-top: 20px;
    }

    footer a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }

    footer a:hover {
      color: #00c3ff;
    }
  </style>
</head>
<body>

  <h1>Image Gallery</h1>

  <div class="gallery-container">
    
    <img src="muhammad ali wallpaper.jpeg" alt="Image 2" onclick="openModal(this)">
    <img src="83343be1-ff67-4b73-8858-cc69bf46fcf7.jpeg" alt="Image 8" onclick="openModal(this)">
    <img src="Reaching speeds of up to 242 mph, the Peregrine….jpeg" alt="Image 3" onclick="openModal(this)">
     <img src="Instagram.jpeg" alt="Image 4" onclick="openModal(this)">
    <img src="download (5).jpeg" alt="Image 6" onclick="openModal(this)">
    <img src="adddbdee-42fe-40f0-b41d-3156c51aecc7.jpeg" alt="Image 7" onclick="openModal(this)">
    <img src="islam_khabib.jpg" alt="Image 1" onclick="openModal(this)">
    <img src="FREE FREE PALESTINE.jpeg" alt="Image 5" onclick="openModal(this)">
    
  </div>

  <div id="modal">
    <span id="close" onclick="closeModal()">&#10006;</span>
    <img id="modalImage" src="" alt="Expanded View">
  </div>

  <footer>
    <p>Designed by: Rihan Ahamed.S (212224040276)</p>
  </footer>

  <script>
    function openModal(image) {
      const modal = document.getElementById("modal");
      const modalImage = document.getElementById("modalImage");
      modal.style.display = "block";
      modalImage.src = image.src;
    }

    function closeModal() {
      document.getElementById("modal").style.display = "none";
    }
  </script>

</body>
</html>

~~~

## OUTPUT

![alt text](<Screenshot 2025-05-15 221810.png>)
![alt text](<Screenshot 2025-05-15 221827.png>)
![alt text](<Screenshot 2025-05-15 221916.png>)
![alt text](<Screenshot 2025-05-15 221903.png>)
![alt text](<Screenshot 2025-05-15 221930.png>)
![alt text](<Screenshot 2025-05-15 221843.png>)
## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
