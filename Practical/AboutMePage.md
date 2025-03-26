<!DOCTYPE html>
<html lang="en">
   <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>About Me - HTML Syntax Guide</title>
      <link rel="stylesheet" type="text/css" href="styles.css">
      <script src="script.js" defer></script>
      <link rel="icon" href="favicon.ico" type="image/x-icon">
      <meta name="description" content="Learn HTML through my personal About Me webpage">
      <meta name="author" content="John Doe">
      <meta name="keywords" content="HTML, CSS, JavaScript, Web Development">
      <base href="https://example.com/">
   </head>
   <body>
      <header>
         <h1>About Me</h1>
         <p>Welcome to my personal webpage, where I showcase my background and web development skills.</p>
         <picture>
            <source media="(min-width: 800px)" srcset="profile-large.jpg">
            <source media="(min-width: 400px)" srcset="profile-medium.jpg">
            <img src="profile.jpg" alt="My Profile Picture" width="200" height="200">
         </picture>
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
            <details>
               <summary>More about me</summary>
               <p>I have been developing websites for over 5 years and specialize in front-end technologies.</p>
            </details>
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
               <meter value="90" min="0" max="100">90%</meter>
               <progress value="75" max="100">75%</progress>
            </article>
         </section>
         <section id="examples">
            <h2>HTML Syntax Examples</h2>
            <article>
               <h3>Text Formatting</h3>
               <p><strong>Bold Text</strong>, <em>Italic Text</em>, <u>Underlined Text</u></p>
               <p><mark>Highlighted Text</mark></p>
               <p>Subscript: H<sub>2</sub>O, Superscript: x<sup>2</sup></p>
               <p><small>Small text for fine print</small></p>
               <p><time datetime="2024-03-20">March 20, 2024</time></p>
               <p><data value="123">Product ID</data></p>
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
                     <label for="browser">Choose browser from list:</label>
                     <input list="browsers" id="browser" name="browser">
                     <datalist id="browsers">
                        <option value="Chrome">
                        <option value="Firefox">
                        <option value="Safari">
                     </datalist>
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
                        <optgroup label="Europe">
                           <option value="fr">France</option>
                           <option value="de">Germany</option>
                        </optgroup>
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
                     <output name="result" for="age"></output>
                     <input type="hidden" name="registration_date" value="<?php echo date('Y-m-d'); ?>" disabled>
                     <template>
                        <div>This content is hidden during page load</div>
                     </template>
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
               <ol reversed start="10">
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
                  <colgroup>
                     <col span="1" style="background-color: #f0f0f0">
                     <col span="1" style="background-color: #e0e0e0">
                  </colgroup>
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
            <ruby>
               漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
            </ruby>
         </aside>
         <section id="contact">
            <h2>Contact Me</h2>
            <p>If you'd like to collaborate, feel free to reach out via email at <a href="mailto:john.doe@example.com">john.doe@example.com</a>.</p>
            <video controls width="400" poster="video-preview.jpg">
               <source src="introduction.mp4" type="video/mp4">
               <source src="introduction.ogg" type="video/ogg">
               <source src="introduction.webm" type="video/webm">
               <track src="subtitles_en.vtt" kind="subtitles" srclang="en" label="English">
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
            <canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;"></canvas>
         </section>
      </main>
      <footer>
         <address>
            Contact: <a href="mailto:john.doe@example.com">John Doe</a><br>
            123 Web Dev Street<br>
            Internet City
         </address>
         <p>&copy; 2024 John Doe - All rights reserved.</p>
         <p><bdi>User123</bdi>: 5 stars</p>
         <p><wbr>verylongwordthatneedstobreakatsomepoint</wbr></p>
      </footer>
   </body>
</html>
