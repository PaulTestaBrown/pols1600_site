Hi all,

Just following up with some bookkeeping for the course:

# --- Survey ---

Please take the time complete the class survey 

https://brown.co1.qualtrics.com/jfe/form/SV_ereKWyXCdAojdGu


# --- Assignment 1: Research Questions Due Sunday ---

The prompt for Assignment 1: Research Questions is now live:

https://pols1600.paultesta.org/files/assignments/A1_research_questions.docx

Your research questions are now due by 5pm on Sunday, March 6, 2022 on Canvas:

https://canvas.brown.edu/courses/1087979/assignments/7870538?module_item_id=10762418



# --- Upload Tutorials on Friday ---

Please upload QSS Tutorial 5: Prediction I by 11:59 pm tomorrow. 

You can find the tutorials in upper right panel of R Studio, or open this tutorial by running

learnr::run_tutorial("05-prediction1", package = "qsslearnr")


The tutorial introduces you to concepts of *for loops* 

for(i in 1:n){ do something for each value of i}

and *flow control* which uses R's Vulcan like capacity for logic to say 

for(i in 1:n){ 
    if (i == X){do something only when i == x}else{
        do something when i doesn't equal x
    }

These are important programming skills, that can be useful for stastitical inference and quantitative research. But they take some time to get your head around, so don't worry if you have to click the solutions on this part.


# --- Readings ---


Please read the rest of: Chapter 4 of QSS pp. 165-188 for next week.

Ideally you'll have read this before lecture on Tuesday, and definitely by our lab on Thursday.

In lecture next week, we'll explore we'll explore some alternative explanations or critiques of the "Red Covid" claim using multiple regression.

https://www.nytimes.com/2022/02/18/briefing/red-covid-partisan-deaths-vaccines.html

# --- Packages ---

For our lab on next Thursday, you'll need to have downloaded the packages described here:

https://pols1600.paultesta.org/slides/04-packages.html

And in particular have installed a Cenus API key following the steps described here:

https://pols1600.paultesta.org/slides/04-packages.html#3_Install_a_Census_API_tidycensus_package

The `easystats` package, ironically or maybe just annoyingly, hasn't been so easy to install for some of you.

Try this:

install.packages("easystats", repos = "https://easystats.r-universe.dev")

If that fails or gives you an error, try:

devtools::install_github("easystats/easystats")

If that fails, try

not_so_easystats <- c("insight",     
"datawizard",  
"bayestestR",  
"performance", 
"parameters",  
"effectsize",  
"modelbased",  
"correlation", 
"see",         
"report")      

for(i in not_so_easystats){
    install.packages(i)
}

And if that fails... try installing each package, one by one:

install.packages("datawizard")

Until/if you get an error and a package won't install. 

Easystats is a really useful collection of packages (once it's installed) that I use often in my research (which is why I wanted you to have it installed), but as I've learned, it appears to be a huge pain to make work across multiple platforms. Sorry!


Again please reach out to me if you encounter any issues installing these packages. Have a nice weekend!



Best,
Paul

