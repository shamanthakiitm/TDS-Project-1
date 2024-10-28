# GitHub User and Repository Data Scraper for Austin, TX

This project uses the GitHub API to scrape data on GitHub users based in Austin, Texas, who have over 100 followers, along with details of their public repositories. The data is saved into two CSV files, `users.csv` and `repositories.csv`, for easy analysis and exploration.



## Key Points

- The script leverages the GitHub API to gather data on users in Austin with 100+ followers and up to 500 of their most recent repositories.
- Analysis revealed that a notable number of high-follower users have fewer than 10 public repositories, suggesting a focus on networking or selective sharing.
- Recommendation: Developers can enhance engagement by increasing community contributions and visible public repositories to leverage follower networks more effectively.



## Data Collected

### User Data (`users.csv`)
Each user entry in `users.csv` includes:
- **login**: GitHub username
- **name**: Full name of the user
- **company**: The company the user is associated with (standardized format)
- **location**: User’s city (e.g., Austin)
- **email**: User's public email, if available
- **hireable**: Whether the user is open to job offers
- **bio**: Short bio provided by the user
- **public_repos**: Number of public repositories owned by the user
- **followers**: Number of followers the user has
- **following**: Number of users the user follows
- **created_at**: Date the user joined GitHub

### Repository Data (`repositories.csv`)
Each repository entry in `repositories.csv` includes:
- **login**: GitHub username of the repository owner
- **full_name**: Full name of the repository
- **created_at**: Date the repository was created
- **stargazers_count**: Number of stars on the repository
- **watchers_count**: Number of watchers for the repository
- **language**: Primary programming language used
- **has_projects**: Whether the Projects feature is enabled
- **has_wiki**: Whether the Wiki feature is enabled
- **license_name**: License type of the repository (if available)


## Usage

1. **Setup**: Replace GitHub API Token in the script with your personal GitHub token with `read:user` and `public_repo` permissions.
2. **Run the Script**: Execute the script to create `users.csv` and `repositories.csv`.
