# Ex.08 Design of Interactive Image Gallery
# Date:13.11.2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <body>
        <header>
            <h1><font color="orange">IMAGE GALLERY</font></h1>
        </header>
        <header>
            <h2><font color="aqua">7 WONDERS</font></h2>
        </header>
    </body>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
             background-image: url("background.jpg");
            background-size:cover;
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 300px;
            height: 200px;
            border: 2px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="tajmahal.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="chinawall.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="china.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="colosseum.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="cristo.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="Chichen Itza.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="Machu Picchu.jpg" alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>
```
# OUTPUT:
![Screenshot (64)](https://github.com/user-attachments/assets/e03ecb06-8813-4cbb-b3b3-aaf6c58c06aa)
![Screenshot (65)](https://github.com/user-attachments/assets/32a63716-1400-42c7-8bdc-8f8c1000f18c)
![Screenshot (66)](https://github.com/user-attachments/assets/0b715d1c-71fd-4050-affe-352938220fed)
![Screenshot (67)](https://github.com/user-attachments/assets/9e486c49-1d2e-4756-8311-8621c9a68bfb)
![Screenshot (68)](https://github.com/user-attachments/assets/293eae8e-98df-4257-83f2-e62a35e419e7)
![Screenshot (69)](https://github.com/user-attachments/assets/96074ae7-040e-4299-ace9-0c25cad1320a)
![Screenshot (70)](https://github.com/user-attachments/assets/243bbb67-9478-4099-831f-df873e543e79)
![Screenshot (71)](https://github.com/user-attachments/assets/fd764c34-d180-464c-8965-c120e821b3d4)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
