# SaucedemoProject

Steps to run and Test the Semodemo Project:

Step1: download the saucedemo.zip project (due to some SSH problem and access isuue as i am using my company laptop , so, i had to upload project via creating zip).
Step2: open project in IntelliJ or any other other IDEA
step3: build porject - open Maven - (see right side) and do clean install
step4: check if build is succesfully completesd- finished with exit code 0
step5: then GO to src/test/java/org/com/testcases/SaucedemoTestPage.java 
step6: right click and run the test (cltr+shift+F10)
step7: once test is done, check the test result and steps in Run, then it will start executing the steps in Chrome.
Step8 : once done and if its passed, it will show ,( Total tests run: 1, Passes: 1, Failures: 0, Skips: 0) in Run.


Exercise 4:

1) Generally first we have to find tools , which tool/lib is easy and best to automated but in genearal steps I will follow as below.
First I will test the endpoint and status manually to understand the behaviour and scenarios. 
Creating the method for verify the good weather test with status code (200) , by proving endpoint and diffent scenarios.
Simillary , for the bad weather/input inputs and validate the status code(400,404 ) against the input provided.
Testing with the different method, in this case - it is GET method.
also, Validate the response body based on the status code .




2) Test cases:
a)Return value based on input condition : maily covering good weather scenarios (available , pending and sold), execute the scenarios and validate the response.(statusa code 400)
b) providing Multiple status values and validate the status code and response.
b)Does not return anything- empty
c)Bad weathere scenarios: proving wrong input- (anything out of good weather scenarios) and check the status code 400.
d)Modify certain resources: Invalid input and Method etc and validate the response.
e)Authenciation cases: probably Updating data structure will have some outcome or effect on the system, and that should be authenticated

3) It depends upon the tool we use :
for this scenario, we can also use directly with for loop and Java lib. 
but also we can rest assured lib 
if we use Java script: Super Test, Mocha BDD etc but in my experince tools having inbuit lib to validate various responses.
