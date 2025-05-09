# Ex.08 Design of Interactive Image Gallery
## Date:9.05.2025

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
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Image Gallery</title>
</head>

<body>
    <!-- Heading Name -->
    <div class="heading">
        <h1>Image Gallery</h1>
    </div>

    <!-- Image Gallery section all images in one div -->
    <div class="gallery">
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240311163321/Types-of-Wastes-(Banner).webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240311163321/Types-of-Wastes-(Banner).webp')"
                alt="Image 1">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240311125007/Invertebrates-(Banner).webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240311125007/Invertebrates-(Banner).webp')"
                alt="Image 2">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240311120816/GBlog-banner.webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240311120816/GBlog-banner.webp')"
                alt="Image 3">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240308123700/Layers-of-Atmosphere-Banner-02.webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240308123700/Layers-of-Atmosphere-Banner-02.webp')"
                alt="Image 4">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240307180031/List-of-Rocket-Launching-Stations-in-India---banner.webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240307180031/List-of-Rocket-Launching-Stations-in-India---banner.webp')"
                alt="Image 5">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240215134226/Russia-Banner-copy-2.webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240215134226/Russia-Banner-copy-2.webp')"
                alt="Image 6">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240226155245/girl-dog-names-banner.webp"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240226155245/girl-dog-names-banner.webp')"
                alt="Image 7">
        </div>
        <div class="gallery-item">
            <img src=
"https://media.geeksforgeeks.org/wp-content/uploads/20240215151423/Types-of-Microscope-(Banner).png"
                onclick="openModal(
'https://media.geeksforgeeks.org/wp-content/uploads/20240215151423/Types-of-Microscope-(Banner).png')"
                alt="Image 8">
        </div>
    </div>

    <!-- Modal for Image Display -->
    <div id="myModal" class="modal">
        <span class="close" onclick="closeModal()">&times;</span>
        <img class="modal-content" id="modalImage">
    </div>

    <!-- JavaScript for Modal -->
    <script>
        function openModal(src) {
            document.getElementById("modalImage").src = src;
            document.getElementById("myModal").style.display = "block";
        }

        function closeModal() {
            document.getElementById("myModal").style.display = "none";
        }
    </script>
</body>

</html>


.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 10px;
  padding: 20px;
}

.gallery-item {
  overflow: hidden;
}

.gallery-item img {
  width: 100%;
  height: auto;
  display: block;
}

.modal {
  display: none;
  position: fixed;
  z-index: 1;
  padding-top: 100px;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0, 0, 0, 0.9);
}

.modal-content {
  margin: auto;
  display: block;
  max-width: 90%;
  max-height: 90%;
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}
function openModal(imageSrc) {
  let modal = document.getElementById("myModal");
  let modalImg = document.getElementById("modalImage");
  modal.style.display = "block";
  modalImg.src = imageSrc;
}

function closeModal() {
  let modal = document.getElementById("myModal");
  modal.style.display = "none";
}

```
## OUTPUT:
![Screenshot 2025-05-09 142526](https://github.com/user-attachments/assets/6d86617e-dc41-4862-9890-e0843bc01568)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
