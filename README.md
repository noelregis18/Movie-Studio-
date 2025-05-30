# MovieStudioYT

A modern movie browsing application built with Next.js, featuring a beautiful UI with dark/light mode, movie listings by categories, search functionality, and detailed movie information.

![MovieStudioYT Screenshot](https://via.placeholder.com/800x400?text=MovieStudioYT+Screenshot)

## Features

- **Movie Categories**: Browse movies by Now Playing, Upcoming, Top Rated, and Popular
- **Movie Details**: View detailed information about each movie
- **Search Functionality**: Search for movies by title or keywords
- **Genre Filtering**: Filter movies by genre
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Dark/Light Mode**: Toggle between dark and light themes
- **Carousel Banner**: Featured movies showcase with auto-scrolling
- **Video Player**: Watch movie trailers directly in the app

## Tech Stack

- **Framework**: [Next.js 14](https://nextjs.org/) with App Router
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **UI Components**: Custom components with [Radix UI](https://www.radix-ui.com/)
- **Carousel**: [Embla Carousel](https://www.embla-carousel.com/)
- **Video Player**: [React YouTube](https://github.com/tjallingt/react-youtube)
- **Form Handling**: [React Hook Form](https://react-hook-form.com/) with [Zod](https://github.com/colinhacks/zod) validation
- **Theming**: [Next Themes](https://github.com/pacocoursey/next-themes)
- **API**: [The Movie Database (TMDB) API](https://www.themoviedb.org/documentation/api)

## Getting Started

### Prerequisites

- Node.js 18.x or later
- TMDB API Key (get it from [TMDB](https://www.themoviedb.org/settings/api))

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/moviestudioyt.git
   cd moviestudioyt
   ```

2. Install dependencies
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. Set up environment variables
   - Create a `.env.local` file in the root directory
   - Add your TMDB API key and access token
   ```
   NEXT_URL=http://localhost:3000/
   TMDB_API_KEY=your_tmdb_api_key
   TMDB_READ_ACCESS_KEY=your_tmdb_read_access_token
   ```

4. Start the development server
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the application

## Project Structure

```
├── public/              # Static assets
├── src/
│   ├── app/             # App router pages
│   │   ├── genre/       # Genre filtering pages
│   │   ├── movie/       # Movie details pages
│   │   ├── search/      # Search results pages
│   │   └── viewmore/    # View more movies pages
│   ├── components/      # React components
│   │   └── ui/          # UI components
│   └── lib/             # Utility functions
└── type.ts             # TypeScript type definitions
```

## API Integration

This project uses The Movie Database (TMDB) API to fetch movie data. The API calls are implemented in `src/lib/getMovies.ts` and include:

- Now Playing movies
- Upcoming movies
- Top Rated movies
- Popular movies
- Movie search
- Movie details

## Deployment

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out the [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the API
- [Next.js](https://nextjs.org/) for the amazing framework
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
