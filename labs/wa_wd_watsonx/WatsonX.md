**watsonx.ai Environments**

First to access ibm watsonx dataplatform and use prompt labs please use the below link
[https://dataplatform.cloud.ibm.com/wx/home?context=wx](url)

**To open the Prompt Lab, from the watsonx.ai home page, choose a project, and then click Experiment with foundation models and build prompts.**

**Prompt editor**
You type your prompt in the prompt editor which looks like below. The prompt editor has two modes: freeform and structured.

<img width="1433" alt="image" src="https://github.com/cloud-native-toolkit/watsonx-workshop/assets/73220577/5123fff2-f151-4f64-9671-cc8427843b29">

**Freeform mode**
For a plain text editing mode, click Freeform. When you click Generate in freeform mode, the prompt text is sent to the model exactly as you typed it.

**Structured mode**
To enter different parts of your prompt in separate text areas, click Structured.

Instruction: In the Set Up section, you can specify an instruction, if it makes sense for your use case. An instruction is an imperative statement, such as "Summarize the following article."
Examples: Also in the Set Up section, you can specify one or more pairs of example input and the corresponding desired output. If you need a specific prefix to the input or the output, you can replace the default labels, "Input:" or "Output:", with your desired labels. (Providing a few example input-output pairs in your prompt is called few-shot prompting.)
Test input: In the Try section, you can enter the final input of your prompt.
When you click Generate in structured mode, the text from the fields is sent to the model in a template format.

**Prompt engineering**

**PROMT 1 Test**

---------------

Model: google/flan-ul2
Parameters: {
    "decoding_method": "greedy",
    "repetition_penalty": 2,
    "stop_sequences": [
      "##"
    ],
    "min_new_tokens": 50,
    "max_new_tokens": 200,
}

You are an analyst who verifies the call transcript based on a checklist provided to you and writes a short summary with important details.  Your task is to read the call transcript surrounded by triple quotes, write a short summary in complete sentence only from given transcript and also answer following questions in the checklist and write in the output summary.

Checklist Questions:
1: Did the Virtual Agent verifies customer name and email ?
2: What was the issue customer facing ?
3: Was the issue resolved ?
4: What was the overall sentiment of the transcript, neutral, negative or positive ?
5: Did customer ask to connect to a live agent ?

Call Transcript:
"""
1) [Virtual Agent]: Thank you for your inquiry.  NetPro will automatically answer frequently asked questions! Select the inquiry menu or enter your question in a short sentence.
 - Installation Help
 - Troubleshooting
 - Subscribe to Gearheads
 - Subscribe to Pro Support

2) [Customer]: I'm facing issues with internet connectivity on my modem router
3) [Virtual Agent]: As I can understand you have an issue experiencing connectivity issues with your cable modem or modem router, correct?
 - Yes
 - No

4) [Customer]: Yes
5) [Virtual Agent]: Please provide your complete name

6) [Customer]: John Smith
7) [Virtual Agent]: Please share your email Id as well for verification

8) [Customer]: john.smith@example.com
9) [Virtual Agent]: Thank you for verification, I see that you do not have any devices registered with the details you provided. If you have not registered the new devices, I can help you with that. Shall we proceed with the registration?
 - Yes
 - No

10) [Customer]: Yes
11) [Virtual Agent]: Please follow below steps to register your product:
Register new device

12) [Customer]: I've just registered my modem CR2000
13) [Virtual Agent]: Thank you for registering your product, now let's get the issue resolved. From your description, you need help with following query:

<br />





I have an issue with internet connectivity.
 - Yes
 - No

14) [Customer]: yes
15) [Virtual Agent]: As I can see the recent device you registered is below, correct ?

<br />





**CR2000**
 - Yes
 - No

16) [Customer]: yes
17) [Virtual Agent]: Please follow below instructions for resolving the internet connectivity issues:
Internet connectivity issues steps
Is the issue resolved now ?
 - Yes
 - No

18) [Customer]: no I'm still not able to connect to internet
19) [Virtual Agent]: I'm sorry to hear that you are still facing problems.  Would you like to connect to an Agent for helping you with the issue you are facing ?
 - Yes
 - No

20) [Customer]: Yes
"""

Output Summary:

---------------------


INSTRUCTION: 
You will be given a list of product reviews. Your task is to generate a short summary, only from given product reviews from an ecommerce site to give feedback to another customer.

EXAMPLE 1: 
INPUT: 
1: I am very happy with the way it cleans, and the fact that it is energy efficient.\n2: Love it! Very efficient. Best washer I’ve owned. Clothes come out almost dry.\n3: Excellent choice for us. Home depot Thanksgiving deals were fantastic to buy a washer and dryer. Device wise looks pretty efficient with water usage, which is the primary concern for us economically and environmentally speaking.

OUTPUT:
Here are some key points from the given customer experiences:\n\nThe customers like how efficiently their clothes get cleaned and comes out dry by using less electricity/water than previous models they have used in past. 

TEST:
It really performs great and it is very easy to operate.

Plenty of room to wash my California King comforter. The vast range of settings are wonderful and the memory setting gives my kids the ability to use it with pushing 1 button.

I love this GE Washer that I just purchased with the matching dryer. It's efficient, easy to use, and fits well.

Great reliable washer for a small family and easy to use!

It is quiet, easy to learn to use. strong and many washing option




