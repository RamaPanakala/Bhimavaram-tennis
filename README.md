# Bhimavaram Tennis Management

This is the web application for managing the Bhimavaram tennis club - tournaments, players, scores, and rankings. It helps organize matches and track who's winning.

## What does it do?

The app lets you:
- Create and run singles and doubles tournaments
- Add players and track their stats
- Record match results and update rankings
- View player profiles and tournament history
- See charts and analytics
- Manage teams and categories

Everyone in the club can visit the site to check tournaments, see who's ranked where, and look at match results.

## Getting Started

You'll need:
- PHP (7.0 or newer)
- MySQL database
- A web server (Apache works fine)

### Quick Setup

1. Clone or download the project
2. Import the database:
   ```
   mysql -u root -p bhimavaram_tennis < bhimavaramtennis.sql
   ```
3. Edit `NewBhim/dashboard/admin/config.php` with your database info:
   ```php
   $host = "localhost";
   $user = "your_db_user";
   $password = "your_db_password";
   $database = "bhimavaram_tennis";
   ```
4. Put the `NewBhim/dashboard/` folder in your web server folder (usually `htdocs`)
5. Open the site: `http://localhost/dashboard/`

## Using It

**Admin Login**: Go to `/admin/` and log in to manage everything

**Add a Player**: Players section - fill in their name and info

**Create Tournament**: Pick singles or doubles, add players, set a date

**Enter Scores**: When matches finish, add the results - rankings update automatically

**Check Rankings**: Players can see the leaderboard and their stats

## What's Inside

```
NewBhim/dashboard/
├── admin/
│   ├── index.php         - Admin dashboard
│   ├── players.php       - Manage all players
│   ├── tournament.php    - Create tournaments
│   ├── singles.php       - Singles matches
│   ├── doubles.php       - Doubles matches
│   └── config.php        - Database setup
├── singles.php           - View singles results
├── doubles.php           - View doubles results
├── profiles.php          - Player profiles
├── ranks.php             - Player rankings
├── css/                  - Styling
└── js/                   - Interactive features
```

## Database

Main things stored in the database:
- Players and their profiles
- Tournaments and matches
- Match results and scores
- Player points and rankings
- Teams and categories
- Club information

## Notes

- Keep your admin password secure
- Back up your database regularly
- The site is built with HTML, CSS, PHP, and MySQL

That's it! It's a straightforward system for running tennis tournaments locally.