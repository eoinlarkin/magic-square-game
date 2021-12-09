# Magic Square Game

![am-i-responsive](./docs/images/am-i-responsive.png)

## Objective

The objective of the site is to create a game based on [magic squares](https://en.wikipedia.org/wiki/Magic_square) for the user to solve. 

In developing the site, I decided to dynamically generate the magic squares; this introduced some complexity in the structure of the code but overall led to a more robust game with a large number of permutations for the number of potential magic squares to solve.

### User stories

As a site user:

- I want a site that is easy to use and navigate
- I want a site that offers varying difficulty levels and provides guidance if stuck
- I want a site that works across a number of devices

As a site owner:

- I want to ensure that the site has a distinctive visual identity
- I want to develop a site with a clear call to action
- I want to ensure that the Magic Square game is easy to play and provides assistance to the user if they are stuck
- I want to ensure that the user base is as wide as possible and that the site works across different platforms and screen sizes
- I want the ability to dynamically generate the magic squares as opposed to using a library of magic squares to serve to the user to solve

## Wireframes

Before building the site, I mapped out the following wireframes using [wireframe.cc](https://wireframe.cc/). My objective was to target a simple design and to ensure that the intention of each page was clear to the user.

  - <details>
    <summary><strong style="color:skyblue">Intro Page Wireframe:</strong></summary>
    <a href="https://wireframe.cc/cWFJp3" target="_blank">wireframe.cc</a>
    <img src="./docs/images/wireframe-intro-page.png" alt="wireframe-intro-page"/>
    </details>

  - <details>
    <summary><strong style="color:skyblue">Instructions Page Wireframe:</strong></summary>
    <a href="https://wireframe.cc/C2WVwq" target="_blank">wireframe.cc</a>
    <img src="./docs/images/wireframe-instructions-page.png" alt="wireframe-instructions-page"/>
    </details>

  - <details>
    <summary><strong style="color:skyblue">Settings Page Wirefame:</strong></summary>
    <a href="https://wireframe.cc/oG2XvV" target="_blank">wireframe.cc</a>
    <img src="./docs/images/wireframe-settings-page.png" alt="wireframe-settings-page"/>
    </details>

  - <details>
    <summary><strong style="color:skyblue">Game Page Wireframe:</strong></summary>
    <a href="https://wireframe.cc/FEA7MX" target="_blank">wireframe.cc</a>
    <img src="./docs/images/wireframe-game-page.png" alt="wireframe-game-page"/>
    </details>

  - <details>
    <summary><strong style="color:skyblue">Responsive Layout Wireframe:</strong></summary>
    <a href="https://wireframe.cc/HNiknf" target="_blank">wireframe.cc</a>
    <img src="./docs/images/wireframe-settings-responsive.png" alt="wireframe-settings-responsive"/>
    </details>

On implementing the actual design, I made one minor change - the three control buttons *(Instructions, Settings, Play Game)* were moved from within the game container box. Instead I decided to place these three buttons under the site title.

I felt that this led to an improved user experience, with a clear separation between the game and the controls used to move between the different game sections.

## JavaScript

JavaScript was used to achieve the following functionality:

- To dynamically create the values for the Magic Square that the user will solve
- To control user responses to button presses and to validate user inputs

### Magic Square Generation

A magic square of length and height of `root` n can be constructed using an array of length `n` of integers increasing by a constant `k`


In order to randomly generate a magic square, the following inputs are required:

- A sequence of n integers, with a fixed difference k between subsequent integers
- An algorithm for completing the magic square 

The De la Loubère (or siamese) method is proposed as the algorithm for completing the magic square.

![magic-square-gif](/docs/images/siamese-method.gif)

- Wikipedia page for Magic Squares: [link] 
- MathLab paper on Magic Squares: 
- Wikipedia page on the De la Loubère method" [link](https://en.wikipedia.org/wiki/Siamese_method)

### Site Interaction



## Layout and Features

Overview of the site features:

### Fonts

In selecting the fonts for the site I had two objectives:

- Select a title font that could be used in place of a logo
- Select a font that would compliment the title font while retaining legibility

The site fonts were chosen using [Google Fonts](https://fonts.google.com/). The fonts chosen were [Monoton](https://fonts.google.com/specimen/Monoton?query=monoton) for the title and [Titillium Web](https://fonts.google.com/specimen/Titillium+Web?query=titill) for the body content.

### Color Scheme

<img src="./docs/images/magic-square-palette.png" alt="color-palette" width=400px height=200px>

A broad color palette was chosen for the site with a range of complimenting colors chosen.

In choosing the color palette, my objective was to select a color palette that would create a strong visual identity as well as suggest a playful, fun game.


### Layout and Features
The following section provides an overview of the site features and design, with screenshots providing a visual overview of each feature.

- **Introduction Container**

  - <details>
    <summary><strong style="color:skyblue">Screenshot:</strong></summary>
    <img src="./docs/images/screenshot-01-intro.png" alt="intro-container"/>
    </details>
  - The Introduction pane welcomes the user to the site and features a clear call to action.
  - I originally planned a site logo, however ultimately I used a text logo; this logo animates when the user hovers over it and adds to overall identity of the site. 


- **Instructions Container**
  
  - <details>
    <summary><strong style="color:skyblue">Screenshot:</strong></summary>
    <img src="./docs/images/screenshot-02-instructions.png" alt="intro-container"/>
    </details>
  - Overview of feature 1


- **Settings Container**

  - <details>
    <summary><strong style="color:skyblue">Screenshot:</strong></summary>
    <img src="./docs/images/screenshot-03-settings.png" alt="settingscd-container"/>
    </details>
  - Overview of feature 1

- **Game Container**

  - <details>
    <summary><strong style="color:skyblue">Screenshot 01:</strong></summary>
    <img src="./docs/images/screenshot-04-game-01.png" alt="game-container-01"/>
    </details>
  - <details>
    <summary><strong style="color:skyblue">Screenshot 02:</strong></summary>
    <img src="./docs/images/screenshot-04-game-02.png" alt="game-container-02"/>
    </details>
  - Overview of feature 1

- **Responsive Design**

  - <details>
    <summary><strong style="color:skyblue">Screenshot:</strong></summary>
    <img src="./docs/images/screenshot-03-settings-responsive.png" alt="responsive-design"/>
    </details>
  - Overview of feature 1


### Potential Additional Features

Overall, I am satisfied with the functionality and feature set of the developed site. In terms of additional features, I believe the game could be further enhanced through the addition of a scoreboard feature.

- **Scoreboard**
This would provide users with the ability to view their scores; I would propose implementing a timer, with the user assigned a scored based on how quickly they managed to solve the Magic Square. The feature would require the use of local storage to record the user name and score and allow multiple users to play against each other.

## Testing 

### Device Testing

Testing was completed across a number of platforms as follows:

- The site was tested on Chrome, Firefox and Safari
- Platform specific testing was completed on Windows and Linux desktop environments. Mobile testing was completed on iOS
- The site responsiveness was tested across both Apple phones and tables. In addition, responsiveness was tested using Chrome Dev Tools, wth screen sizes from `280px` (Galaxy Fold) upwards tested.

### Performance Testing

Performance was tested using Lighthouse in Chrome Dev Tools. No significant issues were reported for either Desktop of Mobile

- **Desktop Results**  
  ![lighthouse-desktop](docs/lighthouse/lighthouse-desktop.png)  
  The full report can be found [here](docs/lighthouse/lighthouse-desktop.pdf)

- **Mobile Results**  
  ![lighthouse-mobile](docs/lighthouse/lighthouse-mobile.png)  
  The full report can be found [here](docs/lighthouse/lighthouse-mobile.pdf)


### Validator Testing 

- HTML
    - No errors were reported when running the code through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Feoinlarkin.github.io%2Fmagic-square-game%2F) 
- CSS
    - No errors were found when passing through the official [Jigsaw validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Feoinlarkin.github.io%2Fmagic-square-game%2F&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - A number of warnings were triggered; however these related to the use of vendor extensions to enable the animation of the main title (e.g. `-moz-text-fill-color`)
- JavaScript
    - No errors were found when passing through the official [Jshint validator](https://jshint.com/).
    - The following screenshot summarises the output:  
    ![jshint](docs/jshint/jshint-output.png)
      


### Bugs

The min max values returned NaN - this was fixed by referencing the following link :
https://medium.com/@vladbezden/how-to-get-min-or-max-of-an-array-in-javascript-1c264ec6e1aa


### Unfixed Bugs

There are no known bugs present in the final site deployment.

## Deployment

The site was deployed using GitHub pages to the following location: [link](https://eoinlarkin.github.io/magic-square-game/)

## Attribution 

- The following guide was used to create the text gradients [link](https://fossheim.io/writing/posts/css-text-gradient/)
- The following StackOverFlow post was used to help implement the fadeIn and fadeOut functionality of the `container-intro` div: [link](https://stackoverflow.com/questions/12584481/simple-fade-in-fade-out-div-with-jquery-on-click)
- Sample code was leveraged from the following CodePen example to create the animated gradient for the title [link](https://codepen.io/bsander/pen/pPpbNm?editors=1100)
- The following code was 
- The following paper was used to better understand the algorithm to generate the Magic Square: [link](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/magic.pdf)
- The following code examples were used to help create the alert banners that were used for the *hint*, *correct answer* and *wrong answer* messages: [link](https://www.w3schools.com/howto/howto_js_alert.asp)

- - - 

## Development

### Languages
- HTML
- CSS
- JavaScript
- jQuery

### Tools / Technologies

- **[VScode](https://code.visualstudio.com/)**  
All coding was completed in VS Code.
- **[cdnjs](https://cdnjs.com/libraries/jquery)**
cdnjs was used as the reference for the jQuery JavaScript library.
- **[coolors.co](https://coolors.co/)**  
Potential site palettes were tested with Coolors.  
- **[gauger.io](https://gauger.io/fonticon/)**  
This website was used to generate the favicon using an icon from Font Awesome.
- **[Am I Responsive?](http://ami.responsivedesign.is/)**  
For rendering the device preview image
- **[https://ecotrust-canada.github.io/](https://ecotrust-canada.github.io/markdown-toc/)**  
For generating the formatted table of contents in markdown
- **[Google Fonts](https://fonts.google.com/)**  
Used to provide the custom fonts for the site


Other

- CodeInstitute modules on HTML, CSS and JavaScript.
- My mentor for his suggestions and feedback on the project.
- My friends who helped test the logic and design of the website.
- My teachers who first introduced me to Magic Squares and the symmetries that exist in mathematics.

- - - 