# Jungle Devs - Frontend Fundamentals

  ## Description
  **Challenge goal**: The goal of the present challenge is to acquire and consolidate knowledge on HTML (a markup language) and CSS (a stylesheet language) by using them both to create a static webpage (no iterations with the user, show a display of content) based on a provided design.
  
  **Target level**: This is an entry level course, no prior knowledge of programming is needed.
  
  **Final accomplishment**: By the end of this course you'll be able to create static webpages using HTML and CSS. A webpage completely done by scratch based on a predefined design.
  
  
  ## Resources
  **Design**: [Figma](https://www.figma.com/file/fdncF938AXrCMjOFw1n483/Frontend-%E2%80%93-Challenge-1B)
  
  
  ## Acceptance criteria
  * Have HTML and CSS split in two files:
    * index.html;
    * styles.css.
  * Use the images from the [resource folder](/resources) (you can also export them on Figma, if you are up to an extra challenge);
  * HTML semantics usage (make sure you are using the correct tags);
  * CSS Grid and Flex box are mandatory;
  * Don't use inline styles.
  
## Prerequisites
  * Preferably, use an Integrated development environment (IDE) or code editor. 
    * Suggested Editor: Virtual Studio Code - VS Code (https://code.visualstudio.com/download);
  * Any browser, preferably your favorite.
  
## Instructions to Run
  * Fork this repository and clone it;
  * Open your index.html file and open it in your favorite browser (IE doesn't count 😆);
  * Every change you make to your HTML or CSS you'll need to refresh your webpage on your browser.
  
## Additional Information
  * Right click on your webpage and click on inspect to open the dev tools that will help your work. Use the elements tab (or inspector on firefox) to check the HTML and CSS you're applying to your webpage;
  * Not all HTML and CSS features work on all browsers. For more information, you can check on Can I Use if the feature is supported (https://caniuse.com/);
  * Check if the code editor of your choice has any extensions that can help you:
    * If you chose to use VS Code, you can use Live Server extension that will live reload your browser: https://github.com/ritwickdey/vscode-live-server.

## Improvements
#### Layout:
- [x] Wrong green color on "Become a Nanny Share host" and "send" buttons
- [x] Wrong font-weight on "Sarah's day care available now in North Sydney Wednesday, Thursday, Friday - 7:30 - 5:30"
- [x] Bad text shown "Well now it is, with Hapu.{' '} Hapu means tribe a"
- [x] Wrong color of division (hr element)
- [x] Wrong color of texts (usually black when they should have been gray)

#### Code:

- [x] The "Become a Nanny Share host" may look like a button, but it's most likely a link (it's ok not to know this, since it's only one screen) so semantically it should be an anchor tag. Same thing applies to the list inside the header/nav, they should have been anchors.
- [x] The section "Easily create or join a local nanny share with Hapu" is inside the header, but it isn't a header, it's the first section, this should be outside the header tag.
- [x] When you start a new section you're free to use a new h1 heading tag, going for an h2 is not a problem, but you could lose count of how many heading you had before, so always go for an h1 (remember to style it correctly)
- [x] Why did you put a span directly inside a paragraph? No need for the span `<p><span>Ready to get started?</span></p>`
- [x] Remember that the button tag main type is "submit" so every button outside a form you'll need to specify type="button"
- [x] When adding an outside link using an anchor with target blank always add [rel="noopener noreferrer"](https://pointjupiter.com/what-noopener-noreferrer-nofollow-explained/)  
- [x] When working with grid please use the [grid-template-areas](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-areas) instead of grid-column per item.
- [x] Use rem for everything, not only font-size (you can make it be multiple of 10 instead of 16 as the default)