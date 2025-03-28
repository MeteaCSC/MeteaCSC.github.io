# NOTE:
This is not the original MVCS website. It is built using astro, so if you would like to contribute, make sure to reference the documentation below:

[Astro docs](https://docs.astro.build/en/getting-started/)

- Understand how astro components work in pages
- Understand how astro layouts work with slots

# The Metea Valley CSC Website

The website where our club posts all sorts of important recources such as meeting plans and general club information for the world to see.

# Contributing

We are always happy for someone to share their ideas for how the website, but we just require 2 things

1) Keep it school appropriate 
2) Anything new that is added must pass the build tests before changes can be pushed to cloudflare (WIP)

If you are unfamiliar with version control I suggest you check out how to make a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) and learn the basics of [git](https://www.w3schools.com/git/git_intro.asp?remote=github). Nequa also has a pretty good guide on their [repo](https://github.com/NVComputing/nvcomputingsite).
## Setup

#### GOOGLE IS YOUR FRIEND. If you ever have a question about something, someone online has probally answered it. Look farther than just the first search result.

Make sure that you have npm, git, and Node.js installed, otherwise, you won't be able to run the website or commit changes.

The setup for this project may be changing a lot, so it might be good to check this every so often until we get Cloudflare integration working.

Download the dependencies by running:

```bash
npm install
```

Then to start the express server on port 4321 type of respective commands into the terminal:

Linux

```bash
npm run dev
```

Windows/MacOS
```bash
not sure yet but check the astro docs
```


Now go to http://localhost:4321/ in your favorite web brower to view the website!

## Project Structure

```bash
── public # this is where non-code is stored
   ├── fonts # want more fonts? put the ttf files here
   ├── images # any and all images go here
   ├── style # add your css files here, the file paths when imported should be "/public/style/your-style.css"
── src                 
   ├── assets           # just some svgs
   ├── components       # want to edit things like the navbar, footer, head and header? check out the components located here
   ├── layouts          # standard formats for pages (astro layouts) are here
   └── pages            # EJS/HTML
       └── markdown     # Site wide resources (ex navbar/footer)

```

## Adding new resources

### Calendar
In the root directory there should be a file called `dates.json` where you can add any new events. 

An example for how this should look is:
```json
{
    "date": "2024-09-12",
    "name": "Activity Fair",
    "timeStart": 0,         // Ignore this since its a whole day thing
    "timeEnd": 0            // Also the calendar doesn't support times (yet)
}
```

### Weekly slides

TODO

### Leaderboards

TODO