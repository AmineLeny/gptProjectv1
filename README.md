# gptProject

I'm gonna explain  the python script







<img width="532" alt="Screenshot 2023-12-24 at 16 54 53" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/09c3c912-625c-4cce-92a4-d67075975850">




These lines import necessary libraries and modules : os,fastapi,openAI,csv,dotenv 

the load_dotenv()  load the environment variable stored in the .env file that contains our secret gpt api key [ I did this for security purposes ] 


<img width="173" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/87abd49d-bf86-444e-aedd-d8fb3de31002">

here I created an instance of the FastApi() class i named it app







 


<img width="154" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/3031cf60-6a3d-4404-b35a-5e0c1bacc244">

This line initializes an empty list messages. This list will be used to keep track of the conversation between the user and the assistant.


<img width="293" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/e06c3dca-a2e7-4e13-ac90-8b476ab95155">


This line defines a class named ChatGPTMicroservice.



<img width="625" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/8c5f13d8-e63f-4865-918a-fd6c1972daec">

This is the constructor method of the ChatGPTMicroservice class. It initializes an instance of the class with an OpenAI API key and a default data directory. It also sets the csv_file attribute to the path of the CSV file where the conversation data will be stored.



<img width="828" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/6775786d-287b-4951-b596-1889176bd2b2">

    
This method is used to query the ChatGPT API with a user's question. It appends the user's message to the messages list, sends the message to the OpenAI API, and stores the generated response in the messages list as well. It then calls the save_to_csv method to save the conversation to a CSV file.


  <img width="840" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/21d3bc14-0ce0-4dab-adad-e3242dcc3613">

    

This method is responsible for saving the conversation to a CSV file. It opens the CSV file in append mode, creates a DictWriter object, and writes a new row to the CSV file with the question and answer.


<img width="951" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/07b38003-c87c-40a2-a8df-0a202723c9d4">



This is a FastAPI route definition. It specifies an HTTP POST endpoint at the path "/ask". The endpoint takes parameters for the question, model, max_tokens, and temperature. It creates an instance of the ChatGPTMicroservice class, queries the ChatGPT API, and returns the generated response. If an exception occurs, it raises an HTTP 500 exception with the details of the error.





