# College-Connect
The social network for college students.

## Configuration
### Step 1. Create an account and a project in GraphCMS
First, [create an account in GraphCMS](https://app.graphcms.com).

### Step 2. Create a new GraphCMS project
After creating an account, create a new project from the **Blog Starter template** - be sure to include the example content.

### Step 3. Set up environment variables
Copy the `.env.local.example` file in this directory to `.env.local` (which will be ignored by Git):

```bash
cp .env.local.example .env.local
```

Inside your project dashboard, navigate to **Settings > API Access page**.

Then set each variable in `.env.local`:

- `GRAPHCMS_PROJECT_API`: Set it to the API endpoint under **Endpoints**, at the top of the page.
- `GRAPHCMS_PROD_AUTH_TOKEN`: Copy the `NEXT_EXAMPLE_CMS_GCMS_PROD_AUTH_TOKEN` token under **Existing tokens**, at the bottom of the page. This will only query content that is published.
- `GRAPHCMS_DEV_AUTH_TOKEN`: Copy the `NEXT_EXAMPLE_CMS_GCMS_DEV_AUTH_TOKEN` token under **Existing tokens**, at the bottom of the page. This will only query content that is in draft.
- `GRAPHCMS_PREVIEW_SECRET` can be any random string (but avoid spaces), like `MY_SECRET` - this is used for [Preview Mode](https://nextjs.org/docs/advanced-features/preview-mode).

### Step 4. Run Next.js in development mode
```bash
npm install
npm run dev

# or

yarn install
yarn dev
```

The app should be up and running on [http://localhost:3000](http://localhost:3000)!
