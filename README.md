
# Cricket Simulation

## Overview

This project simulates a cricket match between teams. It includes functionalities such as defining teams, players (batsmen and bowlers), and simulating the match to generate a score chart. The project is developed using PHP and SQL for database interactions.

## Setup Instructions

### Prerequisites

- PHP (version 7.4 or higher recommended)
- MySQL (or any compatible database server)
- A web server (such as Apache or Nginx)
- Composer (for managing PHP dependencies)

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/cricket-simulation.git
   cd cricket-simulation
   ```

2. **Install Dependencies**

   If you have any dependencies managed by Composer, install them:

   ```bash
   composer install
   ```

3. **Database Setup**

   - Create a new MySQL database.
   - Import the SQL files (`TeamSQL.php`, `PlayerSQL.php`) to create the necessary tables and insert initial data.

   ```sql
   -- Example commands to run in your MySQL environment
   source path/to/TeamSQL.php;
   source path/to/PlayerSQL.php;
   ```

4. **Configure the Project**

   - Update the database configuration in the project files where necessary (usually in a configuration file like `config.php` or directly in the script files).

5. **Run the Project**

   - Place the project files in your web server's root directory.
   - Access the project through your web browser (e.g., `http://localhost/cricket-simulation/start.php`).

## Project Structure and Description

### Files

1. **TeamSQL.php**
   
   Contains SQL queries and database interactions related to cricket teams. Includes functionality for adding, updating, deleting, and retrieving team information from the database.

2. **PlayerSQL.php**

   Contains SQL queries for managing player information. This includes batsmen and bowlers' data.

3. **start.php**

   The main entry point of the project. Initializes the simulation and sets up the necessary components to start the cricket match.

4. **ScoreChart.php**

   Handles the generation and display of the score chart for the match. It shows the results of the simulated cricket match.

5. **Player.php**

   Defines the `Player` class. This class likely includes properties and methods common to all players, such as name, type, and statistics.

6. **Batsman.php**

   Defines the `Batsman` class, which extends the `Player` class. This class includes properties and methods specific to batsmen, such as runs scored and balls faced.

7. **Bowler.php**

   Defines the `Bowler` class, which extends the `Player` class. This class includes properties and methods specific to bowlers, such as overs bowled and wickets taken.

8. **Team.php**

   Defines the `Team` class. This class includes properties and methods for managing a cricket team, such as team name, players, and team statistics.

9. **TeamCollection.php**

   Manages a collection of `Team` objects. Provides functionalities to add, retrieve, and manage multiple teams.

## Project Flow

1. **Initialization:**
   - `start.php` initializes the project and sets up the necessary components.
   
2. **Team and Player Management:**
   - Teams and players are managed through `Team.php`, `Player.php`, `Batsman.php`, and `Bowler.php`.
   - Database interactions are handled through `TeamSQL.php` and `PlayerSQL.php`.

3. **Simulation:**
   - The cricket match is simulated using the player and team data.
   - Results are generated and displayed using `ScoreChart.php`.

## Developed By

Abdullah Awan  
GitHub: [abawan7](https://github.com/abawan7)  
Email: [mlkabawan336@gmail.com](mailto:mlkabawan336@gmail.com)

