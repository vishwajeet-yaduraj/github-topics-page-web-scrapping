"# github-topics-page-web-scrapping" 
# Overview
This project is a Python-based tool designed to scrape the top 30 trending topics on GitHub and retrieve detailed information about the top 20 repositories associated with each topic. The collected data includes the repository's username, name, URL, and star count, which are then saved into CSV files, organized by topic.

# Features
* Scrapes Top 25 GitHub Topics: Automatically identifies and retrieves the top 25 trending topics on GitHub.
* Extracts Detailed Repository Data: For each topic, the top 20 repositories are scraped, including their username, repository name, URL, and star count.
* CSV Export: Each topic's data is saved as a separate CSV file within a Data folder, making it easy to access and analyze.
* Efficient and Scalable: Designed to be scalable, allowing for future enhancements such as adding more topics, repositories, and additional data points.

# Project Structure
* scrape_topic_repos(url): The main function that coordinates the scraping of topics and their respective repositories.
* get_repo_info(h3_tags, star_tags): Extracts detailed information about each repository.
* get_stars_count(span): Converts star counts from string format (e.g., '1.2k') to integer format.
* get_topic_repos(topic_soup): Compiles the repository data into a DataFrame for further processing.
* scrape_topics(topic_url, path): Handles the scraping of repository data for a specific topic and saves it to a CSV file.
* get_url_page(topic_url): Downloads the HTML content of a given GitHub topics page.
* scrape_topics_page(url): Scrapes the list of topics from the provided GitHub URL.

# Installation
1. Clone the repository:
2. git clone https://github.com/vishwajeet-yaduraj/github-topics-page-web=scrapping.git
   cd github-topics-page-web=scrapping
## Usage
To scrape the top 30 GitHub topics and their top 20 repositories, simply run the script with the desired GitHub topics URL.
The scraped data will be saved in the Data directory.

Example usage: scrape_topic_repos("https://github.com/topics")
This will create a Data folder containing CSV files for each topic with the top repositories' information.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request if you'd like to contribute to the project.

