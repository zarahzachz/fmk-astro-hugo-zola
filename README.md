# FMK: Astro, Hugo, and Zola

A personal experiment where I create and compare a simple blog built with Astro, Hugo, and Zola.

The following parameters will be explored as part of this experiement:

- To get a feel for the Markdown parsing, each build will make use of the same content (mostly from `/original-content`)
- To get a feel for project organization and maintenence, each build will have at least two templates
  - Homepage view has list of all content, filterable
  - Single page view is the individual url for each piece of content
- To see how extendable the Markdown content can be, each build will have at least one a reusable component in a Markdown file
  - Just for simplicity, this will be an alert component
- To see if adding CSS is hard and to experiment with each build's CSS capabilities, basic styling will be added to control layout (for mobile and desktop)
- To test how easy it is to use JS (e.g., minification, treeshaking, etc.), each build will have a "filter content" feature to sort content by tag and/or content type
- **Stretch goal:** To get a feel for built-in functionality, each build will implement 5 posts and notes per page pagination

I'll grade how each SSG performs based on the "How much did doing this piss me off?" scale (🤩, 😎, 😐, 😠, or 🤬).

## Astro

To run the project locally, `cd astro` and run `npm run dev` (assuming everything's been installed).

Report card:

| Subject                | Grade |
| ---------------------- | ----- |
| Markdown               | 😠    |
| Templates              | 😐    |
| Shortcodes             | -     |
| CSS                    | 😎    |
| JS                     | -     |
| Built-in functionality | -     |

Questions:

1. Why does Astro have a dozen different ways to grab content from a file? Do I use Fragment? Glob? Content? Slot? Collections? I spent a few hours trying to accomplish what I thought was a simple thing. This can definitely be chalked up to me being new to Astro, but it was still a giant pain in the ass, espcially when other SSG have simple `<Content>` tags you can use and it just works.
2. Is there an easier way to define a template for a set of pages? I think I've seen other SSG with a config or data file you can add to a page group's directory and it let's you bulk edit the content in that folder. I can't find anything like this in the docs, but that doesn't mean it doesn't exist. If it doesn't, this is a very annoying oversight.

## Hugo

Report card:

| Subject                | Grade | Notes |
| ---------------------- | ----- | ----- |
| Markdown               | -     | -     |
| Templates              | -     | -     |
| Shortcodes             | -     | -     |
| CSS                    | -     | -     |
| JS                     | -     | -     |
| Built-in functionality | -     | -     |

## Zola

Report card:

| Subject                | Grade | Notes |
| ---------------------- | ----- | ----- |
| Markdown               | -     | -     |
| Templates              | -     | -     |
| Shortcodes             | -     | -     |
| CSS                    | -     | -     |
| JS                     | -     | -     |
| Built-in functionality | -     | -     |
