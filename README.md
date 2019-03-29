# Sprint Challenge: Advanced CSS - Space Walkers Web Page

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?

  A: A responsive website has a layout that will adapt to any screen size fluidly, 	using media query breakpoints.

	An adaptive website will have static media query breakpoints for specific 		device screen sizes, and the content will snap into place when a breakpoint is 	changed. Essentially a developer would create 2 or 3 different layouts.

2. Describe what it means to be mobile first vs desktop first.

  A: To be mobile first your design layout will consist of strategizing content to 	be delivered to the user primarily on the mobile device. When writing in your 	CSS files the strategy would be to code the styling starting on the mobile 		screen size first, and then scaling up.

	To be Desktop first your design layout is going to be optimized for desktop 	layout delivery. From there you would scale your site down to a mobile 		experience.

	In both cases it would be smart to build the site as a responsive design.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?

  A: The default font-size of a browser is 16px. If we set the html tag font size 	to 62.5%, this will set the default size of the site to 10px. Which will in turn 	make the calculations of em/rem a lot easier to make.

  (62.5/100)x16 = 10px

4. How would you describe preprocessing to someone new to CSS?

  A: It is a program that lets you generate css from its own syntax. The features 	preprocessing gives you make reading and writing css easier.

  To use a preprocessor you need to install a compiler on onto your machine to 	convert the syntax to vanilla css.

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

  A: My favorite concept in preprocessing is nesting. It is just so convenient!  	The concept that gives me the most trouble is maps. I haven’t fully dove into 	the topic yet. 

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Because you are using a preprocessor, there are two parts to setting up your project.  Be sure to run through the git set up first and then set up the preprocessor.

### Git Set up

Follow these steps to set up your project:

- [x ] Create a forked copy of this project.
- [ x] Add your project manager as collaborator on Github.
- [x ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ x] Create a new branch: git checkout -b `<firstName-lastName>`.
- [x ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ x] Push commits: git push origin `<firstName-lastName>`.

Follow these steps for completing your project.

- [x ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [x ] Add your project manager as a reviewer on the pull-request
- [x ] Your project manager will count the project as complete by merging the branch back into master.


### Preprocessor Set up

* [x ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [x ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [x ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [x ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [x ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [x ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [x ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [x ] Add a viewport meta tag to the head of your index.html page

* [x ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [x ] Navigation Styles: Use the `navigation.less` file for styling.

* [x ] Main Content Styles: Use the `home-page.less` file for styling

* [x ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [x ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [x ]  Use at least 2 parameters to create your button

* [x ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [x ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [x ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [x ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription
