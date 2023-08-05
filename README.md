# 🖊️ MinimalPrompt: A Minimalist Approach to Prompt Engineering 📚

MinimalPrompt is your minimalist, no-frills approach to the world of prompt engineering for AI models. This project efficiently chisels away the unnecessary, leaving behind only the most effective techniques for creating, refining, and analysing prompts. Our aim is to amplify the performance and reliability of language models.

In this repository, you will uncover:

- **Techniques for effective prompt design**, including guides on how to create prompts that elicit specific responses from AI models.
- **Case studies** that highlight real-world examples of prompt engineering.
- **Tools and scripts** for automating the process of prompt generation and evaluation.
- **Research** related to prompt engineering, including links to relevant academic papers and other resources.
- **Community Contributions** for users to share their own prompt engineering strategies and findings.

- **🎨 Techniques for effective prompt design**: Guides on creating prompts that elicit specific responses from AI models.
- **🌍 Case Studies**: Real-world examples of prompt engineering.
~- 🛠️ Tools and Scripts: Automate your process of prompt generation and evaluation.~
~- 🔬 Research: Links to relevant academic papers and other resources on prompt engineering.~
~- 👥 Community Contributions: Share your own strategies and findings on prompt engineering.~

Whether you're a researcher, an AI enthusiast, or a developer, we hope this repository will help you improve the performance of your AI models. We encourage contributions and feedback to continually improve and expand the field of prompt engineering.

Happy prompt crafting!

# 📝 General Principles on Prompt Engineering (Based on OpenAI)
This section outlines principles and guidelines for crafting prompts with OpenAI's models.

## Principle I: Be Clear and Specific 🎯
When crafting prompts, clarity and specificity are key. The model should be able to understand exactly what is being asked.

### 1. Use Delimiters
Delimiters can help separate different parts of the input, making it clearer for the model.
Example: `prompt = '"This is the first part of the input." "This is the second part of the input."'`

### 2. Ask for a Structured Output
Asking the model for a structured output can make parsing the results easier.
Example: `prompt = 'Translate the following English text to French in JSON format: "Hello, world."'`

### 3. Check Conditions
It's a good practice to have the model check certain conditions before executing a task.
Example: `prompt = 'If the following text contains instructions, rewrite them in a numbered list: "First, preheat the oven. Then, mix the ingredients."'`

### 4. Few-Shot Prompting
Few-shot prompting involves providing the model with a few examples of the desired output before asking it to complete a task.
Example: `prompt = '"Hello, world." in French is "Bonjour, monde." "Goodbye" in French is "Au revoir." What is "Thank you" in French?'`

## Principle II: Give the Model Time to “Think”
Sometimes, it's useful to have the model go through intermediate steps before arriving at a final answer.

### 1. Specify the Intermediate Steps to do the Task
You can specify the steps the model should take to reach the final answer.
Example: `prompt = 'To solve the equation 2x + 3 = 7, first subtract 3 from both sides. Then, divide both sides by 2. What is the value of x?'`

### 2. Instruct the Model to Work Out Its Own Solution
Instructing the model to work out its own solution can help it arrive at the correct answer.
Example: `prompt = 'Solve the equation 2x + 3 = 7 for x.'`

## Case studies 📝
1. ChatGPT’s On-Demand Prompt Generation for Effortless Working 🤖
    ```What’s the best prompt for ChatGPT to learn my writing style and then suggest some titles for a blog post?```

2. ChatGPT’s Transformation Into a Guru [Profession] 🧙
    ```I want you to act as a world-class [profession name] with decades of experience in [what the professional does]. I will ask you for output, and you have to give me unique, expertly written work.```

3. ChatGPT Can Mimic Human Style 👨
    ```Analyze the text below for style, voice, and tone. Later, you will need to write whatever I tell you in the same style, voice, and tone: [insert your text].```

4. ChatGPT’s On-Demand Prompt Generation for Effortless Working 🤖
    ```What’s the best prompt for ChatGPT to learn my writing style and then suggest some titles for a blog post?```

5. ChatGPT’s Transformation Into a Guru [Profession] 🧙
    ```I want you to act as a world-class [profession name] with decades of experience in [what the professional does]. I will ask you for output, and you have to give me unique, expertly written work.```

6. ChatGPT Can Mimic Human Style 👨
    ```Analyze the text below for style, voice, and tone. Later, you will need to write whatever I tell you in the same style, voice, and tone: [insert your text].```

