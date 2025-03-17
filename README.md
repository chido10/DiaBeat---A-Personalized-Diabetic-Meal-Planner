# Executive Summary
DiaBeat is an AI-powered meal planning application designed to address the dietary challenges faced by individuals managing diabetes. Developed using Amazon PartyRock, this solution provides personalized, diabetes-friendly meal recommendations with comprehensive nutritional information to support healthy eating habits.

# Project Background
Diabetes management requires vigilant monitoring of dietary intake and nutrition. Many individuals find it challenging to consistently identify meals that are both appetizing and appropriate for maintaining stable blood glucose levels. DiaBeat was developed to address this need by providing an accessible, user-friendly platform that generates customized meal plans based on specific dietary requirements.

# Solution Overview
This guide provides a comprehensive walkthrough of the DiaBeat development process using Amazon PartyRock's no-code AI platform. The document details each step of the implementation process, from initial concept to final deployment, enabling readers to understand the methodology and potentially replicate similar solutions for other health management applications.
By the conclusion of this guide, readers will gain:
•	A thorough understanding of DiaBeat's functionality and technical implementation
•	Knowledge of how to leverage Amazon PartyRock for healthcare applications
•	Insights applicable to creating similar solutions for fitness, mental health, or personal finance applications

# Implementation Process
The following sections outline the step-by-step development process of the DiaBeat application.


