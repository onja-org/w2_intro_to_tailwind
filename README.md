# 💡 CSS Tailwind Intro Lab

## 🎯 Tasks

**Objective:** ⚡️ Get familiar with using Tailwind CSS by creating a clone of a Discord page.

Use the Tailwind CSS docs to understand the different utility classes better.
https://tailwindcss.com/docs/display

### Sidebar

Use the following utility classes to create the sidebar:

- **fixed** sets the position to fixed
- **top-0** sets the fixed position to the top of the screen
- **left-0** sets the fixed position to the left of the screen
- **h-screen** sets the height to 100% of the view height
- **w-16** sets the width to 16 (units of tailwind spacing scale, not pixels)
- **flex** sets the display to flex
- **flex-col** sets the elements within to display as a column
- **bg-color-XXX** sets the background color (e.g. bg-gray-900)
- **text-color** sets the color of the text (e.g. text-white)
- **shadow-lg** sets the size of the shadow for the sidebar

### Icons

Use the following utility classes to create the icons in the sidebar
(if possible use font awesome? maybe one onja account that everyone can log into)

- **relative** sets the position to relative
- **flex**
- **items-center** aligns items along the center of the containers cross axis
- **justify-center** justifies items along the center of the containers main axis
- **h-12 & w-12** sets height and width to make a square icon
- **my-2** sets both margins on the y-axis to 2
- **mx-auto** sets both margins on the x-axis to auto
- **shadow-lg**
- **bg-color-XXX**
- **text-color-XXX**
- **hover:bg-color-XXX** sets background color when hovering over element
- **hover:text-color** sets text color when hovering over element
- **rounded-full** rounds the edges of the element, full make a full circle (on square width/height elements)
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
