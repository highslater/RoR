Chapter 1  
From zero to deploy  
  
In this first chapter, we’ll get started with Ruby on Rails by installing all  
the necessary software and by setting up our development environment.  

We’ll then create our first Rails application, called hello_app. Immediately  
after we’ll put it under version control with Git. And, put our first app on  
the wider web by deploying it to production.  

1.1 Introduction  

1.1.1 Prerequisites  

1.1.2 Conventions used in this book  

HELP  

https://www.railstutorial.org/#help  


Web development is a tricky business, and despite the best efforts of the tutorial it’s likely that you’ll run into trouble at some point. If you do, I suggest comparing your code to the reference implementation of the sample app to track down any discrepancies. You can also post your question at Stack Overflow using the tag railstutorial.org. (Click here to see questions labeled with that tag.) The creators of the Learn_Rails subreddit have graciously offered to answer questions as well.
Errors in the tutorial can be reported by email, but please triple-check by comparing with the reference implementation of the sample app first.
DEBUGGING TIPS
While it’s impossible to anticipate every potential problem, here are some debugging tips that might help:
Have you compared your code to the reference implementation of the sample app?
Are you using the exact gem versions (including Rails) used in the tutorial?
Did you restart the web server?
Did you try stopping Spring using bin/spring stop?
Did you kill all relevant Spring processes (as described in the book)?
Did you copy-and-paste from the book’s code? (Experience shows that typing in code, while a better learning technique in general, is error-prone, so when in doubt be sure to copy all code exactly.)
Did you re-run bundle install?
Did you try running bundle update?
Did you try Googling the error message?
If your problem is of a general nature, such as having issues installing Rails or configuring your system, I suggest posting to Stack Overflow (again using the tag railstutorial.org), sending a message to the Ruby on Rails Talk mailing list, or posting to the Learn_Rails subreddit. This will allow other people running into your issue (and not just those following the Rails Tutorial) to benefit from the discussion. You can also try asking your question on the Rails IRC channel (#rubyonrails) to get live assistance from other Rails programmers. For issues deploying to Heroku, please contact Heroku technical support.
When asking your question on any mailing list or forum, be sure to include as much relevant information as possible. To maximize your chances of a helpful reply, I especially recommend the article How To Ask Questions The Smart Way by Eric Raymond.  

1.2 Up and running  

1.2.1 Development environment  

Here are the steps for getting started with the cloud development environment:

Sign up for a free account at Cloud9.9 In order to prevent abuse, Cloud9 requires a valid credit card for signup, but the Rails Tutorial workspace is 100% free, and your card will not be charged.
Click on “Go to your Dashboard”.
Select “Create New Workspace”.
As shown in Figure 1.3, create a workspace called “rails-tutorial” (not “rails_tutorial”), set it to “Private to the people I invite”, and select the icon for the Rails Tutorial (not the icon for Ruby on Rails).
Click “Create workspace”.
After Cloud9 has finished provisioning the workspace, it should start automatically.

1.2.2 Installing Rails

The development environment from Section 1.2.1 includes all the software we need to get started except for Rails itself. To install Rails, we’ll use the gem command provided by the RubyGems package manager, which involves typing the command shown in Listing 1.1 into your command-line terminal. (If developing on your local system, this means using a regular terminal window; if using the cloud IDE, this means using the command-line area shown in Figure 1.2.)

Listing 1.1: Installing Rails with a specific version number.
$ gem install rails -v 5.1.2
Here the -v flag ensures that the specified version of Rails gets installed, which is important for getting results consistent with this tutorial.  

