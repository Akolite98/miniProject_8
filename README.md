# Animated Letters - Final Project

This web page presents an interesting animation effect that scales and rotates individual letters when you hover your mouse over them. The effect is created using HTML, CSS, and JavaScript.

## Getting Started

To view the animated letters, open the provided HTML file named `index.html` in your web browser. No additional setup or installation is required.

## How to Use

1. Open the `index.html` file in your web browser.

2. The web page will display the heading "Final Project" along with a sentence.

3. Hover your mouse over each letter of the sentence, and you will notice the letter scales up and rotates slightly.

## Code Details

The implementation uses HTML, CSS, and JavaScript to achieve the animated effect.

### CSS Styles

The CSS styles are embedded in the HTML file within a `<style>` block. The styles define the appearance and animation of the letters.

- The `body` background color is set to `#f5f5f5`, creating a light gray background for the page.

- The `.letter` class represents individual letters and sets their initial style:

  - Font size: `90px`
  - Font family: `"Pacifico", cursive`
  - Display: `inline-block`
  - Color: `#999` (light gray)
  - Transition: `all 250ms ease-in-out` for smooth scaling and rotation animations.

- The `.letter.active` class defines the styles when a letter is active (when the mouse hovers over it):
  - It scales the letter to `1.5` times its original size.
  - It rotates the letter `20deg` clockwise.
  - It changes the color of the letter to `green`.

### JavaScript Logic

The JavaScript code enhances the text inside the `<h1>` element to make individual letters interactive with the mouse.

- The `h1` element is selected using `document.querySelector("h1")`.

- The text content of the `<h1>` element is split into individual letters using `split("")`, and each letter is enclosed within a `<span>` element with the class `letter`.

- Event listeners are added to each letter using the class `js-letter`.
  - When the mouse hovers over a letter (`mouseover` event), the letter's class is changed to `active`, which triggers the scaling and rotation animation defined in the CSS styles.
  - When the mouse moves away from the letter (`mouseout` event), the `active` class is removed, reverting the letter to its original state.

## Note

- This mini-project demonstrates a fun animation effect using basic HTML, CSS, and JavaScript. You can apply similar techniques to create more complex animations and interactivity on your web pages.

- The effect is designed for desktop or laptop devices with a mouse. It may not work as intended on touch-enabled devices.
