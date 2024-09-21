<h1>API Testing Project for **Spotify**</h1>

The scope of this project is to use all  API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: **Spotify**

Tools used: Postman, Newman

Collection link: **https://drive.google.com/file/d/1U-vBnWRGsKoKYW3CoreEYuL-Ed6K1yBb/view?usp=sharing**

<h2>Tests performed</h2>

<ol>
<li>**Get Current User's Profile**</li>

HTTP method for request: **GET**<br>
Request description: **Get detailed profile information about the current user (including the current user's username)**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional,Positive and negative techniques**<br>
Response status code: **200 OK**<br>


Below you can find a picture of the API request from Postman:<br>

![Capture1](https://github.com/user-attachments/assets/72317c8b-4364-4441-ae6c-25d92e76fb7c)





JavaScript Tests:

![Capture1 2](https://github.com/user-attachments/assets/63af82af-871a-4423-a20e-74c482bc11fc)





<li>**Search for item**</li>

HTTP method for request: **GET**<br>
Request description: **Get Spotify catalog information about albums, artists, playlists, tracks, shows, episodes or audiobooks that match a keyword string**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional,Positive and negative techniques**<br>
Response status code: **200 OK**<br>

Below you can find a picture of the API request from Postman:<br>

![Capture2](https://github.com/user-attachments/assets/da7b3070-8e59-4d49-ae5e-2639c39ae536)


JavaScript Tests:

![Capture2 1](https://github.com/user-attachments/assets/06d3631d-de90-41e2-b112-944918407ee8)



<li>**Create playlist**</li>

HTTP method for request: **POST**<br>
Request description: **Create a playlist for a Spotify user. (The playlist will be empty until you add tracks.) Each user is generally limited to a maximum of 11000 playlists**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional,Positive and negative techniques**<br>
Response status code: **201 created**<br>

Below you can find a picture of the API request from Postman:<br>

![Capture3](https://github.com/user-attachments/assets/68a6ca09-f255-4aba-b9e9-564b25d8a7d5)


JavaScript Tests:

![Capture3 1](https://github.com/user-attachments/assets/3c600efe-5481-4596-b08c-8c1f7b9b025c)




<li>**Save shows for current user **</li>

HTTP method for request: **PUT**<br>
Request description: **Save one or more shows to current Spotify user's library**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional and Positive techniques**<br>
Response status code: **200 OK**<br>


Below you can find a picture of the API request from Postman:<br>

![Capture5](https://github.com/user-attachments/assets/6c2eda91-3b2b-4057-981f-663a05879421)


JavaScript Tests:

![Capture5 1](https://github.com/user-attachments/assets/1e157fa3-f5a8-4858-8466-65f1fde9bbad)



<li>**Remove user's saved tracks**</li>

HTTP method for request: **DELETE**<br>
Request description: **Remove one or more tracks from the current user's 'Your Music' library**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional and Positive techniques**<br>
Response status code: **200 OK**<br>


Below you can find a picture of the API request from Postman:<br>

![Capture6](https://github.com/user-attachments/assets/c2953f84-7d94-492b-ab6f-649b8615310a)


JavaScript Tests:


![Capture6 1](https://github.com/user-attachments/assets/4bd5d6de-3cb6-4605-bfb5-1b9990433a73)



<li>**Get featured playlists**</li>

HTTP method for request: **GET**<br>
Request description: **Get a list of Spotify featured playlists (shown, for example, on a Spotify player's 'Browse' tab)**<br>
Test types / techniques used: **Black Box Testing - End2End, Functional and Positive techniques**<br>
Response status code: **200 OK**<br>


Below you can find a picture of the API request from Postman:<br>

![Capture4](https://github.com/user-attachments/assets/765abcce-be3f-4049-951a-e33b0ca533d2)


JavaScript Tests:

![Capture4 1](https://github.com/user-attachments/assets/6a494f8b-c9f3-4422-9065-53707497e1ca)




</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>

![Postman Spotify](https://github.com/user-attachments/assets/5e9aa8ed-2465-42fe-884d-91175af10d7a)



The collection was also run through newman directly from the terminal, and the results can be found below:<br>


![newman run](https://github.com/user-attachments/assets/e0ab681f-1056-4c42-a43f-7bb871fe4fa9)


<h2>Defects found</h2>

The following issues were identified while running the postman tests:<br>

[Jira-all bugs.pdf](https://github.com/user-attachments/files/16920243/Jira-all.bugs.pdf)


<h2>Conclusions</h2>

Following the testing of the Spotify application using the Spotify API, here are the conclusions:

- Number of tests created and executed: Approximately 60 tests were created and executed, covering core functionalities of the Spotify API such as song search, playlist creation, adding songs to playlists, and retrieving artist information.

- Requirement coverage: Around 85% of the defined requirements were covered. Most of the functionalities were tested, except for those requiring a premium account (e.g., offline playback and advanced audio quality).

- Untested functionalities: Tests related to premium account functionalities could not be executed, leaving a minor gap in testing.

- Bugs identified: No critical bugs were found that would prevent the product from being released to production. Most of the issues discovered are minor and can be addressed post-release without impacting the overall user experience.

- Product risks: The only risk identified relates to users with premium accounts, as premium features were not tested. This can be mitigated by future testing of this segment or by collaborating with premium users to verify their experience.

- Recommendations for release: It is recommended to proceed with the production release, provided a plan for additional testing of premium account features is implemented later. Additionally, a rapid feedback mechanism should be established to quickly address any post-launch issues.

- Lessons learned: For future projects involving premium features, early planning for access to premium accounts is advised to ensure complete testing. It would also be beneficial to automate as many core tests as possible to improve the repeatability of testing.

This conclusion reflects the results obtained and the risks identified during the testing process.










