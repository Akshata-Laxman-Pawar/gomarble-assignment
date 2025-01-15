
## Objective

Develop an API server capable of extracting reviews information from any given product page (e.g., Shopify, Amazon). The API should dynamically identify CSS elements of reviews and handle pagination to retrieve all reviews.
# 1.Programming Language 
Python, HTML, CSS
# 2. API Development

- **Endpoint Specification**
    - **Endpoint:** `?url=https://www.amazon.com/dp/B08X8VJQZD`
    - **Method:** `GET`
    - **Response Format:**
{
  "reviews": [
    "This product is amazing! Highly recommended.",
    "Not what I expected. Quality could be better."
  ]
}

### 3. Functional Requirements

- **Dynamic CSS Identification**
    - Utilize Large Language Models (LLMs) to identify dynamic CSS selectors for reviews on the given product page.
- **Pagination Handling**
    - Implement logic to navigate through all pages of reviews to ensure complete data extraction.
- **Universal Compatibility**
    - The API should work with any kind of reviews page and extract relevant information accurately.

### 4. Technical Requirements

- **Browser Automation Frameworks**
    - Use frameworks like **Playwright**, **Puppeteer**, or **Selenium** to simulate browser activity and interact with web pages.
- **LLM Integration**
    - Provide a provision to configure and use OpenAI's LLM with an `OPENAI_API_KEY`.
    - If using a free LLM, include details and credentials in the documentation.

