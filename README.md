# What is A/B testing
The A/B testing is a data driven testing method used to test a different version of an application simultaneously. These versions could be a small change in UI, change in sentiment of text or testing out optimize difficulty level of a mobile game. The test is conducted with two or more variants in an application and collecting the relevant data. The slightly different version of the app will randomly distribute to the assigned test group. All the action, behaviour of the test group will be tracked closely to obtain all relevant data. Then a statistical analysis is conducted to test whether the change is significate enough to make an improvement over the control or another test group. The statistical analysis could allow the developer to adjust to the preferences of the majority of the user in an objective manner.


# When to do a A/B testing
A/B test could be conduct when there is controversial between app developer. The experience of developer is subjective and different users might have different preferences. A/B testing provide a cost effective method to experience. Focus group or user reviews to help when developing application. However, focus group requires relatively longer time to conduct and the simple size are small. While user review could provide insight that developer might overlook, opinion in review could be polarizing and provide not enough details about the issues. The A/B testing could provide preference of majority of user with supporting data. A/B testing could also be used as a pilot program to test out new feature.


# Reason to conduct A/B testing
A/B testing provide a data driven way to verify the change of will have a good chance to lead to good result (e.g. increase in time span in app). The testing allow application to increase in active, boost the retention rate of user all with an objective and measurable way. In the current fast-pace society, constant update in the application in essential. Though with the inappropriate change, the application might lose a huge amount of user and it takes a long time to gain it back. The A/B testing allow developer to test certain features or changes with a relatively small  amount of user, to ensure the change is beneficial.


# Example of A/B testing
1.  UI change
    - The preference of user could be tested by A/B testing, by changing different color of the button, font size and measuring the preference, developer could conclude the most popular layout at the time.


2.  Notification
    - A/B testing also allow the developer to send different notification to different testing group. By sending different notification (or no notification) to different testing group. A/B test could conclude the optimum number of notification and content that most of the user prefer and result in a popular application.


3.  Change in style of writing
    - The title and text in a media application is essential to the success. Using A/B test, the more popular style of writing could be found by measuring different click rate and conversion rate in different testing group.


# Conduct the A/B testing using Firebase
Firebase provide a simple integration of A/B testing, result verification.


1.  Using Firebase remote config to change in UI
    - Firebase remote config allow developer to conduct the A/B test to UI change. The developer first define a default value the parameter enable Firebase remote config (e.g. background color code). The value will the default value of the parameter is shown if there is no change in remote config or the application user is not connected to the internet. If the user is in the testing group and have an internet connection a JSON file send as string and decode locally. The relevant parameter will change the value accordingly


2.  Using Firebase Cloud Messaging to test notification
    - Firebase Cloud Messaging allow developer to send, by designing different testing group, the developer could assign the particular notification to a given test group and measure the effectiveness of notification
Potential issues associate with doing A/B testing


3.  Sampling error
    - Firebase allows us to choose groups of user to be tested. Bias might influence the resulting , causing the conclusion to be made. To mitigate the effect of sampling problem, an A/A testing could be ran prior to the A/B testing. An A/A testing is conducted by two or more test groups with no change in feature or UI, the result should have small to no difference in performance. If there is a significant different of measure, the testing group has to be selected in a different way.


4.  Firebase could not operate in some countries
    - In country like China, Cuba, Iran, North Korea, most of the Google services are banned prohibited. While conducting A/B testing, countries that banned Google services should be exclude from the testing in order to obtain a result or alternative platform have to be deployed to perform A/B testing.


5.  A/B test might incur bug
    - A/B test that contain unknown bug might discourage user to use and try the app again losing potential customers. Minimise the test group to 5-10% could result in less affect to the user community.


6.  Not all users are willing to Participate in testing experience
    - Conducting A/B test without the user consent or aware might result in consumer dissatisfaction. The dissatisfaction might be amplified by media result in huge consequences


7.  Short term performance might not translate to long term effect
    - Even if the change yield a good result with the supporting data, the performance increase might just be driven by novelty (unseen change) but not by the change itself. The performance of the change might need a longer time to observe in order to make a holistic conclusion.
For multivariate testing that contain result might not be clear or misleading
A/B testing allow more than two variants in one testing. However with a testing that consist of multicable variate, the result might not be easily concluded, the causality and correlation might be ambitious.


8.  Metric to test the effectiveness of change in A/B testing
    - Firebase analytics could be used to track the performance and other parameter to understand the result in A/B testing 


9.  Average Time span
    - The increase in average time span with the change means the change is advantageous, the change result in a decrease in average time span is disadvantageous


10. Number of active user
    - The increase in number of active user with the change means the change is advantageous, the change result in a decrease in number of active user is disadvantageous


11. Retention rate
    - The increase in retention rate with the change means the change is advantageous, the change result in a decrease in retention rate is disadvantageous


12. Crash rate
    - The decrease in crash rate is desirable, increase in crash rate is undesirable


13. Occurrence of an event
    - The increase and decrease event occurrence could be both desirable and undesirable depends on the experience hypnosis


14. In-app purchase
    - The increase in In-app purchase with the change brings more income means the change is advantageous, the change result in a decrease in In-app purchase is disadvantageous
