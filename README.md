Team: Hemendra Ande

# **THE SCREENSHOT OF ALL TESTS PASSED IS IN results/all-tests-passed.png**

1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

    Within a Github action that runs whenever code is pushed.

    I can catch problems early before broken code makes it into the main branch. I wank to make sure everyone’s code is being tested in the same environment, so I can avoid the whole “works on my machine, but don't know if it works everywhere” issue. Running tests continuously is much better than waiting until the end, because it makes it easier to figure out exactly what change caused a problem. 

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)

    No, I wouldn’t use an end-to-end test here. End-to-end tests are much better suited for testing the whole app and user flow in the browser. I’d just use a unit test instead. Unit tests are much faster, simpler, and made specifically for testing isolated functions. E2E testing just adds so much overhead.

3) What is the difference between navigation and snapshot mode?

    Navigation mode reloads the page and checks things like performance and loading speed. Whereas Snapshot mode looks at the page as it currently is without reloading it. I feel like it's mostly used for checking accessibility and SEO issues.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

    I would add a language attribute to the html tag so screen readers know the page language. (lang="en" in <html>) 

    I would add a meta description (<meta name="description" content="..."> in <head>) so search engines can display a better summary of the site. 

    I would also optimize the CSS by inlining critical styles directly into the document head or even by deferring non-essential CSS so that the browser paints the UI even faster. The page will load even faster and blocks less during rendering.