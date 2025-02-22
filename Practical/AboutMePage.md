```html

<!DOCTYPE html>
<html lang="en">
   <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>About Me - HTML Syntax Guide</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
      <script src="script.js"></script>
      <link rel="icon" href="favicon.ico" type="image/x-icon">
      <meta name="description" content="Learn HTML through my personal About Me webpage">
   </head>
   <body>
      <header>
         <h1>About Me</h1>
         <p>Welcome to my personal webpage, where I showcase my background and web development skills.</p>
         <img src="profile.jpg" alt="My Profile Picture" width="200" height="200">
         <nav>
            <ul>
               <li><a href="#introduction">Introduction</a></li>
               <li><a href="#skills">Skills</a></li>
               <li><a href="#examples">Examples</a></li>
               <li><a href="#contact">Contact</a></li>
            </ul>
         </nav>
      </header>
      <main>
         <section id="introduction">
            <h2>Introduction</h2>
            <p>Hello! My name is John Doe, and I am a web developer passionate about creating intuitive and functional websites.</p>
         </section>
         <section id="skills">
            <h2>My Skills</h2>
            <article>
               <h3>Web Development</h3>
               <p>I specialize in HTML, CSS, and JavaScript to build responsive and interactive websites.</p>
               <ul>
                  <li>HTML - Structuring the web</li>
                  <li>CSS - Styling web pages</li>
                  <li>JavaScript - Adding interactivity</li>
               </ul>
            </article>
         </section>
         <section id="examples">
            <h2>HTML Syntax Examples</h2>
            <article>
               <h3>Text Formatting</h3>
               <p><strong>Bold Text</strong>, <em>Italic Text</em>, <u>Underlined Text</u></p>
               <p><mark>Highlighted Text</mark></p>
               <p>Subscript: H<sub>2</sub>O, Superscript: x<sup>2</sup></p>
            </article>
            <article>
               <h3>Forms</h3>
               <form action="/register" method="post" enctype="multipart/form-data">
                  <fieldset>
                     <legend>Personal Information</legend>
                     <label for="name">Name:</label>
                     <input type="text" id="name" name="name" required autocomplete="name" readonly>
                     <label for="email">Email:</label>
                     <input type="email" id="email" name="email" required autocomplete="email" required>
                     <label for="password">Password:</label>
                     <input type="password" id="password" name="password" required>
                     <label for="phone">Phone:</label>
                     <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"
                        placeholder="123-456-7890">
                     <label for="birthday">Birthday:</label>
                     <input type="date" id="birthday" name="birthday">
                     <label for="profile_picture">Profile Picture:</label>
                     <input type="file" id="profile_picture" name="profile_picture" accept="image/*">
                  </fieldset>
                  <fieldset>
                     <legend>Address</legend>
                     <label for="address">Address:</label>
                     <textarea id="address" name="address" rows="3"></textarea>
                     <label for="city">City:</label>
                     <input type="text" id="city" name="city">
                     <label for="country">Country:</label>
                     <select id="country" name="country">
                        <option value="us">United States</option>
                        <option value="ca">Canada</option>
                        <option value="uk">United Kingdom</option>
                        <!-- Add more countries as needed -->
                     </select>
                  </fieldset>
                  <fieldset>
                     <legend>Preferences</legend>
                     <label>Gender:</label>
                     <label>
                     <input type="radio" name="gender" value="male">
                     Male
                     </label>
                     <label>
                     <input type="radio" name="gender" value="female">
                     Female
                     </label>
                     <label>
                     <input type="radio" name="gender" value="other">
                     Other
                     </label>
                     <label>
                     <input type="checkbox" id="subscribe" name="subscribe" checked>
                     Subscribe to newsletter
                     </label>
                     <label for="volume">Volume Preference:</label>
                     <input type="range" id="volume" name="volume" min="0" max="100" value="50">
                     <label for="favcolor">Favorite Color:</label>
                     <input type="color" id="favcolor" name="favcolor" value="#ff0000">
                  </fieldset>
                  <fieldset>
                     <legend>Additional Information</legend>
                     <label for="website">Website:</label>
                     <input type="url" id="website" name="website">
                     <label for="age">Age:</label>
                     <input type="number" id="age" name="age" min="13" max="120">
                     <input type="hidden" name="registration_date" value="<?php echo date('Y-m-d'); ?>" disabled>
                  </fieldset>
                  <input type="submit" value="Register">
                  <input type="reset" value="Reset">
                  <button type="button" onclick="alert('Cancel Registration')">Cancel</button>
               </form>
            </article>
            <article>
               <h3>Lists</h3>
               <ul>
                  <li>HTML Elements</li>
                  <li>CSS Properties</li>
                  <li>JavaScript Functions</li>
               </ul>
               <ol>
                  <li>Plan the website structure</li>
                  <li>Write the HTML code</li>
                  <li>Style with CSS</li>
                  <li>Add interactivity with JavaScript</li>
               </ol>
               <dl>
                  <dt>HTML</dt>
                  <dd>HyperText Markup Language - the structure of the web</dd>
                  <dt>CSS</dt>
                  <dd>Cascading Style Sheets - used for styling</dd>
               </dl>
            </article>
            <article>
               <h3>Table Example</h3>
               <table>
                  <caption>Programming Languages Popularity</caption>
                  <thead>
                     <tr>
                        <th>Language</th>
                        <th>Usage</th>
                     </tr>
                  </thead>
                  <tbody>
                     <tr>
                        <td>JavaScript</td>
                        <td>Web Development</td>
                     </tr>
                     <tr>
                        <td>Python</td>
                        <td>Data Science & AI</td>
                     </tr>
                  </tbody>
                  <tfoot>
                     <tr>
                        <td colspan="2">Data based on 2024 surveys</td>
                     </tr>
                  </tfoot>
               </table>
            </article>
         </section>
         <aside>
            <h2>Did You Know?</h2>
            <p>HTML stands for HyperText Markup Language and is the backbone of the web!</p>
         </aside>
         <section id="contact">
            <h2>Contact Me</h2>
            <p>If you'd like to collaborate, feel free to reach out via email at <a href="mailto:john.doe@example.com">john.doe@example.com</a>.</p>
            <video controls width="400">
               <source src="introduction.mp4" type="video/mp4">
               <source src="introduction.ogg" type="video/ogg">
               <source src="introduction.webm" type="video/webm">
               Your browser does not support the video tag.
            </video>
            <audio controls>
               <source src="background-music.mp3" type="audio/mp3">
               <source src="background-music.ogg" type="audio/ogg">
               <source src="background-music.wav" type="audio/wav">
               Your browser does not support the audio tag.
            </audio>
            <blockquote>
               <p>“The best way to predict the future is to create it.”</p>
               <cite>- Peter Drucker</cite>
            </blockquote>
            <figure>
               <figcaption>A Simple SVG Example:</figcaption>
               <svg width="100" height="100">
                  <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="blue" />
               </svg>
            </figure>
         </section>
      </main>
      <footer>
         <p>&copy; 2024 John Doe - All rights reserved.</p>
      </footer>
   </body>
</html>

```
