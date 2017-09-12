# Sample_Python
http://python-guide-ru.readthedocs.io/en/latest/writing/structure.html


## How to use Github

It makes sense to set some standards of how we will use github so we can see who's modifiying code and to make sure we alway have a branch that has a stable build. To accomplish this task, this is how we have it set up:

* Master Branch: This should always have a stable build. We should always be able to push to production from master without causing any issues.
* Develop Branch: This is where we should test our code. This allows us to test interactions of multiple fixes. So if person A wrote code that works fine on their branch and person B wrote code that works fine on their branch, we can test the interaction between A's and B's code in the develop branch. When the develop branch builds properly, it can be merged to the Master Branch to update features.
* User Branches: These are our individual branches. Whenever we are writing code, this is where we should be pushing changes. Once we have completed a fix and it works in our individual branch, we can merge with the Develop Branch to make sure that it works with everyone else's code (in case other parts have been modified). If issues occur in develop, individuals can still fix code without worrying about breaking production. Once you push a feature to develop, test it on develop, and push to Master, merge the Master Branch with your personal branch so you have the current working version of code.
