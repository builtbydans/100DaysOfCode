# 100 Days Of Code

**Day 1** - I decided to start my journey with the Scrimba Frontend Developer path. In the first module
            'Web Dev Basics', I looked at the basic HTML strucutre and commonly-used elements to help
            build out your HTML. These included heading tags, anchor tags, unordered and ordered list tags and button tags. The main project iof the day was to recreate the Google landing page with pre-written CSS supplied.

**Day 2** - The second day of the module focussed on basic CSS. I continued to work on our Google
            project but instead writing the CSS from scratch. I was introduced to concepts such as display attributes, the box model and using flex-box. I was also exposed to looking at short-hand CSS attributes and how important accessibility is when using <img> tags and designing your frontend. The main project(s) of the day were to recreate the Google clone, build a digital business card using flex-box and increasing the complexity of the CSS we use by building a Space Exploration landing page.

**Day 3** - Today was a pure focus on Flex Box and the different attributes that form part of it. I
            looked at more complex use cases for align-items and justify-content, including looking at
            how to better layout the page taking the x and y axis into account. There was also an introduction to small CSS interactivity inlcuding the hover psuedo code and creating text-shadows and background gradients. The capstone project for the day was to build a birthday website with an image of a gift - when the user would hover over the gif they would be presented with a GIF.

**Day 4** - The course introduced us to JavaScript. The main focus was learning how variables work
            and how we can use DOM manipulation to change the state of the website. We were also introduced to basic datatypes such as string and number. By using the Console and console.log() function, I was able to debug my code and analyse what values were being returned. With this new knowledge, I created the capstone project of the day which was to create a person counter that had an increment button and a save button. One function incremented the counter element on the page and the save() function would save the state in another element that tracked the count.

**Day 5** - As we delve deeper into JS, the course then forces you to apply the learning thus far
            in the last 5 days by building a game score counter. This is built from scratch, including
            the UI. I started the project by breaking the main functions of the program into small tasks.
            I first started with creating the UI, so focussing on the CSS and HTML structure, making sure
            I am using id's and classes correctly. Then, with styling I used Flexbox and made sure that I followed the Figma design that was given to us. Finally, I created the JavaScript functions to increment the game score and as part of the stretch goal, I created a reset button which essentially reset the count variable and changed the DOM elements back to '0'.

**Day 6** - Deep dive into JavaScript today working on the capstone prokject 'Blackjack'. This brought together all the previous learnings including
            DOM manipulation, variables and introduced me to objects, callback functions and conditionals. The objective of the game was to render Blackjack to the client, which consisted of a button to generate a new card which calls a function that uses the Math() library. We then looked at using arrays to store the values of the card and then using a for loop to go through the array and send the values to the sum variable, which then would output the correct action depending on the score.

**Day 7** - As Module 3 'Website Interactivity' drew to an end, the path tests you on multiple JS challenges that contain problem
            sets for the learnings thus far on the module. These included reading from Object key-value pairs, conditionals,
            looping, using Array methods such as .push() and unshift() and learning how to randomise an element using Math() libraries.

            The final capstone project was a Random Password Generator, which upon pressing a button would generate two random 15 character passwords. We were provided with a Figma file that included colour palettes and a finished design and expected to code from scratch, including the HTML tree, the stylesheet and the JS functionality. I began by creating the UI, using Flexbox, margin and paddings and using appropriate naming conventions for both ID's and Classes. Once complete, I began the index.js file by breaking down the problem into small steps. Given an array of multiple characters, I began by retrieving the DOM element by calling the document object and storing this in variables - one for the left password and one for the right password. I then created empty arrays for both these password boxes with the intention to use a loop to grab random elements from the characters array and push them into these empty arrays.

            I then used a for loop and the Math() libraries to loop 15 times, grabbing a random character from the array and then setting the value of arr[i] as the generated password. Finally, I then changed the textContent for the DOM variables from earlier and use .join('') to remove any commas. The project was complete. I intend to continue working on this project by completing the stretch goals: give the user the ability to change the password length, copy password on click and give the user the ability to toggle if they want symbols and numbs in their password or just alphabetical characters.

**Day 8** - As part of the next major project for this module, I worked on building a Chrome Extension
            from scratch. The purpose of the Chrome Extension which was called 'Leads Tracker' was to allow the user to save input directly from the extension, save the tab URL directly from the extension and then to allow the user to delete their saved lists.

            The first part of the project was to build the UI. This simple UI consisted of an input element of the type "text" and three buttons. Each button was then given an appropriate clickhandler function in the index.js file.

            For this project, we ensured persistence by using localStorage. The module went through how to set and get items from localStorage and save them into a variable. This variable was an empty array called myLeads which would save all the leads. A function called render(leads) would then loop through this myLeads array and output DOM HTML in a form of a list, that of which was styled in the stylesheet.css. If there were no leads in the array, the render() function would still run but there would be nothing to render.

            For the 'Save Input' button, the function grabbed the inputElement.value and pushed this into an the myLeads array. The input value was then cleared, localStorage was updated and the render() function was called. For the 'Save Tab' button, we used a Chrome API to grab the URL of the current window and then store this into a Tabs object which was then pushed into the myLeads array, again calling the render() function to update the DOM.

            The final piece was the 'Delete All' button. As the name suggests, this cleared the localStorage use the .clear() function and emptied the myLeads array but re-initialising it as an empty array. As a stretch goal, I changed this into a double-click handler and added an alert() message for extra protection from accidental deletion.

            On this day, I learned about localStorage use, deploying Chrome Extensions, params and arguments in a function, using external API's and manfiest.json() files and manipulation JSON using the .parse() and .stringify() functions.

**Day 9** - Following from the major project yesterday, we continued to work on multiple projects that used the same techniques
            in order to strengthen our muscle memory. The solo project of thhe day was the Unit Converter. As usual, we were provided with a Figma file and a blank sheet. As with my other projects, I decided to create the UI first.

            This was pretty much again using Flexbox, however there were a number of <divs> that were wrapped in <container> tag. I had to go over this a few times in order to get the desired effect, but this continued to strenghten my knowledge of parent-child div relationships when usig flexbox. Furthermore, I learned how to center a <div> in the middle of the <body> tag and one trick I learned is to use overflow: hidden on a parent container - the reason I used this was because I was unable to manipulate the border-radius for the top div in the container object, until I searched for the issue online.

            For the JavaScript element, I found this much easier to break down than previous days. I knew that the first task I wanted to do was ensure I was able to retrieve an input value and add an eventListener to the button. Once I created my variables, I then created a singular function to generate a sentence for each of the units, with each changing depending on the measurement i.e. volume, mass or length. I decided to create this as a parent function, passing in 5 parameters. I wanted to keep the code DRY rather than repeating myself in the getMeasurement functions (which I would have 3 of). It may come across as confusing and upon review, I believe there would have been a more consise way of doing this. I used toFixed() function to round to 3 decimal places as in the requirements and was able to replicate the Figma file. The functions worked as they should and the unit program worked as intended.
