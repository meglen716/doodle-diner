# Doodle Diner

Doodle Diner is a fast-paced, 2D web-based cooking game where players race against the clock to assemble ingredient orders perfectly. Built entirely with web technologies, it features a responsive canvas and a modular graphics system tailored for easy custom art upgrades.

## Features
- Fast-paced stacking gameplay with time penalties and score bonuses.
- Built-in placeholder geometric graphics designed for effortless swapping to custom 2D art.
- Fully responsive HTML5 Canvas that scales dynamically to fit both desktop and mobile screens.
- Modular ES6 JavaScript architecture (currently structured within a single file for simple deployment).
- Custom UI overlays including a splash screen and game over screen styled with Tailwind CSS.

## How to Play
1. Read the Ticket: Look at the order ticket at the top of the screen to see the required ingredients.
2. Stack the Order: Tap or click the ingredient stations at the bottom to stack them on your central plate in the exact order shown (building from bottom to top).
3. Submit: Click "Submit" when your plate matches the ticket perfectly to gain points and bonus time.
4. Trash and Penalties: If you make a mistake, hit "Trash" to clear the plate. Submitting an incorrect order results in a 5-second time penalty.
5. Beat the Clock: Score as many points as possible before the 60-second shift ends.

## Tech Stack
- HTML5 Canvas API
- Vanilla JavaScript (ES6 Classes)
- Tailwind CSS (via CDN for UI styling)

## Customizing the Art
The game uses a dedicated GraphicsEngine class to handle rendering. To swap the geometric placeholder shapes with your own artwork:
1. Open the source code and locate the INGREDIENT_TYPES configuration object.
2. Add your custom image loading logic to the window.onload event.
3. Update the imgSrc property for the respective ingredient to point to your loaded image object. 
4. The graphics engine will automatically detect the image and draw it instead of the placeholder shape.

## Deployment
This project is contained entirely within a single `index.html` file, making it incredibly simple to deploy. Simply upload or push the file to your repository and enable GitHub Pages on the main branch.
