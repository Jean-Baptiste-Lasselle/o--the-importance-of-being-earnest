# On the importance of being earnest

_A repo to share thoughts wih the world._


# How it started

**The 29th of MArch, 2020 5:00 am**.

I am waking up, I have beaksfast, I feel like working :

Currently working on subjects and ideas are exploding all over the place in my head, and

I feel rested and all energy full on the morning, it feels good.

So end of beakfast, I sit at desk startup debian, go to yotube to play anything a background while working.

I see a video suggestion about `terraform` :


I listen to it 2 minutes, and suddenly I can't help wirting a comment that 20 miutes later becomes the
deepest thing I have put in words abotu Infrastructure as code, until today :



## The infrastructure as code pattern


https://www.youtube.com/watch?v=R2UDlNGJHI8

It's really unfair, because video is from 2016, and its now 2020, but I can't help mentioning :
I do agree about why you should be against command line update the terraform state.

but no, you should not yell at them, what should happen, is that you, should provide means to make that (command line update the terraform state) useless, and pointless, modify your high level factory, so that those you don't want to be allowed to command line modify the terraform state, can't :
* `.gitignore` terraform state
* reject any commit / pull /merge request modifying the `.gitignore`. especially important : the commits on a feature branch. And cross repository pull request not from feature, to develop, but from feature (branch) to feature.
* allow only robots to manage terraform state for you : you never commad-line, instead, to do what you want to do, you modify the source code of the robot, and let the robot do the job.

This pattern is extremely important, because now :
* to do any operations, people change source code of the robot, and never EVER touch the infrastructure.
* And now, you, can set any extremely rich and powerful control over those who operate the infrastructure : just as much control as we can hacve today, over developers (that is, a crazy lot). That is, the dev flow on the robot, so have an extremely rich, so much better control, over people changing infrastructure, than just a stupid user permission model, whether it's an OpenID connect / Gravitee.io duet, or a stupid LDAP.
* Actually the imporantce, of being earnest, is that the importance of that extremely powerful control, is that it is control over your own work, not on other people work.
* Finally, you might smile on the corner, if say that anyway today (smart) managers understand don't understand, and probably won't ever in their life, what we are doing : And actually it's aweseome, cause now we have a real context, where there is a real challenge, to bring trust, between us, and the manegrs. At some level, it also is the exact context among us : You do know, I know thing you don't understand (yet), and I do know, that you know things I don'tknow (yet). If we trust each other in work this will make the two of us dream team.

Something said with other words : the robot is a software, and there fore it has a software factory, made of pipelines, workflows, etc... So much more than just a stupid  OpenID connect / Gravitee.io duet,or LDAP.



This pattern is infrastructure as code, so yes, command line changing state is against infratstructure adressed as code, but now that it is explained, there you have the why.
