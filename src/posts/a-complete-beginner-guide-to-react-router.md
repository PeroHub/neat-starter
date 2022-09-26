---
author: Peter
thumbnail: /static/img/276235076_1109454279840248_153228080995940830_n.jpg
imageAlt: A man on laptop
title: A Complete Beginner Guide To React Router
description: Understand the fundamentals on routing in React in 5 minutes.
date: 2022-09-21T12:18:14.657Z
tags:
  - created
image: /static/img/276235076_1109454279840248_153228080995940830_n.jpg
---
# Introduction

Routing hhhhh is the ability to move between different parts of an application when a user enters a URL or clicks an element (link, button, icon etc) within the application.

> React Router is a standard library for routing in React.

It enables the navigation among views of various components in a React Application.

This popular library has three (3) variants:

* **react router:** the core library.
* **react-router-dom:** a variant of the core library meant to be used for web applications.
* **react-router-native:** a variant of the core library used with react native in the development of Android and iOS applications.

# [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-prerequisites "Permalink")Prerequisites

To run the examples in this article, be sure to have some or all of the following.

* **The Node runtime environment -** Install Node for your operating system from the Node [downloads page.](https://nodejs.org/en/download/)
* **A React project:** Quickly create a React project.

COPY

COPY

```

```

# [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-how-to-set-up-react-router "Permalink")How To Set Up React Router

The scope of this article is in the realm of web applications so we can safely choose react-router-dom. This library is installed in a project by running the command below in the project directory.

COPY

COPY

```

```

# [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-adding-react-router-components "Permalink")Adding React Router Components

There are four (4) **main** components in the react router library.

#### [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-browserrouter "Permalink")BrowserRouter

It is used for applications which have a dynamic server that knows how to handle any type of URL. It is the parent component that is used to store all of the other components.\
In your index.js file, import the **BrowserRouter** component and wrap it over your **App.js** component as shown below.

COPY

COPY

```

```

#### [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-routes "Permalink")Routes

Whenever the location changes, Routes looks through all its child routes to find the best match and renders that branch of the UI. It’s a new component introduced in **React Router version 6** and an upgrade of the component.

COPY

COPY

```

```

The main advantages of Routes over Switch is...

> Routes are chosen based on the best match instead of being traversed in order.

#### [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-route "Permalink")Route

It is one of the most important building blocks in the React Router package. It is the conditionally shown component that renders some UI when its path matches the current URL. It renders the appropriate user interface when the current location matches the route’s path.\
The **path** is a prop on the **Route** component that describes the **pathname** that the route should match.\
The **element** is a prop on the **Route** component that describes the **Component** that would be displayed when the path matches the route.

COPY

COPY

```

```

In your App.js, import **Route** and **Routes** component from your **react-router-dom** library package installed earlier on as shown below.

COPY

COPY

```
reertetrertererererererr
```

##### [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-folder-structure "Permalink")Folder Structure

In your project directory, create a folder named **component** inside the src folder and now add 3 files named **home.js**, **about.js** and **contact.js** to the component folder.

![Screenshot 2022-09-20 at 11.37.35.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1663671876107/fjg93lmfH.png?auto=compress,format&format=webp)

Okay... looks good already.

Let's add some content to each file we've created.

> Home.js file

COPY

COPY

```

```

> About.js file

COPY

COPY

```

```

> Contact.js file

COPY

COPY

```

```

In your App.js file, import the files you just created and add the paths as shown below.

COPY

COPY

```javascript
const let
```

#### [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-link "Permalink")Link

The react-router package also contains a component that is used to navigate the different parts of an application by way of hyperlinks. Link component uses the **to** prop to describe the location where the links should navigate to.

COPY

COPY

```

```

It is similar to HTML’s anchor element `(<a> </a>)` but the main difference is that using the Link component does not reload the page but rather, changes the UI. Using an anchor tag would require that the page is reloaded in order to load the new UI. When the Link component is clicked, it also updates the URL.

Let's see how it works. In your App.js file, import add the **Link** component. This should link the various components to their specific routes as shown below.

COPY

COPY

```

```

Run **npm start** on your terminal... You should have your app running and links to various routes as should below.

![Screenshot 2022-09-20 at 12.44.53.png](/static/img/276235076_1109454279840248_153228080995940830_n.jpg "peter")

# [](https://paulkeno.hashnode.dev/a-complete-beginner-guide-to-react-router#heading-conclusion "Permalink")Conclusion

This brings us to the end of the article. Kudos to you if you made it this far.nReact Router is an awesome library that helps us go from a single page to a multi-page application feeling with great usability. (Just keep in mind – at the end of the day, it's still a single page app[(SPA)](https://developer.mozilla.org/en-US/docs/Glossary/SPA)).