
# SkillPilot AI

AI-powered career roadmap and skill guidance platform.

SkillPilot AI helps students and beginners generate personalized career learning roadmaps, track progress, explore useful courses, build projects, and prepare for interviews in a simple and beginner-friendly way.

---

## Project Description

Many students want to start learning a career skill but do not know where to begin. Online roadmaps are often too complex, confusing, or advanced for beginners.

SkillPilot AI solves this problem by creating a clear step-by-step roadmap for any career goal. Users can enter a career path such as **Data Scientist**, **Frontend Developer**, **Product Manager**, or **ML Engineer**, and the app generates a structured learning plan with beginner-friendly levels, tasks, courses, projects, skills, and interview preparation.

---

## Features

- AI-style career roadmap generation
- Beginner-friendly Level 1 and Level 2 guidance
- Step-by-step learning levels
- Progress tracking with XP system
- Saved roadmaps dashboard
- User authentication flow
- Profile page
- Course recommendations
- Project ideas for portfolio building
- Skill checklist
- Interview questions and answers
- Export roadmap as PDF
- Responsive UI for mobile, tablet, and desktop
- Toast notifications and loading states
- Clean and reusable component structure
- Supabase-ready backend integration
- Local demo mode support

---

## Screenshots

Add your screenshots inside an `images/` folder and update the paths below.

```md
![Home Page](images/home.png)
![Dashboard](images/dashboard.png)
![Roadmap Page](images/roadmap.png)
![Login Page](images/login.png)
```

---

## Tech Stack

- React.js
- TypeScript
- Vite
- Tailwind CSS
- Shadcn-style UI components
- React Router
- Framer Motion
- Lucide Icons
- Supabase-ready authentication/database
- jsPDF for PDF export

---

## Development Note

SkillPilot AI was initially planned as a MERN-style project, but it was later rebuilt using React + TypeScript with Supabase-ready backend services for cleaner architecture, faster development, and easier deployment.

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/skillpilot-ai.git
```

### 2. Go to the project folder

```bash
cd skillpilot-ai
```

### 3. Install dependencies

```bash
npm install
```

### 4. Create environment file

```bash
cp .env.example .env
```

### 5. Start the development server

```bash
npm run dev
```

---

## Environment Variables

Create a `.env` file and add the following values if you want to connect Supabase or an AI backend.

```env
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
VITE_AI_ENDPOINT=
VITE_AI_API_KEY=
```

The app also supports local demo mode, so it can run without Supabase keys for testing.

---

## Folder Structure

```bash
src/
 ├── components/
 ├── pages/
 ├── layouts/
 ├── hooks/
 ├── services/
 ├── utils/
 ├── context/
 ├── assets/
 ├── styles/
 ├── data/
 ├── routes/
 └── types/
```

---

## Usage

1. Open the app in the browser  
2. Enter a career goal  
3. Generate a roadmap  
4. Follow the learning levels step by step  
5. Track progress using the XP system  
6. Explore courses, projects, skills, and interview questions  
7. Export the roadmap as a PDF  

---

## Future Improvements

- Add real AI API integration for dynamic roadmap generation
- Add resume improvement suggestions
- Add AI interview practice
- Add admin dashboard
- Add community roadmap sharing
- Add more detailed analytics for progress tracking

---

## Author

**Jashwanth Odapelli**  
Computer Science Student

GitHub: https://github.com/jashwanthodapelli  
LinkedIn: https://www.linkedin.com/in/odapellijashwanth/

---

## License

This project is licensed under the MIT License.
