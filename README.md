Team: Hemendra Ande

1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

    Within a Github action that runs whenever code is pushed.

    This helps catch problems early before broken code makes it into the main branch. It also makes sure everyone’s code is being tested in the same environment, so you avoid the whole “works on my machine” issue. Running tests continuously is way better than waiting until the end, because it makes it easier to figure out exactly what change caused a problem. Overall, it keeps the project more stable and saves a lot of time debugging later.

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)

    No, I wouldn’t use an end-to-end test for that. End-to-end tests are for testing the whole app and user flow in the browser. If I just need to check whether a function returns the right output, I’d use a unit test instead. Unit tests are faster, simpler, and made specifically for testing isolated functions. Using an E2E test for that would just add unnecessary overhead.

3) What is the difference between navigation and snapshot mode?

    Navigation mode reloads the page and checks things like performance and loading speed. Snapshot mode looks at the page as it currently is without reloading it. It is mostly used for checking accessibility and SEO issues.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

   One thing we could improve is adding a language attribute to the html tag so screen readers know the page language. (Add lang="en" to the <html> tag.) 
   
   We could add a meta description (<meta name="description" content="..."> tag into the <head>) so search engines can display a better summary of the site. 
   
   We could also optimize the CSS by inlining our critical styles directly into the document head or deferring non-essential CSS so the browser paints the UI even faster. The page will load even faster and blocks less during rendering.