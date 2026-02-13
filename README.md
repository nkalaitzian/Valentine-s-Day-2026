# Valentine's Day Page

A cute, interactive Valentine's Day webpage with playful animations, a mischievous "No" button, multi-language support, and accessibility options.

## Features
- Animated floating hearts background
- Playful "No" button that moves and morphs
- Multi-language support with rotating subtitles
- Accessibility controls (font size, colorblind palette, dark mode)
- Local preference persistence via cookies

## How to Use
Open index.html in a browser. Use the language selector in the top-right and the accessibility menu for display options.

## Icon Attribution
Cupid bow and arrow icon sourced from SVG Repo:
https://www.svgrepo.com/svg/171822/cupid-bow-and-arrow
Recolored to match the site's pastel palette.

---

<details>
<summary>Prompt History</summary>

1. I want to create a simple valentine's day webpage that will have a question "Will you be my valentine?" and two buttons: Yes, No. The yes button will be clickable, but the no button will jump all around the webpage randomly
	- Created the base page with the question, Yes/No buttons, and a moving No button.
2. Awesome, can we change the graphics to something more minimalistic and with more pastel colors? Prefer burgundy, purple, pink and red
	- Restyled the page with a minimal pastel palette and cleaner typography.
3. Great! Can we make the No button morph into a Yes button that's throbbing with a bright red border after 10 jumps? but when pressed, it won't trigger as the Yes button, but will instead make the no button reappear in a corner.
	- Added a jump counter, morph effect, and fake-Yes click behavior with a corner reset.
4. It needs to stop jumping around after the tenth jump to be clickable. After it's clicked it can start jumping around again
	- Stopped movement while morphed and resumed after the fake-Yes click.
5. can we change the background into small hearts floating around?
also, can we make it look more cute?
Take the attached image as an example to make it look a bit cuter
	- Added floating hearts, glassy card styling, and cuter typography/emojis.
6. The no button sometimes disappears altogether. I'm not sure if it might be getting shrunk to zero dimensions, or if it gets moved outside the dimensions of the browser window.
	- Adjusted positioning logic and cleared conflicting styles.
7. it still disappears after jumping around
	- Improved viewport clamping and cleared transforms.
8. Can you figure out what's wrong?
	- Added detailed debug logs and diagnostics for button positioning.
9. It still disappears
	- Tightened position calculations to keep the button inside the viewport.
10. It got hidden again
	- Added clamping and more viewport metrics in logs.
11. Perfect!
Can we add a funny semi-angry text to appear on screen?
	- Added a playful message on fake-Yes click with timed fadeout.
12. Great! can we add more lines (about 20 in total) and have a single one get chosen randomly?
Also, at the load of the page, can we have the two buttons be on the same line, centered vertically on the page?
	- Added a random pool of lines and centered the buttons.
13. They aren't exactly centered. The no button overlaps with the yes button.
	- Fixed layout by returning No to normal flow on load.
14. The no button can get a bit easy to lose. can we make it stand out a bit more? keep the color pastel if you can.
Can we also make the jumps a bit smoother? less of a teleport action, more of a phasing or a sliding action. If you can, make the transition a bit cute by adding something special to it - improvise
	- Enhanced styling, smooth transitions, and added a heart trail effect.
15. the button disappeared again
	- Moved the No button to the body when jumping to avoid stacking/context issues.
16. Perfect!
Can we add a translation button at the corner that switches from Greek to English Language? along with the appropriate translations for all visible text. And add a cookie so that the browser remembers which language has been chosen.
	- Added language switching and cookie persistence.
17. Perfect! Can we make the Greek language the default one?
	- Set Greek as the default if no cookie is present.
18. awesome! can we make the webpage mobile-friendly?
	- Added responsive styles for smaller screens.
19. Great! for mobile devices though, there will be no cursor to hover, so we need to change the behavior of the no button to work differently for these cases
	- Implemented touch-friendly behavior.
20. can we make it so when I click the yes button, the page will reset? not by a reload, but by resetting the buttons and the bottom text.
	- Implemented a timed reset of the UI without reload.
21. make the reset happen 5 seconds after the yes button is clicked
	- Updated the reset delay to 5 seconds.
