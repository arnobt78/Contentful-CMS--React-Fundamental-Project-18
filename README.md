## Contentful CMS - React Fundamental Project 17

This project demonstrates the integration of Contentful CMS with a React application. It includes a Hero section and a Projects section that fetches and displays data from Contentful.

**Online Live:**

### Installation and Setup

1. Install dependencies:
   ```sh
   npm install
   ```
2. Start the development server:
   ```sh
   npm run dev
   ```

### Project Structure

- **Hero Component**: Displays a hero section with a title and description.
- **Projects Component**: Fetches and displays projects from Contentful.

### Contentful Setup

1. Create a Contentful account and set up a space.
2. Create a content type named `cmsReactProject` with fields for `title`, `url`, and `image`.
3. Add entries to the content type.

### Environment Variables

Create a .env file in the root directory and add your Contentful API key:

```sh
VITE_API_KEY=your_contentful_api_key
```

### Fetching Data

The `useFetchProjects` custom hook in fetchProjects.jsx handles fetching data from Contentful and managing loading state.

### Additional Resources

- [Contentful](https://www.contentful.com/)
- [Undraw](https://undraw.co/) for SVG/PNG images

For more details, refer to the Project Details and Steps Section

## Project Details and Steps

### Structure

Create Hero and Projects components

### Hero Section

Setup Hero component.

### Nice SVG/PNG Images

[Undraw](https://undraw.co/)

### Data

Explore data.js

### Headless CMS

A headless CMS is a back-end only content management system that provides content creators with an intuitive interface for creating and managing content, while leaving the front-end presentation layer to be handled by a separate system or platform. This approach allows for greater flexibility and scalability, as the content can be easily distributed to multiple channels and devices, without being limited by the constraints of a particular front-end system.

### Contentful CMS

Create a Contentful CMS account

[Contentful ](https://www.contentful.com/)

#### Create Data

Setup content type and create few entries

### Explore API

Get Space ID, Access Token and explore code examples.

Space ID -
Access Token -

### Install SDK

- npm install contentful

### Get Entries

```js
import { createClient } from "contentful";

const client = createClient({
  space: "qz00uzgg3leh",
  environment: "master", // defaults to 'master' if not set
  accessToken: import.meta.env.VITE_API_KEY,
});

client
  .getEntries({ content_type: "projects" })
  .then((response) => console.log(response.items))
  .catch(console.error);
```

### Custom Hook

Create custom hook with loading and projects state values.

### Parse Data

Setup projects array

### Setup Products Component

Render data in Products component
