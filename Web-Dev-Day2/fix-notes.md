# Debugging Fix Notes

## Issues Found & Fixed

1.  **HTML Structure**:
    -   **Issue**: `<div>` tag for container was not closed.
    -   **Fix**: Added `</div>` at the end of the content body.
    -   **Issue**: `style` tag was closed as `</stlye>`.
    -   **Fix**: Corrected to `</style>`.
    -   **Issue**: Duplicate or missing structure tags (e.g., `<html>` lang attribute).
    -   **Fix**: Added `lang="en"` and `meta` viewport tag.

2.  **CSS/Styling**:
    -   **Issue**: Inline CSS in `<style>` block had valid syntax errors (missing braces, incorrect property syntax like `body background-color: #333`).
    -   **Fix**: Rewrote CSS with proper syntax (`selector { property: value; }`).
    -   **Issue**: `.container` width was set to `200%`, causing horizontal scroll/overflow.
    -   **Fix**: Changed width to `90%` and added `max-width`.
    -   **Issue**: Linked stylesheet path was `styles.css` (does not exist).
    -   **Fix**: Updated to `style.css` matching the project file.

3.  **Content/Assets**:
    -   **Issue**: Image source `missing-image.jpg` was broken.
    -   **Fix**: Replaced with `hero.png`.
    -   **Issue**: List items `<li>` were unclosed.
    -   **Fix**: Used closing `</li>` tags.
    -   **Issue**: Button `onclick` called undefined function.
    -   **Fix**: Changed to a simple `alert()`.
