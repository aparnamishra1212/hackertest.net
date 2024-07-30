# Hackertest.net Solutions

Welcome to the Hacker Test Solutions repository! This repository provides a step-by-step guide for solving the challenges presented on [Hacker Test](http://www.hackertest.net/), an online "hacker simulator" designed to test and improve your hacking skills.

## Overview

The Hacker Test offers a series of challenges that require you to think like a hacker and utilize various web development and security skills. This guide documents the solutions and thought processes for each level, starting from Level 1 and going up.

## Tools and Prerequisites

To successfully complete the challenges, you'll need:
- A web browser with developer tools (e.g., Firefox, Chrome).
- An application for manipulating images, such as Photoshop or GIMP (optional but helpful).
- Basic knowledge of HTML, JavaScript, and web security concepts.

## Solutions

### Level 1

**Direct Link:** [Level 1](http://www.hackertest.net/)

**Explanation:**
This is the simplest level. The objective is to examine the HTML source code of the page to find any hard-coded information related to the password.

1. Open the page and view the HTML source (cmd-U in Firefox).
2. Look for obvious elements such as "password".
3. Find the `check()` function which compares the input with the expected password.
4. The expected password is `null`.

### Level 2

**Direct Link:** [Level 2](http://www.hackertest.net/null.htm)

**Explanation:**
Similar to Level 1, the password is embedded in the HTML source code. This time, you need to look for a specific string comparison.

1. View the HTML source.
2. Find the password prompt and comparison string.
3. The password is `l3l`.

### Level 3

**Direct Link:** [Level 3](http://www.hackertest.net/l3l.htm)

**Explanation:**
In this level, you are introduced to color-related attributes in the HTML source. The password is hidden within these attributes.

1. View the HTML source.
2. Look for references to "alinkColor".
3. The expected password is `#000000`.

### Level 4 & 5

**Direct Link:** [Level 4 & 5](http://www.hackertest.net/abrae.htm)

**Explanation:**
Level 4 seems like a placeholder as clicking a link directly takes you to Level 5. In Level 5, the password is again in plain sight in the HTML source.

1. Click the "Click here" link to go to the next level.
2. View the source of the new page.
3. The password is `SAvE-as hELpS a lOt`.

### Level 6

**Direct Link:** [Level 6](http://www.hackertest.net/save_as.htm)

**Explanation:**
This level requires you to follow a link to an external JavaScript file where the password is stored.

1. View the HTML source.
2. Follow the link to the external JavaScript file (`passwd.js`).
3. The password is `hackertestz`.

### Level 7

**Direct Link:** [Level 7](http://www.hackertest.net/included.htm)

**Explanation:**
Here, the password is hidden in an image file referenced in the HTML source. You'll need to view the image to find the credentials.

1. View the HTML source.
2. Inspect the background asset (`bg="images/included.gif"`).
3. The credentials are found in the bottom right corner of the image:
    - Username: `phat`
    - Password: `jerkybar3`

Here's a Markdown-friendly format suitable for a GitHub README file:

### LEVEL8

**Direct Link:** [Level 8](http://www.hackertest.net/pwd2.php)  
**Explanation:** The solution involves finding and downloading a PhotoShop document hidden in the source code.

1. View the HTML source and locate the link to the PHP script (`phat.php`).
2. Follow the link and check for the included background image reference.
3. Go to [phat.gif](http://www.hackertest.net/images/phat.gif) and note the instruction: "Look for a .PhotoShopDocument!".
4. Navigate to [phat.psd](http://www.hackertest.net/images/phat.psd) and download the file.
5. Open the file in a program that supports PSD layers (e.g., GIMP).
6. Hide all layers and add them back one by one to find the credentials:
   - **Username:** `zadmin`
   - **Password:** `stebbins`

### LEVEL9

**Direct Link:** [Level 9](http://www.hackertest.net/phat.php)  
**Explanation:** The password is encoded in base64 and requires decoding.

1. Check the HTML source and scroll to find "Password: Z2F6ZWJydWg=".
2. Decode the base64 string:
   - **Encoded:** `Z2F6ZWJydWg=`
   - **Decoded:** `gazebruh`
3. Add a page extension to the decoded word to proceed.

### LEVEL10

**Direct Link:** [Level 10](http://www.hackertest.net/gazebruh.php)  
**Explanation:** The password is hidden within the text on the page using italicized letters.

1. Review the text and identify the italicized letters.
2. Combine the italicized letters to form the password: `shackithalf`.

---
