(scenario-7)creating backend container


here frontend is only present to test whether backend successfully running in container

backend test done using -
1- direct frontend
2- using postman

You are a Full-Stack Engineer in charge of deploying the Hospital Management System for a university healthcare portal. The project has two parts: ·         
Backend (API): Spring Boot application that exposes /auth/signup and /auth/login are endpoints. Uses MySQL database and runs on localhost:8081.  
Backend url: https://github.com/suneethabulla/hospital-backend.git ·         
Frontend: React (Vite) application that consumes these endpoints and displays Login and Signup pages. 
Dashboard page showing hospital modules (Doctors, Patients, Appointments) and runs on localhost:5173. 
Frontend url: https://github.com/suneethabulla/hospital-frontend.git Your task is to download, run, and deploy the system following CI/CD best practices. 

1.Clone the GitHub repository of the Hospital Management System onto your local machine. Execute locally and verify your frontend successful login and signup functionality by interacting with the backend API at http://localhost:8081   
2.Backend Deployment via Docker without Volume   Output verification: http://localhost:8081/auth/signup?username=testuser&email=testuser@gmail.com&password=admin123



successfully deployed backend in docker using docker with port 8081
you can verify the output in outputs folder i have provided all output screenshots

you can also verify this by cloning this and running on docker container by using this commands

docker build -t hospital-backend .

docker run -d -p 8081:8081 --name hospital-backend hospital-backend
you can customize port number
i used 8081 because in 8080 jenkins is running

Thank you"# endsemlab" 
