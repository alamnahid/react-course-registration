
## Live Link: http://husky-lawyer.surge.sh/

#### Add at least 3 Project features

* This project shows 9 courses details that are dynamically loaded from a json file with the API.

* User can select courses, selected course name, total credit, total price will be shown on the course card.

* User can take a total 20 credits if user wants to take more than 20 credits course then a toast will show that your credit limit is over.


#### Discuss how you managed the state in your assignment project.

Use state is one of React hook which returns an array of two values. One is the current state and the other is the updated state. I put a default value of useState.

#### The states I used in the assignment project are:

* First I used state to dynamically load the courses from the JSON file and put the fetched data into setCourses(). I have taken an empty array as the default value of this state. This state return the course lists from the JSON file.

* For selected course I created a use state. When user can select any course after that the data of the selected course will be updated on setSelectedCourse() state. I have taken an empty array as the default value of this state, all the selected courses will be stored in this array.

* Declare a state to show total credit. Here, the default value of the state is zero, when the user selects any course, every time the value of the state is updated, the credit of the course will be added to the state. By doing this I am getting total credit from this state.

* I have declared a state to calculate the total price. The default value of which is taken as zero. When the user selects the course, the price of the course will be added here and the value of the state will be updated and the total price of all the courses will be returned.

* The state I declared lastly is to calculate the remaining credit. User can take total 20 credit. So, I have taken this stated default value twenty, when the user selects a course, the credit of his selected course will be subtracted from twenty. When the credit reaches 20 he can't take any more courses and the value remains after subtraction I will get a return of the value from the state.

* And I used UseEffect to load the data dynamically


"# react-course-registration" 
