# MediQueue Client

MediQueue is a production-ready tutoring and booking platform for students, tutors, and facility owners. This repository contains the Next.js frontend that powers the public marketplace, authentication flow, tutor browsing, and booking experience.

## Live Links
- Website: https://mediqueue-client.vercel.app/
- Server API: https://mediqueue-s-2e8c.onrender.com/api

## Project Overview
MediQueue connects students with qualified tutors and provides a clean, responsive interface for discovering experts, managing sessions, and exploring learning opportunities. The frontend is built with Next.js 16, React 18, Tailwind CSS, and Better Auth to deliver a polished portfolio-ready experience.

## Key Features
- Secure sign-in and registration flow
- Tutor discovery, profile browsing, and booking details
- Role-aware dashboard access for students and tutors
- Protected routes and session-aware UI
- Dark/light theme support
- Responsive, production-ready frontend design

## User Roles
- Student: browse tutors, view sessions, book learning support
- Tutor: manage profile, availability, and teaching offerings
- Facility Owner: list and manage available spaces or resources

## Technology Stack
### Frontend Technologies
- Next.js 16
- React 18
- Tailwind CSS
- Framer Motion
- Lucide Icons
- React Hook Form

### Backend Technologies
- Express.js
- MongoDB + Mongoose
- Better Auth
- JWT / cookie-based session handling

### Database Technologies
- MongoDB Atlas

### Authentication System
- Better Auth
- Google OAuth (optional integration)
- Protected API routes with session validation

## API Overview
This client communicates with the backend API hosted at the live Render service above. The main areas include:
- `/api/auth`
- `/api/tutors`
- `/api/bookings`
- `/api/facilities`

## Installation Guide
```bash
cd Client
npm install
npm run dev
```

## Environment Variables Guide
Create a `.env.local` file in the `Client/` folder:
```env
NEXT_PUBLIC_API_URL=http://localhost:5000/api
NEXT_PUBLIC_BETTER_AUTH_URL=http://localhost:3000
BETTER_AUTH_SECRET=your_better_auth_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

## Local Development Setup
1. Start the backend API from the `server/` directory.
2. Run `npm install` in `Client/`.
3. Create `.env.local` with the variables above.
4. Launch the frontend with `npm run dev`.

## Folder Structure
```text
Client/
├── src/
│   ├── app/            # App routes and pages
│   ├── components/     # Reusable UI components
│   ├── context/        # Auth and theme providers
│   ├── lib/            # Auth helpers and utilities
│   └── styles/         # Global styling
├── public/             # Static assets
├── package.json
├── README.md
└── next.config.mjs
```

## Deployment Information
- Frontend hosting: Vercel
- Backend hosting: Render
- Production URL: https://mediqueue-client.vercel.app/
- API URL: https://mediqueue-s-2e8c.onrender.com/api

## Screenshots
Placeholder for portfolio screenshots:
- Home page hero and tutor discovery view
- Tutor details and booking interface
- Dashboard and session management flow

## Future Improvements
- Add admin-facing analytics dashboard
- Introduce review and rating system for tutors
- Expand booking notifications and reminders
- Improve accessibility and performance audits

## Troubleshooting Guide
- If the app does not load, confirm the backend is running and `NEXT_PUBLIC_API_URL` is correct.
- If authentication fails, verify `BETTER_AUTH_SECRET`, `GOOGLE_CLIENT_ID`, and `GOOGLE_CLIENT_SECRET`.
- If the build fails, run `npm run lint` and `npm run build` to identify issues.

## Contributing
Contributions are welcome. Please open an issue or submit a pull request with clear documentation for any changes.

## License
This project is distributed under the MIT license.

## Contact
- Email: narayon231206@gmail.com
- GitHub: https://github.com/narayon231206
- Portfolio-ready repository: MediQueue
