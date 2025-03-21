# University Registration System

## What is this project?
This is a web app for university students and admins to manage course registrations. Students can:
- Log in with their roll number.
- See available courses and register for them.
- Check their schedule and remove courses.
- Subscribe to full courses and get notified when seats are available.

Admins can:
- Log in with a username and password.
- Add, update, or delete courses.
- See all student registrations and remove them if needed.
- Override registrations to add students to full courses.

## How to Set Up the Project
Follow these steps to run the project on your computer:

1. **Clone the Repository**  
   Copy this project to your computer by running this command in your terminal:
git clone https://github.com/your-username/UniversityRegistrationSystem.git
(Replace `your-username` with your GitHub username.)

2. **Go to the Project Folder**  
Move to the project folder by running:
cd UniversityRegistrationSystem

3. **Install Required Packages**  
This project uses Node.js. Install the needed packages by running:
npm install


4. **Set Up MongoDB**  
- Make sure MongoDB is installed on your computer and running.
- The app connects to a local MongoDB database called `studentRegistration`.

5. **Create a `.env` File**  
- In the project folder, create a file named `.env`.
- Add these lines to the `.env` file:
PORT=3000
MONGODB_URI=mongodb://localhost:27017/studentRegistration

Copy
- This tells the app which port to use and where to find the MongoDB database.

6. **Add Sample Data (Optional)**  
- To add some sample students and courses to the database, run:
npm run seed

Copy
- This will add a few students (roll numbers: `12345`, `67890`) and courses (like "Introduction to Programming").

7. **Start the App**  
Run this command to start the app:
npm start

Copy
- The app will start on `http://localhost:3000`. Open this link in your browser.

## How to Use the App
- **For Students**:
1. On the homepage, click "Student Login".
2. Enter your roll number (e.g., `12345` or `67890`).
3. You can see available courses, register for them, and check your schedule.
4. If a course is full, click "Subscribe" to get a notification when a seat is available.

- **For Admins**:
1. On the homepage, click "Admin Login".
2. Use username: `admin` and password: `admin123`.
3. You can add, update, or delete courses.
4. You can see all student registrations and remove them.
5. Use the "Override Registration" section to add a student to a full course by entering their roll number and the course name.

## Project Files
- `server.js`: The main file that runs the app and handles all requests.
- `models/`: Contains the database models for students and courses.
- `public/`: Contains the CSS and JavaScript files for the website.
- `views/`: Contains the HTML pages for the website.
- `seed.js`: Adds sample data to the database.
- `.env`: Stores settings like the port and database URL (don’t share this file!).

## Tools Used
- **Node.js**: To run the app.
- **Express**: To create the web server.
- **MongoDB**: To store data about students and courses.
- **Mongoose**: To work with MongoDB easily.
- **dotenv**: To manage settings in the `.env` file.

## Need Help?
If you have any questions or problems, feel free to open an issue on this GitHub repository, and I’ll help you!

---

**Made by [Abdullah]**
