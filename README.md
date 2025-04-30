# Task Round for Better
## Software Engineering (Applied AI) Work From Home Internship 
### Details :
Build an AI-powered tool that:
1. Takes code snippets as input and identifies potential performance bottlenecks.
2. Provides suggestions for optimization.
3. Includes a basic interface for users to upload and view results.

### Images :-
Input :
![image](https://github.com/user-attachments/assets/bcee48f4-ebb4-4d8b-b924-60229a0a011a)

Output :-
![image](https://github.com/user-attachments/assets/13de934d-9ae1-4344-a78f-2afa47b83d09)

### Working :- 
Download the repository in your desired directory by running the command 
```git clone https://github.com/Just-a-random-username/Better-Task-Round/```

Download the required python libraries :-
```
pip install -r requirements.txt
```

Run the code using :-
```
streamlit run [Installation Directory]/Better-Task-Round/Streamlit.py
```
or open terminal in Better-Task-Round folder and run :-
```
streamlit run Streamlit.py
```
This will open a browser window in which you can 
- Enter input prompt and guide the LLM to do the task required OR
- Upload a file which will automatically get read by the code, converted to a prompt, and improved by LLM

### Design Choices :-
The design of this project is kept simple, with only functionality being text input prompt and a file upload prompt.
The project does not keep conversation history, so each prompt has to be individually typed, and previous prompts and outputs can not be referred to again.

### Assumptions Made and Limitations:-
- Lack of conversational memory as LLM is only for code improvements.
- Limited context window size - Upto 32,768 tokens
- Accuracy Limitations :- The LLM model used is of a small size (1.5B Parameters), which would affect the output quality. The compromise on output quality had to be made due to hardware limitations of my personal device, however a more trained and larger model will produce a better output

### Tools used and References :
- LLM Model : Qwen2.5-Coder-1.5B-Instruct developed by Alibaba Cloud
- Streamlit for UI elements
