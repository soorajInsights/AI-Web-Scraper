# AI Web Scraper

## Project Description
The AI Web Scraper is a Python-based application designed to scrape websites dynamically based on user-provided URLs. The tool retrieves the DOM content of the site and leverages AI to extract specific information based on user prompts. The project demonstrates the integration of powerful tools such as Selenium, BeautifulSoup, LangChain, and more.

### Features
- **Dynamic Web Scraping**: Use Selenium to navigate and scrape website content.
- **AI-Powered Information Extraction**: Pass prompts to the AI for targeted data extraction.
- **Captcha and IP Ban Handling**: Incorporates Bright Data credentials to bypass captchas and IP restrictions.
- **Streamlit UI**: A user-friendly interface for managing scraping and data extraction workflows.

---

## Installation and Setup

### Prerequisites
- Python 3.8+
- Pipenv or Virtualenv (optional but recommended)
- Selenium WebDriver
- Streamlit
- Bright Data credentials (for handling captchas and unblocking websites)
- [Ollama](https://ollama.com/) (LLM for parsing content)

### Steps to Set Up

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/ai-web-scraper.git
   cd ai-web-scraper
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Install Selenium WebDriver**:
   - Download the appropriate WebDriver for your browser ([Selenium WebDriver](https://www.selenium.dev/documentation/webdriver/)).
   - Chrome driver download [chrome driver](https://googlechromelabs.github.io/chrome-for-testing/)
   - Ensure the WebDriver binary is added to your system PATH.

5. **Install Ollama Locally**:
   - Follow the installation guide for Ollama from their [official website](https://ollama.com/).
   - Ollama models [github link](https://github.com/ollama/ollama) 

7. **Configure Bright Data Credentials**:
   - Sign up at [Bright Data](https://brightdata.com/).
   - Set up your captcha-solving credentials as per the [Bright Data Documentation](https://support.brightdata.com/hc/en-us/articles/360015683617-Setting-up-Captcha-solving).

---

## Usage

### Starting the Streamlit UI
Run the following command to start the Streamlit-based user interface:
```bash
streamlit run app.py
```

### Web Scraping with Selenium
The tool uses Selenium to dynamically load and interact with websites. Ensure that the WebDriver is properly set up and accessible.

### Handling Captchas and Unblocking Websites
The scraper integrates with Bright Data to handle captchas and avoid IP bans. Make sure to provide valid Bright Data credentials in the configuration file.

### Parsing Content with Ollama
Once the DOM content is scraped, you can pass user-defined prompts to Ollama's LLM to extract specific information from the website.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.
