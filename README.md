# Open Source Article Summarizer with OpenAI GPT-4

Yo-yaku AI summarizer is an open-source article summarization tool powered by the advanced capabilities of OpenAI GPT-4. Designed to help users quickly grasp the essence of lengthy articles, Yo-yaku transforms verbose content into clear, concise, and informative summaries. By leveraging the cutting-edge natural language processing techniques of GPT-4, Yo-yaku ensures that generated summaries maintain context, coherence, and accuracy.

## Key Features

- Open-source
- Powered by GPT-4
- Flexible input formats
- Customizable summary length
- Easy integration
- Multi-platform compatibility

## Demo
![youyaku_ai_summarizer](https://github.com/maegatro/yo-yaku_ai_summarizer/assets/47557622/1c1ac531-af38-4ca8-8235-a9b68d9c9991)

[Live Demo](https://6514f046e2c62539d6186ae1--zingy-cheesecake-1d4e1a.netlify.app/)

## Installation
Follow these steps to install and set up Sumz on your local machine:

Clone the repository:
```
git clone https://github.com/jbxamora/articlesumz.git
```
Install Dependencies:

```npm i ``` or ```npm install```

Create dotenv file:
```
VITE_RAPID_API_KEY=yourapikey
```
Run on your local machine:
```
npm run dev
```
Enjoy Summarizing!

## API
View The Endpoints Here:

This is an API which extracts news/article body from a URL and uses GPT to summarize the article content.
[Rapid API](https://rapidapi.com/restyler/api/article-extractor-and-summarizer)

### Example Config
```js
const axios = require("axios");

const options = {
  method: 'POST',
  url: 'https://article-extractor-and-summarizer.p.rapidapi.com/summarize-text',
  headers: {
    'content-type': 'application/json',
    'X-RapidAPI-Key': 'yourapikey',
    'X-RapidAPI-Host': 'article-extractor-and-summarizer.p.rapidapi.com'
  },
  data: '{"text":"article of markdown text"}'
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
```
