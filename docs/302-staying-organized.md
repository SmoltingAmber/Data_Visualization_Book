# Staying organized {#organization}

When you first start learning a computing tool like R, most people just put their files in "Downloads" or "Documents" or even on the "Desktop" with no particular thought to names or organization. This is fine when you are first experimenting, but it quickly gets out of control, especially when you want to keep one project separate from another, add data files, or want to share files with a collaborator.

Here are some suggestions to help you get and stay organized.

## Put everything in a folder

Many people just dump files at random on their Desktop, Documents, or Downloads directory. That's a recipe for chaos, as you eventually use the same file name as you did a few weeks ago (like example.Rmd) and you overwrite something or just mix up different projects.

Whenever you start a new project, such as a course, create a folder with an easy to understand name like "STAT2430" or "Data-Visualization". Spaces in file names in general are fine, but if you plan to share files with others its usually best to use a dash (`-`) or underscore (`_`) instead of spaces, since spaces in file names cause problems with some computing tools. (I put project folders in 'Dropbox' or 'One Drive' so I don't have to worry about backups.)


## Sub-projects

For each component of a project, create a new folder (directory) called something meaningful like "assignment-1".  
When I open R, instead of creating a new R markdown file right away, I first start a new project (File > New Project...). This new project can be in this new folder or you can create a new folder. 

You can choose to start using version control with the project. I suggest you do! Version control on your local machine takes very little extra effort and can be really handy if (when!) you delete something you didn't mean to, or decide to undo a whole bunch of changes that didn't work out the way you hoped. This works on your own computer -- no need to use github.

A project encourages you keep all your files together in the same place. Rstudio will remember which files were open when you quit and re-open them for you. It makes the process of switching from one project to another much easier. You can have two different Rstudio sessions open in different windows at the same time. Each R session has its own window and workspace and operates completely independently of any other R session you have open. I suggest you don't mix files from multiple projects in an R session; that works against your effort to stay organized.


## Files and Folders

You can put all your files in this project in this one folder, but if you have different kinds of files -- R markdown documents, data files, figures, and presentations, it can help you stay organized to create a sub-folder for each type of file. I find it particularly useful to do this for two kinds of files. Any file I get from somewhere else, typically a data file from a collaborator or the internet, goes in its own folder ("sources") and I never modify these files. That way I can clean up copies of a file and always know what the original file looked like. This is not really necessary if you use version control, but the original data file is the most likely file I'll want to use again and I think the duplication is worth the effort. Second, any files that are created by my R code: figures, data tables, or the results of time-consuming calculations, for example, because I know they can always be deleted and recreated later on. Putting them in their own folder reminds me I don't need to use version control on them; my code created them and there is no need to keep the results.

## Naming conventions

It's helpful to create informative names for files. If two files are related, use similar names with a different suffix (world-map.R and world-map.png, for example). If some steps need to be performed in a particular order, a simple way is to use a number (01, 02, etc) as a prefix. I used this convention when writing these notes to help me keep the sections in order. For advanced projects, there are specialty tools (e.g., drake) for performing calculations in a particular order, but a simple numbering scheme works for many projects that ourgrow simple sequencing of calculations in a single file.


## Resources

* Healy. Appendix. [Managing projects and files](https://socviz.co/appendix.html#managing-projects-and-files)
* Avoid using directory paths that won't exist on someone else's computer when you share files by using the [Here pacakge](https://here.r-lib.org/) ([github](https://github.com/jennybc/here_here)).
* R for Data Science notes on [scripts](https://r4ds.had.co.nz/workflow-scripts.html) and  [projects](https://r4ds.had.co.nz/workflow-projects.html)
* Drake [package](https://github.com/ropensci/drake) and [manual](https://books.ropensci.org/drake/)
* If you are worried about versions of packages changing, you can keep track of the packages you used and their versions using [checkpoint](https://github.com/RevolutionAnalytics/checkpoint) or [packrat](http://rstudio.github.io/packrat/)

