# Technical Debt

A running list of sources of potential technical debt within ORCA and its environment.

## Source Repository / Build Process

### Outdated RCS
The code is stored in [Rational ClearCase](https://en.wikipedia.org/wiki/Rational_ClearCase), a revision control system from the early 1990s. It doesn't integrate with any modern DevOps tools, which functionally blocks any modernization of the deployment process.

### Homebrewed Deploy Process
The deploy process is run on a custom system. It works just fine, but, like the use of ClearCase, this is an obstacle to integrating with modern DevOps tools.

### Obviated COBOL
The repository has a fair amount of COBOL in it. This is said to have been replaced with Java-based functionality in ~2013, but it remains in the repo.

### Obviated Batch Scripts
The repository has a fair number of batch scripts throughout, for the testing and deploy process. This is quite normal, but apparently these were replaced with Java-based functionality sometime in the past few years. Leaving them in the repo provides the illusion of functionality in the wrong place.

## Front End

### IE-Specific Code
The front-end of ORCA was written in the mid-00s, targeting Internet Explorer, and it has the shortcomings that one would expect from that. Reliance on IE-specific functionality (e.g., `window.showModalDialog`) renders the site almost completely unusable in other browsers.

### Tightly-Coupled Front and Back Ends
There is no API layer separating the front end from the back end. This makes it quite difficult to modularize the site.

### Intermingled Design and Functionality
The front-end was created in an era when it wasn’t standard to use semantic HTML, restricting design to CSS. Instead, layout is done in the HTML itself. Most block elements are `div`s. This makes it difficult to e.g. move to a responsive design.
