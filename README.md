# Hacker News Reader
### Smart.bid Front-end Interview Assignment

[Hacker News](https://news.ycombinator.com) is a discussion board website for programmers and tech entrepreneurs. Despite its popularity, its user interface is astoundingly basic and outdated.

The goal of this task is to (somewhat) fix it by building a modern single-page-application for consuming content from Hacker News, using their [official API](https://github.com/HackerNews/API).

> Tip: Consider using the
> [node-hn-api](https://github.com/arjunsajeev/node-hn-api) Hacker News
> API wrapper library. it's compatible with browsers too (despite its
> name).

## Requirements
- **Javascript:** It's preferred to use React, but use any libraries, frameworks and tools of your choice.
- Your project should be well structured and organized, your code should be clean.
- It should be easy to run your web app.
- Visual design files of the our desired web app are provided in this repository (links below). Your product should visually match these files to a large extent. Use the color reference and the listed resources below. Dimensions, spacing and font sizes are not expected to perfectly match.
 
### Part 1: Homepage
 Design: [default state](https://raw.githubusercontent.com/ewebdev/hackernews-fed-assignment/master/1-homepage.png), [link hover](https://raw.githubusercontent.com/ewebdev/hackernews-fed-assignment/master/1-homepage-link-hover.png)
 1. The homepage of our web app should load and display the top 10 Hacker News stories.
 2. Each story in our web app should consists of: its posting time, author name, title, URL (in most stories), score and number of comments (threads) -- You can find these all in the API docs. In addition, we would like to emphasize stories with high traction with a orange flame icon. You should consider stories with score higher than 100 or stories with at least 25 comments (threads). 
 3. Clicking on a URL in a story should open it by-default in a new browser tab.
 4. A fixed navigation bar with just the the letter "Y" as the logo at the top-left corner.
 5. **Bonus:** Add a loading indicator.
 6. **Bonus:** Adapt the website for smaller screens (mobile devices).
 7. **Bonus:** Add an in-app caching mechanism for better user experience.
 
### Part 2: Story Page
  Design: [full page](https://raw.githubusercontent.com/ewebdev/hackernews-fed-assignment/master/2-story-page.png)
 1. Clicking on any part of a story item in the homepage, other than the story URL, should lead to a story page where's the full comments of the story are loaded and displayed.
 2. Comments on Hacker News are multi-level hierarchical, make sure to load and display the full comments tree (it may involve numerous requests).
 3. This page should have its own URL and it should include the ID of the story. Remember we're building a single-page-application, so client-side routing is required.
 4. Clicking on the logo in the navbar should navigate to the homepage. 
 5. **Bonus:** Add a loading indicator for the comments, with a real-time counter of the fetched comments.

### Colors
 - Orange: #ff6600
 - Page light-grey background: #f7f7f7
 - Text black-ish: #3e3e3e
 - Icons grey: #c5c5c5

### Resources
 - [Google Material Icons](http://google.github.io/material-design-icons/) -- The icons you should be using are: "comment", "thumb up", "whatshot", "link", "account circle".
- ["Lato" web font](https://fonts.google.com/selection?query=lato&selection.family=Lato:400,700) -- Lato is the font that's being used in the designs.
- [Hacker News - Homepage](https://news.ycombinator.com)
- [Hacker News - Official API](https://github.com/HackerNews/API)
- [node-hn-api (npm package)](https://github.com/arjunsajeev/node-hn-api) -- A promise based wrapper for official Hacker News API.