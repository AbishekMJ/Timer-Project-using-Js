# Timer-Project-using-Js
 It is a Java Script Project 
This HTML and CSS code represents a basic timer interface, often referred to as a Pomodoro Timer, where users can adjust session and break lengths, start and stop the timer, and reset it. Here's an explanation of the different parts of the code:

### HTML Structure

- **DOCTYPE Declaration and Language**: The `<!DOCTYPE html>` declares the document type as HTML5. The `lang="en"` attribute in the `<html>` tag specifies the language of the content.

- **Head Section**:
  - The `<meta charset="UTF-8">` sets the character encoding to UTF-8, ensuring the correct display of characters.
  - The `<meta name="viewport" content="width=device-width, initial-scale=1.0">` tag makes the page responsive by controlling the page's dimensions and scaling.
  - `<title>document</title>` sets the title of the webpage, which appears in the browser's title bar or tab.
  - The `<style>` tag contains the CSS styles that control the appearance and layout of the page.

- **Body Section**:
  - **Container**: The `.container` div houses all the elements of the timer.
  - **Timer Display**: The `.timer-display` div shows the current time left in the session.
  - **Session Length Display**: The `.session` and `.close session` divs display and control the session and break lengths, respectively.
  - **Control Panel**: Each `.control-panel` div includes buttons to increase or decrease session/break lengths, with the current length displayed in between.
  - **Buttons**: The `.buttons` div contains the "Reset" and "Start/Stop" buttons to control the timer.

### CSS Styling

- **Body**:
  - The `display: flex;` property makes the container a flexbox, which helps in centering and aligning the contents.
  - The background color is set to black, and the text is aligned to the center.

- **Container**:
  - The `.container` is centered, with white text color and a width of 100%.

- **Timer Display**:
  - The `.timer-display` div is styled with a large font size and centered content to clearly display the time left.

- **Session and Break Controls**:
  - `.session` and `.close session` are given a background with slight opacity for a subtle visual effect.
  - Buttons within `.control-panel` are styled to be large and easy to interact with.

- **Buttons**:
  - The `#reset` and `#start_stop` buttons have different background colors to differentiate their functions.

### JavaScript Functionality

- **Variables**:
  - `sessionLength` and `breakLength` store the duration for sessions and breaks.
  - `interval` and `isRunning` control the timer's state.

- **Session and Break Adjustments**:
  - Event listeners on the increment/decrement buttons (`session-increment`, `session-decrement`, etc.) adjust the session and break lengths, updating the display accordingly.

- **Timer Control**:
  - The `#start_stop` button starts or stops the timer by toggling `isRunning`. It also updates the button's text between "Start" and "Stop".
  - The `#reset` button resets the session and break lengths to default values and updates the timer display.

- **Timer Update**:
  - The `updateTimer()` function updates the timer display based on the current session length.
  - The `startTimer()` function handles the countdown logic, updating the minutes and seconds every second.

This code provides the basic functionality for a Pomodoro Timer, where users can set session times, start/stop the timer, and reset it to default values. The design is minimalistic with clear visual cues and interactive elements.
