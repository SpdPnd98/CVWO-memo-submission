# CVWO-memo-submission
This github repo contains my journey in completing the CVWO Winter Assignment.

## Student Details:

*Name*: Bryan Tee Pak Hong
*Matriculation Number*: A0221495E

## Installation of Rails:
The guide from [https://github.com/CVWO/setup-guide](https://github.com/CVWO/setup-guide) is very comprehensive.

![Rails installed Successfully!](/images/rails_installed.png "Rails installed Successfully!")

## Write-up:
You can find the link to the write-up [here](/docs/writeup.pdf).

## Updates:

31/12/2020 - 4/1/2021: Following [React with Rails tutorial by digitalocean.com](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-ruby-on-rails-project-with-a-react-frontend).

Learning Outcome:
1. Basic React to Rails interaction
2. sending of JSON from Rails -> Ruby -> React (controller -> html.erb file -> React)
3. Fetching JSON response in React from Rails.
4. CRUD interactions in React and Rails.

Link to the attempt (its a carbon copy of the tutorial) can be found here: [https://github.com/SpdPnd98/react_rails_recipe_tutorial](https://github.com/SpdPnd98/react_rails_recipe_tutorial)

5/1/2021: Followed [Tic-Tac-Toe tutorial](https://reactjs.org/tutorial/tutorial.html#setup-for-the-tutorial) from official React Website. Read on [state and lifecycles](https://reactjs.org/docs/state-and-lifecycle.html) in react. 


Results can be found here: [https://github.com/SpdPnd98/tic-tac-toe-react](https://github.com/SpdPnd98/tic-tac-toe-react)

6/1/2021: Recreated Rails and React separately, starting Rails as an API-Only app, and React purely as front-end. Proceed with development of Rails before React.

7/1/2021 - 8/1/2021: creating frontend with typescript. Found some useful resources
- [Response types for fetching from api](https://medium.com/@isachenx/making-a-fetch-request-with-typescript-4a6b523f1e69)
- [Typescript Cheetsheet](https://github.com/typescript-cheatsheets/react#reacttypescript-cheatsheets)

9/1/2021 - 10/1/2021: moving between hostel, took 2 days off. Long story short I had too much things.

11/1/2021: discussed higher level idea with fellow CVWO assignment, when alone tried to figure out potential issues with Internal Server Error (500) and Bad Request (400). The issue was redirection from ruby interface, a workaround was to do a new query and return the result as a JSON (original was to do a API call to memoboard index and return JSON, so was functionally identical).

12/1/2021: Read up on [comparison between props and states](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md), and learnt how to differentiate when to put an attribute in state vs props. Did a refactor for cleaner manipulation of react components. Allowed CORS delete and update from rails.
