# PhyzzMars Frontend

<img src="logo.png" width="200">

PhyzzMars is a learning platform that helps students solve physics problems with the help of experts. This repository contains the frontend of its landing page. It is built with plain HTML and CSS and a very small piece of JavaScript. There is no framework and no build step, so the project is easy to read, easy to edit and easy to host anywhere.

## About the project

The page is written in Uzbek and introduces the idea of the application. A student who is stuck on a problem, especially in classical mechanics, can get a clear and complete solution from experts. The application lets users submit a problem in three ways, by voice, by photo or by text. It covers physics topics from primary school all the way up to university level.

## What is on the page

The landing page is a single screen that scrolls from top to bottom and is split into several sections.

The navigation bar sits at the top and holds the logo, the project name, four links and a start button that appears only on small screens. Below it the intro section greets the visitor with a large purple headline, a short pitch and a wide hero image with an arrow button. After that comes the features section, which shows three rounded cards that explain what the service offers. The info section then describes in more detail what students get and repeats the call to action with a green start button next to an illustration. The sponsors section shows the partners of the project, a specialized school named after Mirzo Ulug'bek and Mars Republic, and invites visitors to support the project. The footer closes the page with helper links, a link to the mobile app on Play Market and a copyright line.

## Project structure

The file main.html is the only page and contains all the markup. The folder style holds main.css, which contains every style rule including the responsive rules. The file app.js contains one small function that toggles a responsive class on the navigation list, which is meant for a mobile menu. The folder img keeps all pictures used on the page such as the logo, the hero image, the sponsor logos and the Play Market badge. The file logo.png in the root is used by this README. The folder .github/workflows holds a workflow that publishes the site.

## Running locally

Nothing has to be installed. Download or clone the repository and open main.html in any modern browser. If you prefer to use a local server, any static server will work, for example the Live Server extension in Visual Studio Code.

The page loads the Work Sans font from Google Fonts and the Font Awesome icon set from a CDN, so an internet connection is needed to see it exactly as designed.

## Responsive behavior

The layout adapts to different screen sizes with CSS media queries. The main container grows in steps from 320 pixels up to 1536 pixels depending on the width of the screen. On screens up to 768 pixels wide the project name is hidden, headlines become smaller, the cards and sponsors wrap onto new lines and the large illustration in the info section is removed. On screens up to 584 pixels wide the navigation links are hidden and a compact start button is shown instead.

## Deployment

The repository includes a GitHub Actions workflow that deploys the whole repository to GitHub Pages. It runs automatically on every push to the master branch and it can also be started manually from the Actions tab. Keep in mind that the entry file is called main.html, so on GitHub Pages the site opens at the path main.html unless the file is renamed to index.html.

## Notes for contributors

Most links and buttons on the page currently point to a placeholder and do not lead anywhere yet. The hamburger menu markup is commented out in main.html and in main.css, so the toggle function in app.js is not connected to anything for now. These are good places to start if you want to extend the project. When you add new sections, follow the existing naming style where class names describe the block and its parts, such as intro, intro__title and intro__text.
