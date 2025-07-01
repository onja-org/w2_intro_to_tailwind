# 💡 CSS Tailwind Intro Lab

## 🎯 Tasks

**Objective:** ⚡️ Get familiar with using Tailwind CSS by creating a clone of a Discord page.

Use the Tailwind CSS docs to understand the different utility classes better.
https://tailwindcss.com/docs/display

The start of this lab will show you how to structure your elements with Tailwind CSS classes. It is important to write these out yourself without copy/pasting it, to help you remember the classes. 

### Sidebar

Let's start by creating a sidebar that is fixed on the left side of the screen from top to bottom. We will add temporary elements with letters to make sure it is all working correctly.

<div class="fixed top-0 left-0 h-screen w-16 flex flex-col bg-gray-900 text-white shadow-lg">
    <i>A</i>
    <i>B</i>
    <i>C</i>
    <i>D</i>
    <i>E</i>
</div>

Here is an explanation of each utility class used above:
- **fixed** sets the position to fixed
- **top-0** sets the fixed position to the top of the screen
- **left-0** sets the fixed position to the left of the screen
- **h-screen** sets the height to 100% of the view height
- **w-16** sets the width to 16 (units of tailwind spacing scale, not pixels)
- **flex** sets the display to flex
- **flex-col** sets the elements within to display as a column
- **bg-color-XXX** sets the background color
- **text-color** sets the color of the text
- **shadow-lg** sets the size of the shadow for the sidebar

### Icons

Now we need icons in our sidebar. These will be icons from the font awesome website, the <script> tag in the <head> of the document will allow these icons to be used. Inside the sidebar <div>, each icon will have its own <div> and an <i> element which will have a class from the font awesome website to fetch the icon.

Here are the classes necessary for the first icon, the discord logo. 

    <div class="relative flex items-center justify-center h-12 w-12 my-2 mx-auto shadow-lg bg-blue-800 text-white rounded-full">
        <i class="fa-brands fa-discord"></i>
    </div>

Once you have that icon, complete the rest of the icons with the same classes, except for the colors. the background color should be gray-800, with a text color of green-600.

Here is an explanation of all the new utility classes used:
- **relative** sets the position to relative
- **items-center** aligns items along the center of the containers cross axis
- **justify-center** justifies items along the center of the containers main axis
- **h-12 & w-12** sets height and width to make a square icon
- **my-2** sets both margins on the y-axis to 2
- **mx-auto** sets both margins on the x-axis to auto
- **rounded-full** rounds the edges of the element, full make a full circle (on square width/height elements)


### Transitions

Now that we have our icons displayed, we can add transitions to show the user when they are hovering over an icon. There are many different transitions we can add with Tailwind CSS fully installed, however with this project using the Tailwind CDN, our options are limited. Therefore we will only be changing the colors of the icon when hovering. 

To set a class to respond to a condition like hovering, you add the appropriate keyword before the class with a colon (:). An example for an element with a white background that changes to a black background when hovering would be "bg-white hover:bg-black"

For our main icons (not the blue discord logo), we have a gray background with green text/icon logo. Let's set the icons to change to a green-600 background with white text when hovering the mouse over it. For the discord logo icon, we can reverse the colors to a white background and text color of blue-800. We'll also need to set some classes for the transition effects. There are many options, but we will set the following classes for each icon:
- transition-all
- duration-300
- ease-linear

Here's the explanation for the new classes:
- **hover:bg-color-XXX** sets background color when hovering over element
- **hover:text-color** sets text color when hovering over element
- **transition-all** specifies which properties should transition
- **duration-XXX** set the transition duration of the element in milliseconds (e.g. duration-300)
- **ease-linear** sets the easing curve of the transition


### Main Content Area

Use what you've learned, and the Tailwind Docs, to fill out the main content area. There should be a: 

Heading section, with a maind heading and sub-heading, such as Discord, Onja Discord Server.

List of messages, with a user profile picture, username, and message

Input field at the bottom of the screen to send a new message to the server (does not need to be functional).

### Bonus features

- Using the given colors from tailwind does not match Discord completely. Create custom CSS classes in a CSS file to use matching colors

    Discord primary color: #202225
            secondary color: #2f3136
            tertiary color: #36393f

    Example: 
        CSS File

        .bg-primary {
            background-color: #202225;
        }

        HTML/Tailwind
        class="other classes... bg-primary ...other classes"

- 
