### About
[Watchtower](https://internetdemocracy.in/watchtower/) provides an overview of Indian government bodies that work on information security (or infosec).

![Imgur](http://i.imgur.com/E2FgxYG.jpg)

### Architecture
Watchtower is built as a web application built with HTML5, CSS, JavaScript, and is backed by a single data source, a [Google Sheet](https://docs.google.com/spreadsheets/d/1t_7K7Asg92NXmt9EDxvrQFYdy1w7XWMsft2xJTRTo8M/edit?usp=sharing).
Watchtower also relies on a few open source libraries which are detailed below. Watchtower itself, is [open source](https://github.com/InetDemocracyProject/watchtower/blob/gh-pages/LICENSE).

Watchtower mainly consists of the following components:
1. A sidebar that provides an overview of the project. It also serves to show contextual information, such as government body's details when it's clicked on.
2. A map of India's government bodies working on infosec.
3. A widget to filter the bodies in the visualization based on some criterion.

### Dependencies

1. [vis.js](http://visjs.org/) is used to render the map.
2. [ractive.js](http://www.ractivejs.org/) is used to render and dynamically update the components on the page.
3. [jQuery](https://jquery.com/) for basic DOM manipulation.
4. [Bootstrap](http://getbootstrap.com/css/) for CSS grids and components.
5. [tabletop](https://github.com/jsoma/tabletop) to import data from the Google Sheet.

### Workflow

When a user loads [watchtower](https://github.com/InetDemocracyProject/watchtower), the data from the Google Sheet is imported into the page. This data is processed and is used to render the components on the page. 