22. Can we add more supported languages? Let's add support for French, German, Spanish, Portuguese, Italian, Bulgarian, Romanian, Polish, Chinese, Korean, Japanese
	- Added all requested languages and switched to a dropdown.
23. Awesome! Can we add alternative texts to "Μερικές ιστορίες αγάπης δεν επιτρέπουν το "όχι" 🐾"? Maybe 5 alternatives that get selected on page load.
	- Added rotating subtitle options for Greek.
24. Yeah, let's add rotating subtitles for the other languages as well. Feel free to switch up the tone of the text as well, use different emojis. Just keep it cute.
	- Added rotating subtitles for all languages.
25. Yes, please add more variants and make them playful. Also, if you can, change the subtitle emojis for the greek language. The first 4 all use the same emoji.
	- Expanded subtitle pools and varied Greek emojis.
26. Amazing! Can we also add an accessibility button next to the language select button? When inactive, it will display an accessibility icon, but if you click it, it will expand to reveal four buttons:
- + to decrease/increase font size
another button that will toggle colors for colorblinded people
and the fourth button will toggle between dark and light mode
	- Added an accessibility panel with font, colorblind, and theme toggles.
27. Amazing. Can we have the accessibility settings be stored in a cookie like the language?
	- Persisted a11y settings in cookies.
28. Amazing! Can we add a slight incognito footer at the bottom of the page that links to my ko-fi page?
https://ko-fi.com/pastouris
	- Added a subtle Ko-fi link in the footer.
29. Let's make it more minimal, and can you add the github repository link as well?
https://github.com/nkalaitzian/Valentine-s-Day-2026
	- Simplified footer and added GitHub link.
30. Maybe move the text to the lower-left corner.
	- Moved the footer to the lower-left.
31. Great!
Can we also add rotating emojis for the emoji header?
	- Added emoji rotation logic.
32. Actually, let's keep the emojis still
Let them change on page load, or when the yes button is clicked
	- Limited emoji changes to load and Yes clicks.
33. Oh, let's also rotate the subtitle when the yes button is clicked
	- Rotated subtitles on Yes click.
34. Can you create a simple README explaining what the page is?
Also, create a different section at the bottom of it, displaying every prompt I've asked you so far, from the beginning to the end. If I keep prompting you, add them to the end of the readme.
	- Added README with a prompt history section.
35. Can you think of a way to make the webpage more fun?
Either by adding more functionality, an easter egg, or something else.
	- Proposed secret mode, love meter, and cursor trail.
36. I love all three of these ideas.
	- Implemented all three features.
37. In the accessibility buttons, can we add a reset for the font size and a percentage display for how the size has changed?
	- Added a reset control and live font size percentage readout.
38. keep in mind to always update the README.md file with every new prompt
	- Acknowledged and will keep appending new prompts with summaries.
39. Perfect! Can we also add an icon for the browser tab?
	- Added a simple heart favicon and linked it in the HTML head.
40. Can we make the cursor change into a cupid bow and arrow when something happens? improvise on the conditions
	- Added a cupid cursor that activates during secret mode or when the love meter fills.
41. That doesn't really look like a cupid bow and arrow. Can you fix it?
	- Refined the cursor SVG for a clearer cupid arrow look.
42. Maybe just a cupid arrow? Like an arrow with a heart at the pointy end, and feathers at the back.
	- Replaced the cursor with a heart-tipped arrow design.
43. maybe something that looks more like this
	- Updated the cursor SVG to resemble the shared bow-and-arrow style.
44. Change the colors to fit the color scheme
Also, the shape is wrong
	- Adjusted the cursor colors to the pastel palette and simplified the bow silhouette.
45. I've downloaded a SVG from
https://www.svgrepo.com/svg/171822/cupid-bow-and-arrow
can you rename the file, color it with some of the colors we're already using and add a disclaimer in the readme about the source of the icon?
	- Replaced the cursor icon with the downloaded SVG, recolored it, and added attribution.
46. Rotate the svg 90 degrees counterclockwise
	- Rotated the cupid cursor SVG by -90 degrees.
</details>
