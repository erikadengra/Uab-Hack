## Inspiration
The inspiration of this challenge came from the growing need for effective tools to help students optimize their academic performance through data intelligence. Our goal was to leverage algorithm-based optimization and predictive analytics to give students a clearer view of their progress, making the most of the information available on platforms like Moodle. 

## What it does
Is an academic optimization tool that uses advanced algorithms to analyze diverse educational data, providing personalized recommendations for students. Based on their grades, submitted assignments, and participation, it predicts performance and suggests actions to maximize results according to each student's profile and study habits. 

## How we built it

Starting from the data, we selected those features that seemed most relevant to academic performance. We removed all null values and filtered out any outliers to ensure data consistency, and remove all values that we did not consider relevant or did not have enough values (e.g. partial grades). We then created new columns for variables we considered relevant and standardized the dataset to prepare it for modeling. 

Initially, we trained a regression model to predict students grades. However, due to insufficient statistical strength, we decided to add additional data on assignments types. This revealed a modest correlation between the type of assignment a student completed and their final grade, though it was not yet sufficient for reliable prediction. This observation suggests that including metadata about assignments could provide further insights. 

Moreover, we hypothesize that other variables (such as the student's economic status, personal situation, and sleep hours) might be highly relevant to more precise predictions. These additional data points could help us refine the model and uncover new patterns impacting academic performance.

## Challenges we ran into

One major challenge was cleaning and preprocessing Moodle data, as these datasets can be complex and often incomplete. Initial attempts with a regression model revealed limited predictive power, leading us to explore additional metadata about assignment types, which highlighted the need for more comprehensive data, such as socioeconomic factors.

## Accomplishments that we're proud of

We're proud to have identified key indicators that influence academic performance, particularly the link between assignment types and grades. Despite limited data, our adjustments to the model revealed insights that could be further developed. Additionally, our ability to adapt our approach mid-project, incorporating additional variables to increase model reliability, demonstrated our flexibility and commitment to finding the best solution. 

## What we learned

This project taught us the importance of an interative approach to data analysis. We learned that predictive modelling in education requires more than just grades and assignments, it benefits greatly from a holistic view of a student's context. Furthermore, the need for extensive metadata in academic predictions became evident, reinforcing the value of data diversity in AI models. 

## What's next for  Algorithm-Based Academic Optimization.

Our next steps include to integrate more complex metadata, such as socioeconomic background, personal challenges, and lifestyle habits, to enhance model accuracy. We also plan to collaborate with educational institutions to obtain more diverse datasets and refine our algorithms. Ultimately, we aim to develop a comprehensive tool that can support students by predicting academic outcomes more accurately and suggesting actionable steps for improvement. 
