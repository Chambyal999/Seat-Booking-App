Problem statement
For the given HTML and CSS for the website implement your Javascript to build a working Seat Booking App.


Expected Output:


Requirements:

1- Using the given MovieList Array update the dropdown menu and append it to the select element with class "selectMovie".

2- Each option created should have an event attached to it.

3- The event should do the following operation:-

-update the movie name and movie Price on the elements with the id "movieName"  and "moviePrice" respectively

-change the total Price of the element with the id "totalPrice" according to the price of the Movie.
4- There should be a default Movie name as "Flash" and a movie Price as "7" which should be updated on selecting other options.

5- For the Seats:-

-You can access all seats using "#seatCont .seat" in the querySelectorAll.
-Some seats are already occupied and have class "seat occupied".
-Add event listeners to seats other than the occupied ones.
6- The event listener should add the following functionalities:-

-If the seat is not already selected select the seat and add "selected" to the classList of the seat.
-If the seat is selected deselect the seat and remove the "selected" from the classList.
-The price should be updated based on each selection of seat.
-The seat selected should be added to the element with Id "selectedSeatsHolder" to show how many seats have been selected.
7- The continue button should have an event listener which should be able to perform:-

-If there is no seat selected then the alert the user "Oops no seat Selected".
-If there are some selected seats then alert the user "Yayy! Your Seats have been booked".
-For all the seats that are selected remove "Selected" from the classList and add "occupied" to it.
-Update the Price and set it to 0.</br>
-Update the seatHolderSection to its default value which is a span with textContent "No seat Selected".
8- For the cancel button add the event listener which should be able to perform the following operation:-

-should be able to remove the "selected" from the classList of the selected seats.
-Update the Price and set it to 0.
-Update the seatHolderSection to its default value which is a span with textContent "No seat Selected".

Test Cases:-

1- Check the seat Event listener-

a- Add event listener 'click' to all the seats with class 'seat' that comes under class 'seatCont'. By clicking on seats, add "selected" to the classList of the seat. Also, store all the added classes in a separate empty array. Inside this array do all the operations. 

b- The seats with class 'seat occupied' should not add "selected" to the classList of the selected seats. Should remove class 'selected' from the classList of selected seats on deselecting the seats. 
2- Check the Price Section-

a- Update the price of the selected seats under the id 'totalPrice'. The initial price should be 0. The price should be equal to no. of seats * movie price. For Example: - For the movie Flash, if we select one seat then the price should be 7 and if we select a second seat then the price should be 14. 
3- Check the SelectedSeat Section-

a-  Create a function that checks on the array that we used earlier for adding and removing the class 'selected' in the first test case. With every click of the seats the number of seats should be updated in the section with id 'selectedSeatsHolder'. If the array is empty means there is no class 'selected' in the ArrayList then the message 'NO SEAT SELECTED' should display. 