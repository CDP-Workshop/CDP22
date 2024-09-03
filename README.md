
Contains the website and the files to support the organization of the Compiler-Driven Performance Workshop

# setting up website locally

Clone the git repository (change GIT_REPO_NAME): `git clone GIT_REPO_NAME`

Make sure to have the ruby header files installed on your system, then:

`gem install bundler`

`bundle install`

To build the website: `bundle exec jekyll build`

Then test it locally using a local webserver (this will make sure the website gets rebuilt automatically when any file changes):

`bundle exec jekyll serve --incremental`

To continuously update the local copy of the website while changing it use the command:

`bundle exec jekyll serve --watch`

To see the local version go to the following URL:

http://localhost:4000/

Once done with changes:

`git commit -a`

`git push`

Check to see everything works: [https://cc-conference.github.io/18/]

# Changes that are needed each year for a new edition of the workshop

- To add/remove drop-down menus from the main site, edit the file docs/_layouts/default.html

* There is a long entry bracketed by \<li> and \</li> for each drop-down menu.
* The entries in the menu link to files in the docs folder. For example de "Call for Contributions" menu links to the file docs/call.html.

- Make sure to add the program for the previous year to the folder docs/previous and to create a new entry at the top of the "Previous CDPs" drop-down menu by editing the docs/_layouts/default.html file.

- Review the entire site to look for places where dates, workshop edition, location, schedule, may need editing.

