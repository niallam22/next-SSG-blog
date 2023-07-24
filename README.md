## Niall's SSG blog

This is a [Next.js](https://nextjs.org/) blog using SSG (static-site-generation) to improve SEO and user experience.

## Link to project: https://nialls-ssg-blog.vercel.app/
![Navigating the blog](SSG-blog.gif?raw=true "Navigating the blog")

## About this project: 
This blog is made with Next.js 13. Blog posts are statically generated from markdown files at build time this supports improved loading speed and improved SEO because the pages don't need to be rendered server side. Blog posts and their corrosponding routes are dynamicall generated which means new posts can be easily created without needing to configure new routes and pages each time.

# Tech used: 
> Typescript,
> React,
> Next.js 13,
> Tailwind CSS

## How it's made:
1. The home route contains links to dynamically generated routes to blog posts so that new blog posts can be added by creating new markdown files in the blog post directory and be automatically rendered.
2. getStaticParams is used to pre-fetch the blog posts so that the routes can be rendered SSG at build time rather than at request, server-side-rendering (SSR). This improves speed and SEO. 
3. Post params are used to dynamically generate page meta data related to the articles to support SEO.
4. The site is responsive and mobile friendly and has been styled with Tailwind.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
