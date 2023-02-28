# Lotion
Lotion is a simple and lightweight blogging engine that uses Notion.so as a CMS.

## Features
Easy to use and customize
Posts and pages are managed in Notion, giving you a familiar and powerful interface for content creation and management
Uses Notion's powerful database features to allow for flexible categorization and organization of content
Built-in support for Markdown formatting
Automatic generation of RSS feed and sitemap
SEO-friendly URLs


## Installation and setup
To get started with Lotion, you'll need a Notion account and an API key. You can get your API key by following these instructions.

Once you have your API key, you'll need to set up a Notion database to hold your blog posts and pages. You can use the example database provided with Lotion as a starting point.

Next, clone the Lotion repository and install its dependencies:

```sh
git clone https://github.com/username/lotion.git
cd lotion
npm install
```
Copy the .env.example file to .env and fill in your Notion API key and database ID:

```sh
cp .env.example .env
```

```makefile
NOTION_API_KEY=your-notion-api-key
NOTION_DATABASE_ID=your-notion-database-id
```
Finally, start the development server:

```sh
npm run dev
```

## Usage
Lotion is designed to be easy to use and customize. All posts and pages are managed in Notion, so you can use its familiar interface to create and edit content.

To create a new post, simply add a new row to the "Posts" table in your Notion database. The "Title" column will be used as the title of the post, and the "Content" column should contain the Markdown-formatted content of the post.

To create a new page, add a new row to the "Pages" table in your Notion database. The "Title" column will be used as the title of the page, and the "Content" column should contain the Markdown-formatted content of the page.

To customize the appearance of your blog, you can edit the CSS and templates in the src directory.

## Deployment
To deploy Lotion to a production server, you can build the project and serve the generated files using a static file server like NGINX or Apache.

To build the project, run:

```sh
npm run build
```

This will generate the static files in the out directory. You can then serve these files using your preferred web server.

## License
Lotion is released under the MIT License.
