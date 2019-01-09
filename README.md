# Integrating Jeopardy

![The Jeopardy board](https://upload.wikimedia.org/wikipedia/commons/d/d8/Jeopardy_game_board.png)

### :warning: Read the submission guidelines at the bottom of this page first.

1. Refactor your Jeopardy app to use your Grid and Cell classes, and to be organized in terms of categories and difficulty values (dollar values), just like in the real game. *(5 points)*
2. When making your GET Request, validate that neither the question nor the answer are empty, If they are invalid, skip and find another *(2 points)*. You should not see any HTML in your response, if you find that the response does contain HTML, you can use this RegEx function to test for HTML tags and HTML entities: `const containsHTML = text => /(<.+?>)|(&.{1,6}?;)/.test(text);`.
3. Notice that jService allows users to increment an "invalid_count" property on their questions. (They do this by allowing a user to send a DELETE request, however this a "soft" DELETE and does not remove the questions from the API Database, we will not be using this feature for this assessment. More about soft DELETE [here](https://guides.cfwheels.org/docs/soft-delete).) Anything with an `invalid_count` should be skipped, too. *(2 points)*.
4. Escaped characters (e.g. `\"`) are easy to deal with, so just remove the slash from these strings. *(1 points)*

# Submission Guidelines
1. Fork [this](https://gitlab.com/kenzie-academy/se/fe/intro-to-backend-from-the-perspective-of-the-frontend/s_integrating-jeopardy-and-instantanswers.git) repo and clone it to your machine.
2. Enable GitLab Pages for your repo.
3. Add your code, per the instructions above.
4. Push your completed code to your own repo.
5. Submit a pull request to the *original* repo.
6. On the PR, add a comment with a link to your GitLab Page for your project.
7. On Canvas, submit a link to your PR.

