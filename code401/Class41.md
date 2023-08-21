# Reading Questions Class 41

## Explain the concept of dynamic routes in Next.js and how they differ from static routes.

Dynamic routes in Next.js enable creating pages with variable URL segments, allowing a single component to handle multiple URLs. For instance, a blog post page can use dynamic routes to show various posts. Static routes involve separate files for each route and are suitable for pages without dynamic content.

## Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?

Deploying a Next.js app involves building it, choosing a platform (Vercel, Netlify, AWS Amplify), connecting the repo, configuring build settings, and triggering deployment. Platforms like Vercel offer seamless integration and automatic deployments, while Netlify provides easy hosting and CI/CD. AWS Amplify combines hosting with serverless backend capabilities.

## How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.

Next.js serves static files from the public directory, storing assets like images. You can directly reference them using /filename.ext. Additionally, referencing assets in the head section for things like styles is possible using the same approach, enhancing optimization and performance.


