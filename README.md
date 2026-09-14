# Circular Progress Bar
This project is a circular progress bar created using HTML, CSS, and JavaScript while following a course provided by [Coddy.tech](https://coddy.tech/landing/courses/circular_progress_bar__frontend_project). It demonstrates how JavaScript can be used together with CSS gradients and DOM manipulation to create an animated progress indicator.

## Live Demo
View the project on **[GitHub Pages](https://brunorybicki.github.io/Circular-Progress-Bar/)**.

## Features
- **Animated Progress:** Increases the displayed percentage from `0%` to `90%`.
- **Circular Progress Indicator:** Uses `conic-gradient()` to visualize the current progress.
- **DOM Manipulation:** Updates the percentage text and progress circle dynamically with JavaScript.
- **JavaScript Timer:** Uses `setTimeout()` to control the speed of the animation.
- **Pseudo-element:** Uses the `::before` pseudo-element to create the inner white circle.
- **Gradient Background:** Applies a linear gradient to the page background.
- **Flexbox Layout:** Centers the progress component on the page.

## File Structure
- `index.html`: Contains the basic HTML structure and circular progress component.
- `styles.css`: Defines the layout, appearance, colors, and circular progress styling.
- `script.js`: Handles the progress animation and percentage updates.

## Usage
To run the project locally:
1. Download or clone the repository.
2. Open the `index.html` file in a web browser.
3. The progress animation will start automatically.

## How It Works
The `.circular-progress` element creates the circular progress indicator, while its `::before` pseudo-element creates the white inner circle. JavaScript selects the progress circle and percentage value using `document.querySelector()`.

The `updateProgress()` function increases the progress value one step at a time, updates the displayed percentage, and changes the `conic-gradient()` background of the progress circle. Each percentage point is multiplied by `3.6` to convert the value into degrees on a 360-degree circle. The function continues running with `setTimeout()` until the progress reaches `90%`.

## Customization
You can customize the progress bar by:
- Changing the target percentage in `progressEndValue`.
- Adjusting the animation speed using the `speed` value.
- Modifying the progress and background colors.
- Changing the size of the circular progress indicator.
- Editing the container size, spacing, and border radius.
- Changing the text size and colors.

## Acknowledgment
This project was built using the guide provided by Coddy.tech. The original project can be found **[here](https://coddy.tech/landing/courses/circular_progress_bar__frontend_project)**.
