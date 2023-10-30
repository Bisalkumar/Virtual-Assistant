
# Virtual Assistant   
 This project is created only for those who are interested in building a Virtual Assistant. Generally, it took lots of time to write code from scratch to build a Virtual Assistant. So, I have built a Library called "JarvisAI", which gives you easy functionality to build your own Virtual Assistant.    
# Content-    
    
1. What is JarvisAI?    
2. Prerequisite    
3. Architecture  
4. Getting Started- How to use it?    
5. What it can do (Features it supports)    
6. Future / Request Features    
7. Contribute    

  
## Premium Plan-

What is our premium plan?

- AI will be able to understand all your commands. It will answer all your questions apart from below basic intent.

- It will be able to handle intent- 'others / Unknown Intent'. Free plan doesn't support this.

- It will be automatically upgraded to use GPT-3 based model in the future. Currently, it uses other advance custom AI models to answer queries.

- Currently unlimited API calls. Later we might change / limit.

- Currently, it doesn't remember the previous context of the chat, but soon it will be. We don't store your
        personal chat information.

**Check out our plan: https://jarvisai.in/dashboard**


## YouTube Tutorial-  
  
Click on the image below to watch the tutorial on YouTube-  

**Tutorial Latest-**

[![JarvisAI Tutorial 1](https://img.youtube.com/vi/hPE-kdRmYf8/0.jpg)](https://www.youtube.com/watch?v=hPE-kdRmYf8)  

  
**Tutorial 1-**  
  
[![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
  
**Tutorial 2-**  
  
[![JarvisAI Tutorial 2](https://img.youtube.com/vi/6p8bhNGtVbA/0.jpg)](https://www.youtube.com/watch?v=6p8bhNGtVbA)  
  
  
    
## **1. What is Jarvis AI?**    
 Jarvis AI is a Python Module that is able to perform tasks like Chatbot, Assistant, etc. It provides base functionality for any assistant application. This JarvisAI is built using Tensorflow, Pytorch, Transformers, and other open-source libraries and frameworks. Well, you can contribute to this project to make it more powerful.    
  
* Official Website:  [Click Here](https://jarvisai.in)    
    
* Official Instagram Page:  [Click Here](https://www.instagram.com/_jarvisai_)    
    
    
## 2. Prerequisite    
 - Get your Free API key from  [https://jarvisai.in](https://jarvisai.in)    
        
- To use it only Python (> 3.6) is required.    
        
- To contribute to the project: Python is the only prerequisite for basic scripting, Machine Learning, and Deep Learning knowledge will help this model to do tasks like AI-ML. Read the How to Contribute section of this page.  
  
## 3. Architecture  
  
The JarvisAI’s architecture is divided into two parts.  
  
1. User End- It is basically responsible for getting input from the user and after preprocessing input it sends input to JarvisAI’s server. And once the server sends its response back, it produces output on the user screen/system.  
2. Server Side- The server is responsible to handle various kinds of AI-ML, and NLP tasks. It mainly identifies user intent by analyzing user input and interacting with other external APIs and handling user input.  
  
   ![JarvisAI’s Architecture](https://cdn-images-1.medium.com/max/800/1*_PK8b96tBgRHlmZecli-nA.jpeg)  
  
  
## 4. Getting Started- How to use it?    
    
#### NOTE: Old version is depreciated use latest version of JarvisAI

 ### 4.1. Installation-  
  
* Install the latest version-    
  
	```bash  
	pip install JarvisAI  
	```   

#### Optional Steps (Common Installation Issues)-  
  
* [Optional Step] If Pyaudio is not working or not installed you might need to install it separately-  
     
   In the case of Mac OSX do the following:  
     
	```  
	brew install portaudio  
	pip install pyaudio  
	```  
 
 In the case of Windows or Linux do the following:  
     
   - Download pyaudio from: lfd.uci.edu/~gohlke/pythonlibs/#pyaudio  
     
   - ```pip install PyAudio-0.2.11-cp310-cp310-win_amd64.whl```  
  
* [Optional Step] If pycountry is not working or not installed then Install "python3-pycountry" Package on Ubuntu/Linux-  
		 
	```  
	sudo apt-get update -y  
	sudo apt-get install -y python3-pycountry
	```  
 

* [Optional Step] You might need to Install [Microsoft Visual C++ Redistributable for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#microsoft-visual-c-redistributable-for-visual-studio-2022)  
  
### 4.2. Code You Need-  
   
   You need only this piece of code-
	
	
    import JarvisAI

    def custom_function(*args, **kwargs):
        command = kwargs.get('query')
        entities = kwargs.get('entities')
        print(entities)
        # write your code here to do something with the command
        # perform some tasks # return is optional
        return command + ' Executed'
    
    
    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
                           google_speech_api_key=None, backend_tts_api='pyttsx3',
                           use_whisper_asr=False, display_logs=False,
                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
    JarvisAI.add_action('custom_function', custom_function)
    jarvis.start()	
  
   
 ### 4.3. **What's now?**    
    
 It will start your AI, it will ask you to give input and accordingly it will produce output.      
   You can configure  `input_mechanism` and  `output_mechanism` parameter for voice input/output or text input/output.    
    
   ### 4.4. Let's understand the Parameters-    
    
For text input-
    
    input_mechanism='text'

For voice input-
    
    input_mechanism='voice'

For text output-
    
    output_mechanism='text'
    
For voice output-
    
    output_mechanism='voice'

For voice and text output-
    
    output_mechanism='both'
     

## 5. What it can do (Features it supports)-    
    
1. Currently, it supports only english language    
2. Supports voice and text input/output.    
3. Supports AI based voice input (using whisper asr) and by using google api voice input.    
4. All intellectual task is process in JarvisAI server so there is no load on your system.    
5. Lightweight and able to understand natural language (commands)    
6. Ability to add your own custom functions.    
    
### 5.1. Supported Commands-    

These are below supported intent that AI can handle, you can ask in natural language.

**Example- "What is the time now", "make me laugh", "click a photo", etc.**

**Note: Some features / command might not work. WIP. Tell me bugs.**

 1. asking time 
 2. asking date 
 3. greet and hello hi kind of things goodbye
 4. tell me joke
 5. tell me about 
 6. i am bored 
 7. volume control 
 8. tell me news
 9. click photo 
 10. places near me 
 11. play on youtube 
 12. play games 
 13. what can you do 
 14. send email 
 15. download youtube video 
 16. asking weather 
 17. take screenshot 
 18. open website 
 19. send whatsapp message 
 20. covid cases 
 21. check internet speed
 22. others  / Unknown Intent (Premium Feature)

  
### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    

You can set below parameter while creating object of JarvisAI-

    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
                           google_speech_api_key=None, backend_tts_api='pyttsx3',
                           use_whisper_asr=False, display_logs=False,
                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
    
1. **For text input-**'    
    
		input_mechanism='text'
       
2. **For voice input-**    
   
		input_mechanism='voice'
    
3. **For text output-**    
    
	    output_mechanism='text'
    
4. **For voice output-**    

	    output_mechanism='voice'

5. **For voice and text output-**    

	    output_mechanism='both'
       

    
 ## 7. Contribute-    
  
  1. Clone this repo.
  2. Create your file in JarvisAI/JarvisAI/features/<your_file.py>
  3. Write entry function like this-
  
  	
	def some_func(*args, **kwargs):
	    query = kwargs.get("query")
	    entities = kwargs.get("entities")
	    li = ['EVENT', 'FAC', 'GPE', 'LANGUAGE', 'LAW', 'LOC', 'MONEY', 'NORP', 'ORDINAL', 'ORG',
		  'PERCENT', 'PERSON', 'PRODUCT', 'TIME', 'WORK_OF_ART']
	    topic = [entity[0] for entity in entities if entity[1] in li][0]
	    return "This Code Done"
	
  - query is the text that is recognized by your microphone
  
  - entities Named Entity Recognition is a technique of natural language processing that is used for the categorization of the data
  
  - Example-
	
	query: who is Narendra Modi

	entities: [('Narendra Modi', 'PERSON')]
	
	topic: Narendra Modi
 
 	So, now you got the topic from query and now you can play with the topic.
 
  4. Your function can return someting text or perform something. Return text will be automatically print / spoken by your system.
  5. In JarvisAI/JarvisAI/features_manager.py , import and add your function like this
 	
	try:
    		from features.your_file import some_func
	except Exception as e:
		from .features.your_file import some_func
	
	action_map = {
		.....
		....
		'your_intent': some_func
	}
	
  6. That's it now raise pull request. I'll verify your code. If working, ethical and all terms are followed, I'll approve.
  7. You will become contributer.
    
    
## 9. Donate-    
 
Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!

    
**_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
 **_Mention below line for credits-_**    
 ***Credits-***    
 - [https://jarvisai.in](https://jarvisai.in)    


## License    
 [MIT](https://choosealicense.com/licenses/mit/)