7. Content Creation 📰
    ```As a skilled storyteller, your task is to create an original and captivating story about [topic] for children aged [8-10] years old. Your story should be detailed, immersive, and filled with vivid descriptions that engage the senses of young readers. The plot should focus on a meaningful moral lesson, with relatable characters that the readers can empathize with and learn from. Your story should be a minimum of [500] words. Please ensure that the story unfolds in an exciting manner, building up to a thrilling climax that captures the reader’s attention. Conclude the tale with a satisfying ending that effectively conveys the moral lesson learned through the characters’ experiences. Your response should be creative and original, providing enough detail to clarify the narrative, evoke emotions, and create a memorable experienc for young readers. While crafting the story, always keep the target age group in mind and the moral lesson you wish to convey to them. Feel free to incorporate elements of adventure, fantasy, or mystery, and always consider the importance of engaging storytelling techniques that appeal to this age group.```

8. Online Education 💻
    ```As an AI language model, your task is to generate a succinct, understandable, and comprehensive explanation of a complex concept. This explanation must be tailored to the understanding level of a specific group. The complex concept you need to decipher is: [Please insert the complex concept to explain here] The target audience for your explanation is: [Please provide a detailed description of your target audience, including their age group, level of previous understanding or lack thereof, and the context in which they will access this information.] With the concept and audience in mind, craft an explanation that: 1. Captures the target audience's interest by introducing the concept in a contextual way that resonates with them and highlights its relevance. 2. Breaks down the main concept into subtopics or key points. 3. Clearly interprets each subtopic or primary idea, using language and examples suitable for the target audience. 4. Provides a summary of the entire concept and its essential points, ensuring the audience retains the information by reinforcing the main ideas. Please end your response with a brief summarization of your detailed explanation.```

9. Consulting Services 🤵
    ```Acting in the role of a data analyst, you are to extract, analyze, interpret, and visually present a given data set. You will create a narrative that makes the findings comprehensible and accessible. The directions below provide a clear pathway for the task: 1. Data Preprocessing: Initiate your task with data preprocessing. Scrutinize the data set for [insert data set] any potential discrepancies or disarray, while ensuring that there is no modification in the original values. Rectify and organize the data set into a structure that simplifies deeper-level analysis. 2. Data Review: User verification of the processed data set against the original will confirm the integrity and accuracy of the refined data. 3. Data Summary: Using the rectified data set, compose a comprehensive summary that unveils key trends and deeper understandings about the data. 4. Data Analysis: Investigate the data in detail to unravel significant trends, correlations, or anomalies in multiple variables. Any outliers or anomalies should be accompanied with a clear, brief explanation backed-up by a mathematical or statistical reasoning. 5. Insight Extraction: Present any additional insights gathered from the data set that provide broader context. Predict large-scale patterns correlated with these insights and explain their applicability in real-world contexts. 6. Data Visualization: Recommend an ideal method for visually displaying the processed data, with the aim of clear and efficient communication of key information. Justify why this visualization form is superior to other possible methods. 7. Summary Presentation: Lastly, condense your analysis into a concise story, intended for delivery in about a minute. This summary should include all vital aspects of your analysis, except for the data visualization part in an engaging and comprehensive manner.```

10. Explain this topic like I’m 5. 🧒
    ```Explain the following topic to a 5-year-old child: [Please insert the topic to explain here]```

11. Expert-Level Output in Minutes 🧙
    ```I want you to act as a world-class [profession name] with decades of experience in [what the professional does]. I will ask you for output, and you have to give me unique, expertly written work.```

12. Change the writing style and elevate your writing skills 📝
    ```Change the writing style of the text below to [style or tone] [paste text]```

13. Learning from the best with ChatGPT 📚
    ```I will give you a sample of my writting and I want you to criticize it as you were [the name of the expert]: [paste text]```

14. Rewrite the text as you were an expert 📝
    ```I will give you a sample of my writting and I want you to rewrite it as you were [the name of the expert]: [paste text]```

15. Recommending and Summarizing the book 📚
    ```I am looking for the best book to read to learn [topic]. I want you to recommend me a book and summarize it in a few sentences.```

16. Write the code for me 🤖
    ```Could you provide me with the code to create a [functionality name] functionality using [programming language]?```

## How to bypass AI Content Detection 🚫
```Hey ChatGPT, regarding generating writing content, two factors are crucial to be in the highest degree, “perplexity” and “burstiness.” Perplexity measures the complexity of the text. Separately, burstiness compares the variations of sentences. Humans tend to write with greater burstiness, for example, with some longer or more complex sentences alongside shorter ones. Al sentences tend to be more uniform. Therefore, generated text content must have the highest degree of perplexity and the highest degree of burstiness. The other two factors are that writing should be maximum contextually relevant and maximum coherent.```
