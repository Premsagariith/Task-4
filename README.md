 1. **Identified and Removed Fixed-Width or Rigid Layouts**
Used `flexbox` and `percentage-based widths` instead of fixed pixels for layout elements.

 2. **Added Media Queries (`@media max-width: 768px`)**
Introduced mobile-specific styling that:
- Stacked columns vertically
- Adjusted font sizes
- Modified spacing and padding
- Ensured flexible, readable layouts on small screens

3. **Created a Pure CSS Mobile Navigation Menu**
Since JavaScript was not allowed, a `checkbox + label` method was used to simulate a mobile nav toggle (hamburger menu):
- `<input type="checkbox" id="menu-toggle">` serves as the toggle
- `<label for="menu-toggle">☰</label>` acts as a clickable icon
- CSS controls visibility of `<ul>` using `:checked`

 4. **Styled Navigation for Mobile**
Nav items become a dropdown menu with a clean card-style popup using:
```css
#menu-toggle:checked + .hamburger + nav ul {
  display: flex;
}

5. Tested Responsiveness with Chrome DevTools
Used device toolbar (e.g. iPhone X, Galaxy S20) to check visual layout and interactions across screen sizes.

6. Fixed Overflow & Scaling Issues
Used box-sizing: border-box and max-width: 100% on images

Ensured all containers scale properly

7. Improved Design for Premium Feel
Added a hero section with background image and CTA

Used Google Fonts (Poppins) for a modern look

Added hover effects, rounded corners, and shadows

Included a footer for professional completeness