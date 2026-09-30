# AttendEase – Faculty Attendance Portal

A responsive React + Vite Student Attendance Tracker for Task 2.

## Main features
- Dashboard with attendance statistics and low-attendance students.
- Student add, edit, delete and search.
- Faculty Schedule with class-wise subject, room, faculty name and Faculty ID.
- Automatic Morning / Afternoon / Evening label based on the current time.
- Date-wise attendance records using the current date.
- Faculty ID verification before attendance can be entered.
- Attendance is unlocked only when the current day and time match the scheduled class.
- Prevents duplicate attendance submission for the same date, class period and faculty.
- Reports include cumulative student percentages and date-wise faculty sessions.
- Data is stored in browser LocalStorage.

## Run locally
```bash
npm install
npm run dev
```

For Windows PowerShell when script execution is restricted:
```powershell
npm.cmd install
npm.cmd run dev
```

## Production build
```powershell
npm.cmd run build
```

Deploy the generated `dist` folder to Cloudflare Pages using Wrangler:
```powershell
npx.cmd wrangler login
npx.cmd wrangler pages deploy dist
```

## Demo Faculty IDs
The sample timetable includes IDs such as `FAC101`, `FAC102`, `FAC103`, etc. Edit the `schedules` array in `src/App.jsx` to match your real faculty IDs, classes and timetable.
