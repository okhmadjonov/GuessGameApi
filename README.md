# Lasttodoapp
Number Guessing Game App.
This project is built on Windows 10 OS.

## Prerequisite
- [.NET SDK 7.0](https://dotnet.microsoft.com/download)
- [PostgreSQL](https://www.postgresql.org/download/)

## Getting started
1. Cloning the repository
   ``https://github.com/okhmadjonov/GuessGameApi.git``

2. Navigate to the project folder:

   `` cd your-project-name ``
3.  Write on the terminal this code first
   `` dotnet-build
      dotnet restore ``

4. Database setup:
   - Create a PostgreSQL database for the project.
   - Update  the project's appsetting.json file according to your DB configuration (login, password)
     ``   {
          "ConnectionStrings": {
            "DefaultConnection": "Host=localhost;Port=5432;Database=fullgame;Username=postgres;Password=postgres"
          },
          // other settings...
        }  ``
5. Run migrations:
   `` add-migration  "InitialMigration"
      update-database
   ``
6. Run the Application
   `` dotnet run ``

7.  Registration => Login => 
8.  => Authorize Token
9.  From the /api/Game url start game, it will generate session id, just copy it
10.  Past copied session id to  /api/Game/guess/{sessionId}  url's sessionId field, than enter guessing number below the sessionId field
11.  ... other steps can continue user's themself

## Acknowledgements
  Mentioning any libraries, changes or tools is always welcome.
