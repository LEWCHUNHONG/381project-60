# 381project-60

# News Website

## Introduction

Welcome to the News Website project! This web application allows users to manage and interact with news articles. It includes user authentication, a search feature, and the ability to create, update, and delete articles. The project is designed to provide a clean and user-friendly interface, making it easy for users to navigate and manage news content.

## Features

- **User Authentication**: Secure login functionality to ensure that only authorized users can manage news articles.
- **Search Bar**: Quickly find articles by title using a responsive search feature.
- **CRUD Operations**:
  - **Create**: Add new news articles effortlessly.
  - **Read**: View a list of all news articles with relevant details.
  - **Update**: Edit existing articles to keep content current and accurate.
  - **Delete**: Remove articles that are no longer relevant with a simple click.

## Technologies Used

- **Frontend**: EJS (Embedded JavaScript Templates) for rendering dynamic HTML pages.
- **Backend**: Node.js and Express.js for server-side logic.
- **Database**: MongoDB for storing news articles and user data.
- **Middleware**: 
  - `cookie-session` for session management.
  - `body-parser` for parsing incoming request bodies.
  - `method-override` for supporting PUT and DELETE requests.

## Getting Started

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/LEWCHUNHONG/381project-60.git

2. **Add mongodb uri**:
   server.js
   ```bash
   uri = ''

4. **Start server**:
   ```bash
   npm install
   npm start

5. **Register**:
   ```bash
   Click Register
   Create account

6. **Login**:
   ```bash
   Click Login

7. **CURD**:
   ```bash
   Search, Edit, Delete News

8. **RESTful API**:

   ```bash
   Create:
   curl -X POST -H "Content-Type: application/json" --data '{"title":"TEst news123","imageUrl":"","info":"ＴＨＩＳ　ＩＳ　ＴＥＳＴ！！！！"}' <IP:PORT>/api/news/

   
   Read:
   curl -X GET "http://<ip:port>/api/title/<title>"

   
   Updata:
   curl -X PUT -H "Content-type: application/json" -d '{"imageUrl": "", "info": "Updated info"}' '<IP:PORT>/api/title/title/<title>'

   Delete:
   curl -X DELETE "<ip:port>/api/title/<title>"


Docker:

   ```bash
docker login 

docker build -t 381-project-60 .

docker run -p <port>:<port> -d 381-project-60


docker stop <container-id>

docker rm <container-id>

docker image rm <image-id>