🚀 Step 1: Accessing Amazon PartyRock
Every journey begins with the first step, and ours starts at AWS PartyRock. PartyRock is an intuitive AWS service that enables anyone—even without coding skills—to build powerful AI-driven apps quickly.
![image](https://github.com/user-attachments/assets/b0451895-6930-49b3-8834-b7b181e3dd8e)

📌 Step 2: Starting a New App
Once logged into PartyRock, click on "Create New App". It's easy and straightforward. You'll be prompted with, "What do you want to build?" I entered my goal clearly: see the attached image below.
Why a diabetic meal planner? Well, personalized nutrition significantly helps people with diabetes manage their blood sugar levels, reduces complications, and greatly improves their overall quality of life. You can build any app you want just by entering a prompt to start with, but make sure the prompt is well structured as PartyRock will use it to kick off its first design. This can also be called the initial prompt or general prompt. 
![image](https://github.com/user-attachments/assets/469c35e2-4058-4cb9-b5dd-15fb67c34f52)

 
🎨 Step 3: Customizing DiaBeat's Interface
Next, PartyRock automatically generated an initial layout for DiaBeat which contains the 2 user inputs options just like described in the prompt (Meal Time and Food Preference) and three outputs result Meal Recommendation, Meal Image and Nutritional Information. To personalize it further, we clicked on the edit icon at the top of each widget. You have complete flexibility here to edit each widget based on the name, description, widgets, and for the output widgets you can modify the prompts or choose AI models used for generating content.
 ![image](https://github.com/user-attachments/assets/aa28007c-99bd-4d30-9b81-5db6443620b9)
![image](https://github.com/user-attachments/assets/ba1d12c2-d607-41b0-924d-ac61bf4290ee)
![image](https://github.com/user-attachments/assets/37812665-2b4b-481e-97fc-4453db280ffa)
![image](https://github.com/user-attachments/assets/e2998310-fb45-47db-8387-a3144df535f8)    
 
🖼️ Step 4: Generating Mouth-Watering Meal Recommendations
Once we have set our input and output preferences, next is to test it and see the results. As a user all you must do is to use the input section and input the mealtime and food preference and then press “enter”, the app will generate Meal Recommendation, the corresponding Meal Image and Nutritional Information for you.
 ![image](https://github.com/user-attachments/assets/6943ba81-3d83-40e8-93f9-6f8973ced3d1)
![image](https://github.com/user-attachments/assets/d640f2c4-ffa2-42b0-8b36-df40c77f38ae)

🍱 Step 5: Generating Diabetic-Friendly Meal Prompts
Each output widget can be tweaked for different output expectations or user choice, say for example, we do not like the suggested meal recommendations for model A, we can decide to try another model B. The same with the image generation and the Nutritional Information section. 
For example, the initial Meal Recommendation output used Claude 3.5 Sonnet v2, Meal Image used Stable Image Core, and Nutritional Information used same Claude 3.5 Sonnet v2. We can also edit the prompt further to suit the specific user preference in the prompt section. 
![image](https://github.com/user-attachments/assets/9efdaa8b-1a86-4481-8246-8f571ea801e2)
![image](https://github.com/user-attachments/assets/7bb0b164-5856-4b1e-b8a3-11895d991f96)
![image](https://github.com/user-attachments/assets/afe2263f-1cc6-47b3-b333-e7914588c500)
![image](https://github.com/user-attachments/assets/2d34203e-d0f5-495d-bb12-f9c964bcdd0b)

🧑‍🍳 Step 6: Selecting different AI Models
To enhance user experience and experiment different models, we choose different models for the output widget while maintaining the same inputs “supper” Meal Time and “low carb” for Food Preference. We also maintained the same tailored prompt for the outputs.![image](https://github.com/user-attachments/assets/6d4494e2-bd89-4455-85b4-c801c809f437)
![image](https://github.com/user-attachments/assets/0c6a7c77-ae39-4764-ab4a-a88b0383643f)
![image](https://github.com/user-attachments/assets/4e7b8bde-2fd9-4aa2-be94-0de74d9a3377)
![image](https://github.com/user-attachments/assets/941b80ae-96ca-42b1-a84d-bbd066230bdc)


🥘 Step 7: Testing Personalized Meal Generation using a different model
We extensively tested the app by entering various mealtimes and dietary preferences to ensure meal suggestions were accurate and appetizing. You can also do this for any app you want to build as different model has different response to user inputs. Below is the result of using another model for each output while maintaining the same input and prompts. Personally, we prefer this output.
![image](https://github.com/user-attachments/assets/3405a8c2-914d-476d-a688-658ed45d3a6a)

💬 Step 8: Virtual Dietitian Integration Chatbot
Apart from the core output sections, a virtual dietitian chatbot was also integrated, offering instant, personalized dietary advice to enhance user support and engagement. You can also add more widget for more personalized dietary advice or improved app.
 ![image](https://github.com/user-attachments/assets/9fbfae94-0e56-4ec1-8f7f-6094ee117d46)


🚫 Step 9: Setting Negative Image Prompts
The image output has an advanced option of improving the outcome of the image by using the Negative Prompt. Here we can decide to streamline what the image shows by adding instruction to it. For example, “Avoid negative prompt, e.g., sugar, dairy, fried foods, etc.”
This makes sure that the image follows the given instruction as a guardrail.
   ![image](https://github.com/user-attachments/assets/5d3ab5f8-4a4d-49b4-81db-77f987f782a4)


🔍 Step 10: Reviewing & Refining the App
We meticulously reviewed each app component—interface, recommendations, nutritional information, images, and chatbot responses—to ensure accuracy and user-friendliness.

🌐 Step 11: Publishing DiaBeat
Once we were happy with the app, it was time to share DiaBeat. PartyRock provides multiple options for sharing: Private, Shared, or Public. I chose Shared, allowing anyone with the link to use DiaBeat. This means you can also easily share your creation with friends, family, or community members who might benefit from it. You can use the link below to Visit the DiaBeat app > https://partyrock.aws/u/doodoo10/klRkZDk6a/DiaBeat-Personalized-Diabetic-Meal-Planner
    ![image](https://github.com/user-attachments/assets/51aea08c-b7af-4ea1-abd7-f337b81d705f)
![image](https://github.com/user-attachments/assets/5c0b0fbb-3a03-44c7-be8d-a4881906b90c)


⏳ Time & Cost
•	Estimated Time: 20-30 minutes.
•	Estimated Cost: Free during PartyRock’s initial trial period.
🎉 The Final App
Here is DiaBeat, ready to make daily meal planning healthier, easier, and enjoyable for diabetics!
 ![image](https://github.com/user-attachments/assets/ccac3040-b866-49c4-a12a-29db4c6f6035)
![image](https://github.com/user-attachments/assets/e84326a7-599e-4fd2-b283-14d748c6ada5)

 

🌟 Inspire Your Own Project!
Feeling inspired? Here are more project ideas:
Fitness Planner: Personalized workouts
Mental Wellness App: Tailored mindfulness activities
Budget Manager: Smart financial planning tools
Your unique app can genuinely change lives—start building today! 🚀
