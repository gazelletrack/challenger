# SHIFT - Technical Interview Challenge

Rather than a whiteboard interview or an automated coding test, we have each candidate perform a medium sized interview challenge. This challenge is your opportunity to show off your skills and have insight into the type of technical tasks we deal with on a daily basis at SHIFT.

### Intro to the Challenge

One of our core tools to understand team dynamics is our Perspective Tool. Perspective is a 7 minute test that determines each team member's Myers-Briggs Type Indicator or MBTI (https://www.mindfulnessmuse.com/individual-differences/understanding-myers-briggs-type-indicator). Using this information, and understanding the personality breakdown of each team member, allows for a much better understanding of why a team is having a particular problem.

For this task you will be building a simplified version of our Perspective Test.

We estimate this challenge should take less than 3 hours from start to finish. Please note that this estimate is not a time constraint. You are free to take as little or much time as you feel comfortable with, we are only giving you an estimate so you know the level of effort we expect.

As a full stack engineer you will need to work on both sides of the stack, this challenge will test your skills on both the front-end and the back-end. 

### Open Source Alternative

If you have an open source project that you would like to submit to us instead of performing the coding challenge you may send it to us instead. 

Please note that the open source project will need to demonstrate your ability to work on both the front-end and the back-end as a full stack web developer. You will need to be the primary contributor and the project should be complicated enough to show off your skills.

### User Interface Spec

- The landing page of the web application should show the user a list of questions as shown as the "Perspective Test" page in the design
    - Full Design: https://www.figma.com/file/00SYaOnpIUYLAdvhGlTz4j97/Engineer-Perspective-Test?node-id=1%3A348
    - The personality test should ask 10 questions
        - All questions should be listed on the same page when the user opens up the page

    - Each question should be displayed with 7 radio buttons
        - The radio button furthest to the left indicates a 1 value, while the radio button furthest to the right indicates a 7
    - At the bottom of the test the user should be asked for their email
    - If a user submits without answering all of the questions, they should be given an error message and told what to do
    - Once the user hits submit, their email and test answers should be sent to the server
    - The user then should be directed to their results page

- The results page should display the user's MBTI results as shown as the "Perspective Results" page in the design
    - Full Design: https://www.figma.com/file/00SYaOnpIUYLAdvhGlTz4j97/Engineer-Perspective-Test?node-id=1%3A566
    - On the left of the results box the user should see the text "Your Perspective" followed by their perspective type
    - On the right of the results box the user should see the 4 MBTI dimensions and where they lean on each dimension
        - Note: You do not need to show the degree that they lean from each side, simply coloring the box for the side that they lean on each dimension is valid for this test

### MBTI Test Spec

- Using the provided spreadsheet, display each question as a 1 through 7 rating scale.
    - A user will be asked a question, and then asked to rate on a scale of 1 to 7 how much this question resonates with them.
    - If the user ranks a 1, that means the question doesn't resonate with them at all
    - If the user ranks a 7, that means the question resonates with them fully
    - If the user ranks a 4, that means the resonance was neutral
- There are four dimensions to an MBTI test
    - EI - Extraversion (E) or Introversion (I)
    - SN - Sensing (S) or Intuition (N)
    - TF - Thinking (T) or Feeling (F)
    - JP - Judging (J) or Perceiving (P)
- Each question will determine where a user falls in one of the particular dimensions
    - This is defined per question by the Dimension column on the spreadsheet
        - The direction that the user leans is defined by the Direction and Meaning Columns
    - The result of an MBTI test looks at each of the 4 dimensions and determines which side the user leans
- The end result is the top letter for each dimension
    - If a user leans:
        - Extraversion (E) in the Extraversion/Introversion (E/I) Dimension
        - Intuition (N) in the Sensing/Intuition (S/N) Dimension
        - Thinking (T) in the Thinking/Feeling (T/F) Dimension
        - Perceiving (P) in the Judging/Perceiving (J/P) Dimension
    - Their end result will be: ENTP (Extraversion Intuition Thinking Perceiving)
    - If a user's responses to a dimension are perfectly balanced (they don't lean more to one side or another) the algorithm should default to the first option on the list 
- There is a second spreadsheet that lists inputs from users, and their expected result

Note: This is a watered down version of a MBTI test, it does not ask enough questions to give a statistically accurate result. Your personal input may vary from what you've seen other MBTI tests say, this is expected. Just ensure that the results match the expected results in the tests spreadsheet.
    
### Minimum Technical Requirements

- The written application must be a web-based application
- Data must be written to a backend database in a way that we can see user's individual answers
- Data must be connected to a user in a way that will allow us to determine a person's MBTI based on the email address they submitted with
- The test cases given as input should produce the listed result
- You may implement this in the stack that you feel the most comfortable with. Our stack is:
    - PHP7, Laravel, MySQL for the Backend
    - React.js + TypeScript + MobX for the Frontend 

# Submitting the Challenge

- Create a repository using your personal GitHub account and send us the link. That's it!

Happy Hacking!