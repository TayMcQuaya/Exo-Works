# How to Extract and Use Images for Your Website

This guide explains how to extract specific images from your page screenshots (the `.jpg` files like `Page4.jpg`, `Page5.jpg`, etc.) and add them to your single-page website.

## 1. Why Extract Images?

Your website currently uses placeholder images. To make it look like your PDF brochure, you need to replace these placeholders with the actual images (logos, photos, diagrams, UI screenshots) from your design. Extracting them means "cutting out" just the part of the screenshot you need.

## 2. How to Extract/Crop Images

You'll need a basic image editing tool to crop the images. Most computers have built-in tools:

*   **Windows:**
    *   Open your screenshot (`.jpg` file) with the **Photos** app or **Paint/Paint 3D**.
    *   Look for a **Crop** tool (it usually looks like two right angles forming a square).
    *   Drag the handles of the crop box to select only the specific image element you want (e.g., just the logo, or just a person's photo).
    *   Apply the crop.
    *   Save this cropped image as a **new file**. Use `File > Save a copy` or `Save as` to avoid overwriting your original screenshot.

*   **Mac:**
    *   Open your screenshot (`.jpg` file) with the **Preview** app.
    *   Click and drag your mouse to draw a rectangle around the image element you want.
    *   Go to `Tools > Crop` in the menu bar (or press `Command+K`).
    *   The image will be cropped to your selection.
    *   Save this as a **new file**. Use `File > Export...` or `File > Save As...` and choose a new name and location.

*   **Other Tools:**
    *   Many free online image editors (search for "free online image cropper") or downloadable software (like [GIMP](https://www.gimp.org/)) can also be used. They will have similar crop functionalities.

## 3. Naming and Saving Your Extracted Images

*   **Folder:** Save all your extracted images into the `images` folder located in the same directory as your `index.html` and `style.css` files. (If this folder doesn't exist, please create it).
*   **File Names:**
    *   Use descriptive, lowercase names (e.g., `exoworks_logo.png`, `team_member_jane.jpg`).
    *   Use underscores (`_`) or hyphens (`-`) to separate words. Avoid spaces or special characters.
*   **File Formats:**
    *   **`.png`:** Best for logos, diagrams, icons, or any image with sharp lines, text, or areas of flat color, especially if it needs a transparent background (though for this project, transparency isn't strictly required by the design).
    *   **`.jpg` (or `.jpeg`):** Best for photographs (like team member photos or the main image in the "AI Education" section) as it handles complex colors and gradients well and can be compressed to smaller file sizes.

## 4. Updating the Website (index.html)

After saving your extracted images in the `images` folder, you need to tell the website where to find them by editing the `index.html` file:

1.  Open `index.html` in a text editor.
2.  Look for `<img>` tags. These are used to display images.
3.  Each `<img>` tag has a `src` attribute, which stands for "source." This tells the browser which image file to load.
    Example: `<img src="images/logo_placeholder.png" alt="ExoWorks Logo" class="logo">`
4.  Change the placeholder file name in the `src` attribute to your actual image file name.
    If you saved your logo as `exoworks_logo.png`, the line above would become:
    `<img src="images/exoworks_logo.png" alt="ExoWorks Logo" class="logo">`
    **Important:** Make sure the path starts with `images/` because your images are inside the `images` folder.

## 5. List of Placeholder Images and Suggested New Names

Here's a reminder of the placeholders used in `index.html` and what they refer to. Replace the `src` value for each with the path to your actual extracted image:

*   **Logo (used in multiple sections):**
    *   Placeholder: `images/logo_placeholder.png`
    *   Example new name: `images/exoworks_logo.png`

*   **AI Education Section (`#ai-education`):**
    *   Placeholder: `images/ai_education_placeholder.png` (Image of person with laptop)
    *   Example new name: `images/ai_education_main.jpg`

*   **Solution Section (`#solution`):**
    *   Placeholder: `images/solution_platform_1_placeholder.png` (Left platform UI screenshot)
    *   Example new name: `images/solution_ui_left.jpg`
    *   Placeholder: `images/solution_platform_2_placeholder.png` (Right platform UI screenshot)
    *   Example new name: `images/solution_ui_right.jpg`

*   **Product Section (`#product`):**
    *   Placeholder: `images/schools_diagram_placeholder.png` ("TRADITIONAL SCHOOLS -> AI SCHOOLS" diagram)
    *   Example new name: `images/schools_flow_diagram.png`
    *   Placeholder: `images/dashboard_1_placeholder.png` (Top dashboard screenshot)
    *   Example new name: `images/product_dashboard_top.jpg`
    *   Placeholder: `images/dashboard_2_placeholder.png` (Bottom dashboard screenshot)
    *   Example new name: `images/product_dashboard_bottom.jpg`

*   **Our Team Section (`#our-team`):**
    *   Placeholder: `images/salim_ismail_placeholder.png`
    *   Example new name: `images/salim_ismail.jpg`
    *   Placeholder: `images/eric_pulier_placeholder.png`
    *   Example new name: `images/eric_pulier.jpg`
    *   Placeholder: `images/greg_pulier_placeholder.png`
    *   Example new name: `images/greg_pulier.jpg`

## 6. Viewing Your Changes

After updating the `src` paths in `index.html` and saving the file, open `index.html` in your web browser (usually by double-clicking it) to see your images on the website!

If an image doesn't appear, double-check:
*   The file name in the `src` attribute exactly matches the name of your image file (it's case-sensitive on some systems).
*   The image file is indeed in the `images` folder.
*   The path starts with `images/`.

---

Good luck! Let me know if you have any questions.
