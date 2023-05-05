Download Link: https://assignmentchef.com/product/solved-cse102-homework-10
<br>
<span class="kksr-muted">Rate this product</span>

Write a complete program achieving all the tasks below.

• The program takes a single argument as the name of the file to be read. A sample file is attached (Movies.txt). The program reads this file which has labeled columns separated by commas. Every row of this text file includes information about a movie. You are asked to read every row as a string and decompose the given information (separated by commas).

• The following shows a few entries of this file in table format.

Figure.1 Movie List Example

• You should use the following structure to keep the information for each movie.

Figure.2 Movie Struct

Page 1 of 5

<ul>

 <li>The program should keep the movies in a dynamically allocated struct array. There should be exactly the same number of elements in this array as the number of lines in the file.o Note that the file may have multiple lines for the same movie. You should check this with movie name. If the name is already read and stored in the array, the data should be updated with the new data.</li>

 <li>The program should keep the movie names (can be of arbitrary length) in a dynamically allocated string.</li>

 <li>The number of movies in the Movies.txt file is unknown.</li>

 <li>The program must convert the movie types/genres to a unique numeric value (integer). Youcan start assigning integer values starting from 1 and increase is as new movie types are read.</li>

 <li>Some of the movies has no value for ‘budget’ column. In this case the string ‘unknown’ is used.Part 1: The program should support 8 different operations. Therefore, there should be a menu like the one below. The program should be terminated if and only if the user enters “8” as input. If an entry is invalid or the previously requested action has been taken, the menu should appear repeatedly. If the menu appears due to an invalid entry, there should also be an error message.Part 2: If the user enters ‘1’, the program should return the specified number of movie records, sorted by the selected area. As stated in the first section, if the user enters a wrong value in these selection steps, you should be directed to a new one in order to enter the correct one. If the user selects a single selection, you must return a single record. If the user selects more than one selection, you must fetch all records in the specified range. All rankings must be made in ascending order. Don’t forget! In the first selection, you will choose according to which field it will be sorted.</li>

</ul>

Page 2 of 5

Part 3: 2nd operation lists the movie genres/types as strings, if the user enters “2” as input, the program should list the genres/types as strings.

Part 4: 3rd operation lists the movies based on the information received from the user. The program asks for a “year” first, after that program asks “until that year or since that year?”. Finally, the program lists the names of all movies that have been aired until / since that year. Note that the program must handle invalid year or period values. So, if the oldest movie was released in 2000 and the user wants to print the movie that was released until 2001, the program should display an error message and request new values as there were no movies before 2001.

Page 3 of 5

Part 5: 4th operation lists the movies according to an information received from the user. Firstly, the program asks for a ‘score’, after that the program asks ‘less or greater than that score?’. Finally, the program lists the names of all movies whose score is less / greater than that score. Don’t forget that the program should handle the invalid score or comparison values. So, if there is no movie with a score below 4.7 and the user wants to print movies with a score below 4.7, the program should display an error message and ask for new values because there are no movies scored below 4.7.

Part 6: 5th operation asks for a movie name from the user. If the input matches with a name from the array, then the program prints all information of that movie. If the input doesn’t match with any element of the array, then it should give an error message and ask for a new input. If the ‘budget’ information of that movie was ‘unknown’ when the program read it, then the users should see it as ‘Unknown’.

Part 7: 6th operation basically calculates and prints the average of the IMDB scores of all movies. This value is for example purposes only. The actual value of the file given to you will be different.

Page 4 of 5

Part 8: 7th operation printing the frequence of every genre. I.e. print the number of movies for every genre. These values are for example purposes only. The numbers on the file given to you will be different.

❖ You are not allowed to use any library other than; ➢ &lt;stdio.h&gt;

➢ &lt;string.h&gt;