This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/zeit/next.js/tree/canary/packages/create-next-app).

## Getting Started

Install all the dependencies

## npm install

Running the development server:

## npm run dev

Open [http://localhost:5003](http://localhost:5003) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

## Steps to publish your gh-pages

### * Install below libraries:

npm install rimraf --save-dev
npm install gh-pages --save-dev
npm install babel-plugin-transform-define --save-dev

### * Add below commands under scripts:

scripts: {
    "export": "next export",
    "deploy": "rm -rf node_modules/.cache && rimraf out && next build && next export && touch out/.nojekyll && gh-pages -d out -t true"
}

### npm run deploy

Command to deploy and Publish your gh-pages

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/zeit/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/import?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
