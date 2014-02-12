AndroidJSON
===========

**************************************************************
Lesson learnt and Initial thoughts on Android development:
**************************************************************
1)Eclipse- JAVA and XML-based programming languages

Initial Thought: 
First of all, in order to familiar to the programming languages of the Eclipse, I developed the simple Android Application, displaying the "Hello World" in TextView. 

Lesson learnt: 
This was my first time to use Eclipse to read JSON data from endpoint and display it in the app. I found it very challenging. I have learnt JAVA and XML-based programming languages to insert the text into the TextView using “setText”, and create the On-Click event.  

2)GUI Interface of Android Application

Initial Thought: 
Initially, I started to drag the TextView and Button into the form. Then, I tried to set the id, gravity, text size, and text style of the textView using XML languages. Besides, I created the TableLayout using XML language. 

Lesson learnt: 
There is a drawback if everything was done by using XML programming language. For example, to display JSON Data in table form, I need to create and named the id of TextViews of each rows of the table in XML language. Besides, I need to declare variables to get the id of the TextViews of each row in order to modify the texts of TextViews. The code will be very long and messy. Therefore, I performed all the actions using JAVA programming languages through looping method: adding rows and columns of the table, and set Id, text Size, gravity of TextSize. 

3)Display JSON data

Initial Thought: 
Instead of reading and extracting data from endpoint, I started to create simple JSON string in order to verify the workability of the coding. I started to perform simple action that is getting the values of the JSON data by entering the keys.

Lesson learnt:
However, there is a disadvantage by just obtaining the values through entering the keys. This method is not feasible once the JSON data is large. Therefore, I have figured out the solution that was using looping method to loop through the JSON data lines by lines, then, display the keys and values of data in table form.  

4) Connect to and read data from endpoint

Initial Thought:
In order to connect to the web service, I have added  "uses-permission android:name="android.permission.INTERNET"/" into the AndroidManifest.xml. By using try and catch method, exception error was caught and displayed on the TextView. Still, I encountered unknown problems which cause the crash happened on android applications. Other than that, the difficult problem that I was facing in this task was:"NetworkOnMainThreadException" exception. This exception prevented the Android Application from obtaining the data. 

Lesson Learnt:
If there was any crash happened while launching the application in phone, I have learnt to solve the problems by viewing the LogCat. With this, I was able to determine source of error. For example, "NetworkOnMainThreadException" error was detected while I debugging the code. I have learnt to use asnyctask in order to read data from the endpoint and solve the "NetworkOnMainThreadException" problem. 

************************************************************
Additional comment on room of improvements of my application:
************************************************************
1) JSON data is able to be displayed in orderly manner according the JSON data of endpoint. 

2) The numbers of rows and columns of the table are created based on the size of JSON data

3) JSON data is able to be displayed nicely according to the endpoint entered by the user
