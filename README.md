# Full Stack Developer Assessment - Game Monitoring Application (.NET Core, Angular)

Your task is to build a Full Stack application using .NET Core for the backend and Angular for the frontend. The application will allow authenticated users to monitor players and team details in a game. Follow the instructions below to complete the assessment.

## Overview

### Backend (.NET Core):

- Implement signup and signin functionality using JSON Web Tokens (JWT) to ensure secure user access to the application.
- Upon signup, users should be assigned a random score.
- Implement role-based access control to restrict certain endpoints to authorized users only.
- Authenticated users can fetch a list of users, including the following details:
  - Rank
  - Name
  - Score
  - Team
- Create CRUD operations for teams.
  - Users can create a team with the following details:
    - Team name (required)
    - Maximum member number (should be greater than 10)
  - The user creating the team will become its owner.
  - Team owners can update team information and have the - ability to reject team member requests.
  - Team owners can also delete the entire team.
- Authenticated users can fetch a list of teams, including the following details:
  - Name
  - Owner Name
  - Total Score (summarize of member scores)
  - Member Number
  - Available Member Number
- Authenticated users can fetch team information, including the following details for each team member:
  - Rank (total rank by score in the game)
  - Name
  - Score
- Implement appropriate error handling and validation throughout the backend to ensure data integrity and security.

### Frontend (Angular):

- Implement a user-friendly interface to interact with the backend API.
- Create signup and signin forms to handle user authentication.
- Display a dashboard for authenticated users to view their details and perform various actions.
- Provide a user interface for team management:
  - Create, update, and delete teams.
  - View team details and members.
  - Allow users to request to join a team and team owners to manage those requests.
- Display a leaderboard showing users ranked by their scores.

## Acceptance Criteria

### Backend:

- Develop a .NET Core backend to handle HTTP requests and responses.
- Use ASP.NET Core Identity and JWT for user authentication and authorization.
- Generate a random score for users upon signup.
- Implement role-based access control to protect certain endpoints.
- Design CRUD operations for teams, including creating, updating, and deleting teams.
- Allow users to join existing teams.
- Create API endpoints to retrieve team information along with details for each team member (rank, score, name).
- Ensure proper error handling and validation to prevent invalid data input and unauthorized access.

### Frontend:

- Develop an Angular frontend to interact with the backend API.
- Implement user authentication using JWT tokens.
- Create responsive and user-friendly forms for signup and signin.
- Implement a dashboard for users to view and manage their profiles and teams.
- Create components for viewing and managing teams and members.
- Display a leaderboard with user ranks and scores.

## Assessment Evaluation

- **Code Quality:** Clear, readable, and maintainable code.
- **Functionality:** Complete and working features as described.
- **Security:** Proper implementation of authentication and authorization.
- **Error Handling:** Graceful handling of errors and edge cases.
- **Query Performance:** Efficient database queries and handling.
- **Unit Tests:** Comprehensive test coverage for both backend and frontend.

## Bonus

- API documentation using Swagger or a similar tool.
- Dockerization for easy setup and deployment.

## Submission Guidelines

- Share the GitHub repository link containing your complete .NET Core backend and Angular frontend code.
- Include clear instructions on how to set up and run both the backend and frontend applications locally.
- Try your best to implement as much as you can from the given requirements.
