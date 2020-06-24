Table of Contents demo for Ezhil theme
---

The Ezhil theme for Hugo seems to do something that interferes with the process of generating a table of contents. When you generate a toc, the links do not contain the path to the page; they are all anchor links off the root of the site. Switching themes to something like ananke results in the correct toc generation behavior.

This is a quick demo project to show this behavior:

- Clone or download this project.
- Start the server with the ezhil theme:
  - `hugo serve -D --port=1221 -t ezhil`
  - Click the link to the test post, and look at the toc. The last anchor link is: `http://localhost:1221/#great-point-3`
- Start the server with the ananke theme:
  - `hugo serve -D --port=1221 -t ananke`
  - Click the link to the test post, and look at the toc. The last anchor link is: `http://localhost:1221/posts/my_test_toc_post/#great-point-3`

What is happening in the ezhil theme that is interfering with the correct generation of the toc?