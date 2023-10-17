# X-Synergy Project Readme

This repository contains the source code and project structure for building the Social media application akin to X using Next.js 13, Tailwind CSS, TypeScript, and Supabase. The project is organized into multiple directories and files, each contributing to various components and functionalities of the Social Media app.

## Directory Structure

- **drizzle/**: Contains SQL files for database schema and metadata.
- **public/**: Includes static assets such as SVG icons.
- **src/**: Contains the main source code for the X-Synergy .
  - **app/**: Application-related code, including user-specific pages.
  - **components/**: Reusable components used in the project.
  - **lib/**: Library and utility code.

## Configuration Files

- **next.config.js**: Configuration for Next.js.
- **postcss.config.js**: Configuration for PostCSS.
- **tailwind.config.js**: Tailwind CSS configuration.
- **tsconfig.json**: TypeScript configuration.

## Database Schema

The `drizzle` directory contains SQL files representing the PostgreSQL database schema. The `meta/` directory contains metadata for the schema evolution.

## Application Code

### `src/app/`

- **`[username]/`**: User-specific pages and components.
  - **`page.tsx`**: User-specific page component.

### `src/app/tweet/`

- **`[id]/`**: Tweet-specific pages and components.
  - **`page.tsx`**: Tweet-specific page component.

### `src/components/`

- **`client-components/`**: Client-side components.
  - Various components for composing tweets, like buttons, profile avatars, and reply dialogs.
- **`server-components/`**: Server-side components.
  - Components related to server-rendered content.
- **`ui/`**: User interface components.
  - Components for avatars, buttons, dialogs, and inputs.

### `src/lib/`

- **`db/`**: Database-related code, including migration and schema management.
- **`supabase/`**: Supabase-related code, including mutations and queries.
- **`utils.ts`**: Utility functions.

## Key Features

- **Dynamic User Interface**: Experience a dynamic and interactive UI designed for engaging user interactions and smooth navigation.

- **Responsive Design**: The project is designed to adapt seamlessly to various screen sizes and devices, ensuring a consistent and enjoyable user experience.

- **Real-time Updates**: Implemented real-time updates to keep users informed about likes, replies, and other interactions, enhancing project interactivity.

- **Secure User Authentication**: Implementation of secure and robust user authentication within the project, prioritizing data protection and user privacy.

- **Optimized Database Schema**: Utilizing a optimized PostgreSQL database schema, ensuring efficient handling of tweet-related data and improved performance within the project.

- **Comprehensive Tweet Functionality**: Capability to create, like, and reply to tweets, providing a comprehensive user experience centered around tweet interactions.

## Usage

Follow these steps to set up and use the X-Synergy application:

1. **Generating Types for Tables (Pre-Authentication)**:

   Before proceeding with authentication, it's essential to generate types for the database tables using Supabase. Follow these steps:

   - **Log in to Supabase CLI**:

     Run the following command to log in to Supabase using Supabase CLI:

     ```bash
     npx supabase login
     ```

   - **Generate Types**:

     Use the following command to generate types for your tables in TypeScript. Replace `--project-id` with your actual Supabase project ID:

     ```bash
     npx supabase gen types typescript --project-id <your-project-id> --schema public > types/supabase.ts
     ```

     This command will generate TypeScript types for your database tables and save them in the `types/supabase.ts` file.

2. **Authentication**:

   Proceed with the authentication setup as described in the main section of the readme.

These steps ensure that you have the necessary types generated for your database tables before setting up authentication for the application.

## Contributing

Contributions to enhance or extend the X-Synergy project are welcome! Feel free to open issues, submit pull requests, or provide feedback on the project.

## Acknowledgements

Special thanks to the creators and instructors of the technologies used in this project.

---
