# CVWO-memo-submission
This github repo contains my journey in completing the CVWO Winter Assignment.
You can now access the website here: [https://memoapp-bryan98.netlify.app/](https://memoapp-bryan98.netlify.app/)


## Student Details:

*Name*: Bryan Tee Pak Hong

*Matriculation Number*: A0221495E

## Installation of Rails:
The guide from [https://github.com/CVWO/setup-guide](https://github.com/CVWO/setup-guide) is very comprehensive.

![Rails installed Successfully!](/images/rails_installed.png "Rails installed Successfully!")

## Write-up:
You can find the link to the write-up [here](/docs/writeup.pdf).

You can find the link to the final report [here](/docs/CVWO&#32;Final&#32;Report.pdf).

I documented some key milestones here. Mostly in the UI portion interacting with backend. [https://www.instagram.com/modelconverge/](https://www.instagram.com/modelconverge/).

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

11/1/2021: discussed higher level idea with fellow CVWO assignment-doing mates, when alone tried to figure out potential issues with Internal Server Error (500) and Bad Request (400). The issue was redirection from ruby interface, a workaround was to do a new query and return the result as a JSON (original was to do a API call to memoboard index and return JSON, so was functionally identical).

12/1/2021: Read up on [comparison between props and states](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md), and learnt how to differentiate when to put an attribute in state vs props. Did a refactor for cleaner manipulation of react components. Allowed CORS delete and update from rails.

13/1/2021: Major refactor from [class components to functional components](https://nimblewebdeveloper.com/blog/convert-react-class-to-function-component). This allowed flexible use for Material-UI styling, as they believe React is going in the functional paradigm direction (Their [docs from basic to advanced styles](https://material-ui.com/styles/basics/) had literally zero info for class based components...). Added [Masonry](https://www.npmjs.com/package/react-masonry-component) to package.json, this allows cards to be ordered nicer than Grids in Materials-UI. Added Update of Memo to backend and frontend logic. Edit is done on the spot, abusing render (this however, takes away some potentially nice animations). 

14/1/2021: Have meetings on Friday and school assignments

15/1/2021 - 16/1/2021: Adding categories. At first considered having a concept of a service for memo to call and get their category colors. Asked opinions from an old friend that has experience with React, and they reminded me what I was doing was essentially implementing Redux from scratch. Decided against using Redux (or even concept for that matter) for now as I wanted to see how much I can push with only react and material-ui. Passing categories as props to each memoForm objects. Color change is visible, but will only be committed when the "Update" button is pushed.

17/1/2021: The nightmare that is adding categories and rerendering stuffs. I have done CRUD for categories (front end portion), and users can now assign categories to their memos. That being said, the code is too messy. I'll implement various filter functions first, before refactoring code to use Redux. 

18/1/2021: Added filtering by category. Did some thinking on whether I should do a SQL query or filter on the front end. Plan to migrate Categories and Memos to Redux. Deployment should begin soon!

19/1/2021: Learning basics of Redux. In the process of migrating. Had some homework so focused on those today.

20/1/2021: Still trying out redux. Read some tutorials. There is this website that teaches [how to add redux to project...](https://www.freecodecamp.org/news/how-to-use-redux-in-your-react-typescript-app/) maybe worth trying? Tried deploying on Heroku and Netlify. Initial deployment was quite smooth. 

You can now access the website here: [https://memoapp-bryan98.netlify.app/](https://memoapp-bryan98.netlify.app/)

Known issues: 
- when reloading, must go to root, or it will show error.

[this blog](https://www.netlify.com/blog/2019/01/16/redirect-rules-for-all-how-to-configure-redirects-for-your-static-site/) seems to show a possible fix. netlify can read the `_redirect` file or a `netlify.toml` file.

21/1/2021-22/1/2021: School is ramping up, completing tutorials/labs.

23/1/2021: reconsidered applying redux due to time constraints and (relatively) low complexity of the app. Added snackbar when adding/deleting/updating memos. Implemented R of memoboards.

24/1/2021 - 29/1/2021: School is ramping up!

30/1/2021: Added Pomodoro Timer.

Thanks for the fun assignment, really enriched my winter holidays!