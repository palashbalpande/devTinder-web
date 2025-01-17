# DevTinder

- Created a Vite + React app
- Remove unnecessary code & create a hello world app
- Install Tailwind CSS
- Install DaisyUI
- Add Navbar component to App.jsx
- Create a Navbar.jsx separate component file
- Install react router dom
- Create BrowserRouter > Routes > Route=/ Body > RouteChildren
- Create an Outlet in your Body component
- Create a Footer
- Create a Login page
- Install axios
- CORS - install CORS in backend => add middleware to app with configurations: origins, credentials: true {app.use(cors());}
- Whenever you're making API calls so pass axios => { withCredentials: true }
- Install react-redux + @reduxjs/toolkit => configureStore => Provider => createSlice => add reducer to store
- Add redux devtools in chrome
- Login & check if your data is coming properly in the store
- Navbar should update as soon as user logs in
- Refactor our code to add constants file
- You should not be able to access other routes without login 
- If token is not present, redirect to login page
- Logout Feature
- Get the feed and add the feed on the store
- build the user card on feed
- Edit Profile Feature
- Show Toast Message on profile updates
- New Page - See all my connections
- New Page - See all my connection Requests
- Feature - Accept/Reject Connection Request
- Send/Ignore the user card from the feed
- Signup New User
- E2E testing

Body 
    Navbar
    Route=/ => Feed
    Route=/login => Login
    Route=/connections => Connections
    Router=/profile => Profile

# Deplyment

- Signup on AWS
- Launch instance
- chmod 400 <secret-key-file-name>.pem
- ssh -i "devTinder-secret.pem" ubuntu@ec2-52-66-236-12.ap-south-1.compute.amazonaws.com
- Install Node version 20.15.1
- Git clone
- Frontend
    - npm install -> install dependecies
    - npm run build
    - sudo apt update
    - sudo apt install nginx
    - sudo systemctl start nginx
    - sudo systemctl enable nginx
    - copy code from dist(build files) to /var/www/html
    - sudo scp -r dist/* /var/www/html 
    - Enable port :80 of your instance
- Backend
    - 