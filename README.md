# Dynamic Content Loader

This repository hosts a responsive iframe loader for various types of content, including PDF documents and websites. The dynamic content loader is designed to be used with TimelineJS to display media content within the timeline slides.

## Features

- Responsive iframe for embedding content
- Supports PDF documents and websites
- Easy integration with TimelineJS
- Customizable aspect ratio for iframe

## Usage

1. Host the `dynamic-content-loader.html` file on a web server or a platform like GitHub Pages, Netlify, or any other hosting provider that allows you to host static HTML files.

2. For each timeline event in your Google Sheets document, append the content URL (either PDF or website) as a query parameter to the hosted `dynamic-content-loader.html` file URL. The format should look like this:

https://yourwebsite.com/dynamic-content-loader.html?content=https://path-to-your-content.pdf-or-website
 
3. Paste the modified URL into the "Media" column for each slide in your Google Sheets document.

Now, when you preview your TimelineJS timeline, each slide will display the content (PDF or website) using the dynamic content loader, loading the appropriate content based on the query parameter.

## Customization

To adjust the aspect ratio of the responsive iframe, edit the `padding-top` value in the `.responsive-iframe-container` CSS rule within the `dynamic-content-loader.html` file. The default value is `56.25%`, which corresponds to a 16:9 aspect ratio. Change this value to achieve your desired aspect ratio.

## License

This project is open-source and available for free use, modification, and distribution under the MIT License. See the LICENSE file for more details.
