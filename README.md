<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OOCSS Page </title>
    <link rel="stylesheet" href="styles.css"> <!-- Link to the external CSS file -->
</head>
<body>
    <header class="header">
        <h1 class="header__title">OOCSS Sample Page </h1>
    </header>
    <main class="main">
        <section class="card">
            <div class="card__content">
                <h2 class="card__title">Card Title</h2>
                <p class="card__description">This is a description of the card content.</p>
                <a href="#" class="button button--primary">Read More</a>
                <a href="#" class="button button--secondary">Share</a>
            </div>
        </section>
        <section class="card">
            <div class="card__content">
                <h2 class="card__title">Another Card Title</h2>
                <p class="card__description">This is another description of a card content.</p>
                <a href="#" class="button button--primary">Read More</a>
                <a href="#" class="button button--secondary">Share</a>
            </div>
        </section>
    </main>
    <footer class="footer">
        <p>© 2024 OOCSS Page | All Rights Reserved</p>
    </footer>
</body>
</html>




/* styles.css */
/* Basic reset for margins and padding */
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}
.header {
    background-color: #007bff; /* Header background color */
    color: white; /* Header text color */
    text-align: center; /* Center header text */
    padding: 20px; /* Padding around header */
}
.header__title {
    margin: 0; /* Remove default margin */
}
.main {
    display: flex; /* Flexbox for layout */
    flex-direction: column; /* Stack cards vertically */
    align-items: center; /* Center align items */
    padding: 20px; /* Padding around main content */
}
.card {
    background-color: #ffffff; /* Card background color */
    border: 1px solid #ddd; /* Card border */
    border-radius: 8px; /* Rounded corners */
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Subtle shadow */
    width: 300px; /* Fixed width for the card */
    margin: 20px; /* Margin around each card */
    overflow: hidden; /* Prevent content overflow */
}
.card__image {
    width: 100%; /* Full width for the image */
    height: auto; /* Maintain aspect ratio */
}
.card__content {
    padding: 15px; /* Padding inside the card content */
}
.card__title {
    font-size: 20px; /* Font size for the card title */
    color: #333; /* Dark grey color for the title */
    margin: 0; /* Remove default margin */
}
.card__description {
    font-size: 14px; /* Font size for the description */
    color: #555; /* Grey color for the description */
    margin: 10px 0; /* Margin above and below the description */
}
.button {
    display: inline-block; /* Make buttons inline */
    padding: 10px 15px; /* Padding for the buttons */
    margin-right: 10px; /* Space between buttons */
    border: none; /* Remove default border */
    border-radius: 5px; /* Rounded corners for buttons */
    text-decoration: none; /* Remove underline from links */
    color: white; /* White text color */
}
.button--primary {
    background-color: #007bff; /* Blue background for primary button */
}
.button--secondary {
    background-color: #6c757d; /* Grey background for secondary button */
}
.footer {
    text-align: center; /* Centered text */
    padding: 10px; /* Padding around footer */
    background-color: #f1f1f1; /* Light background for footer */
    color: #333; /* Dark text color */
    position: relative; /* Positioning for footer */
    bottom: 0; /* Aligns footer at the bottom */
    width: 100%} /* Full width for footer */