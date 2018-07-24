# GifTastic
GIFTASTIC

Tools: HTML5, CSS3, Bootstrap4, JavaScript, jQuery, AJAX technique, GIPHY API

Summary: The application loads a set of feeling/emotion words. Clicking one will load a random set of 10 still GIPHY images. Clicking on the image will active it; clicking again will stop it. User also can enter their own emotion in the search box, and it will add that word to the list as a button and, when clicked, will populate an additional 10 GIPHY on the page.

Problem: The task was to use the GIPHY API in combination with the AJAX technique to create a dynamic application that will populate a set of 10 GIPHY static images at a time. Then when another button is clicked simply add (rather than overwrite) the next 10 GIPHY images. Create an input box where the user can add their own word to the list and, when clicked, adds GIPHY to the page just like the original buttons.

Solution: Create a dynamic web page that populates gifs from GIPHY using the AJAX technique with the GIPHY API, and utilize JavaScript and jQuery to update the HTML. This was achieved by capitalizing on the power of AJAX to update the web page without a hard refresh, and pull data from the API after the page had loaded so that previously pulled images would remain on the page while new images were added.

My Technical Approach: First I had to create a GIPHY account and acquire an API key. I created an HTML mockup and added some basic CSS styling. I then created an array of feeling words and then a for loop to dynamically create buttons for each of the words. I also included a small piece of jQuery code to clear any duplicated buttons. I also added a class to the creation of new buttons so that when the user input their own word, the button generated will be styled and appended to the button list just like the original buttons. I then used AJAX to queryURL and get the images and pull them into the display area divs on the page. I added some additional code so that when the images were pulled, the image rating and the image title were appended to the gif. Because I didn’t like the styling of the ratings being pulled back, I added .toUpperCase and some classes to the ratings, title and image borders. I also set up a toggle to change the data-state of the images from still to animate and back again. This was done through an if/else nested within an on click function using jQuery. Finally I added a user input field and created a push so the new feeling word would get appended to the list of buttons. I set the number of images to be returned to 10, and as a new set of 10 images were called I prepended them so they would populate at the top of the page, while also not overwriting any images below them. I then had to make some additional adjustments in the original HTML. Finally, I completed the project by adding a “powered by GIPHY” linked image, and updated the styling on the page and dynamically created elements with CSS, and ensured the application was mobile responsive.

Licenses, Credits & Attributions: All images utilized in the collage banner were provided by https://www.pexels.com, a repository of free stock photos.

Link to Deployed Game: https://dannysprouse.github.io/GifTastic/

Copyright ©2018 Danny S. Sprouse All Rights Reserved