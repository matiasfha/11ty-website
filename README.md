<p align="center"><img src="https://www.11ty.dev/img/logo-github.svg" width="200" height="200" alt="eleventy Logo"></p>

# 11ty.dev 🕚⚡️🎈🐀

* https://www.11ty.dev/

The website and documentation for the [Eleventy static site generator](https://github.com/11ty/eleventy/).

## Running Locally

```
npm install
npm run get-new-data
npx @11ty/eleventy --serve
```

Browse to http://localhost:8080/ (8080 is the default but it’ll bump to a new port if that one is taken, so use whatever port shows up when you run the `--serve` command).

* Refresh Supporters: `npm run get-new-supporters`

## How to Use

This is the official website and documentation for Eleventy (11ty), a simple static site generator. Here's how to use it:

### Development
1. **Start the development server**: Run `npm start` to start the development server with hot-reload on port 8091
2. **Browse locally**: Open your browser to http://localhost:8091/ (or the port shown in the console)
3. **Make changes**: Edit files in the `src/` directory and see changes reflected in real-time

### Building
* **Development build**: Run `npm run build` to create a production-ready build in the `_site` directory
* **Production build**: Run `npm run build-production` to fetch fresh data and create an optimized production build

### Useful Commands
* `npm run get-new-data` - Fetch the latest community projects and data
* `npm run create-search-index` - Generate the search index for the site
* `npm run check-links` - Verify all internal links are working
* `npm run format` - Format code using Prettier

### Project Structure
* `/src` - Source files for the website
* `/_site` - Generated static site (created after build)
* `/config` - Eleventy configuration files
* `/.eleventy.js` - Main Eleventy configuration

For more information about Eleventy itself, visit [the documentation](https://www.11ty.dev/docs/).

## Third-party Integrations

* [IFTTT](https://ifttt.com/) daily web hook to build the site once a day to update stats and counts in footer.
* [Zapier](https://zapier.com/) (Open Collective + Netlify integration) to run a new production build when a new contributor joins Open Collective. _Warning: while avatar will show on the site, there is still a manual step to send the Netlify Identity invitation for the Eleventy Contributor Account._
