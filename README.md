IProMS
======

IProMS, which stands for "Intuitive Project Management System", is intended to be a complete, intuitive project management and ticket tracking system for small teams. Project management software is big business with heavy hitting entries such as Redmine and Version One. Ticket systems (helpdesk systems) are a more varied bunch, until one starts looking at things such as workflows and SLAs.

In searching for a project management system that would fit my needs, I found four primary problems that all but eliminated each and every one of them:

Cost Prohibitive
-----
While software such as Version One may be powerful, full-featured solutions, they're also expensive. Small groups or small teams may not have the means or the willingness to fork over that kind of cash. There are more affordable solutions, but they come with issues of their own.

No On-Premises Hosting
-----
Basecamp is one of the most highly recommended project management solutions on the market. Its pricing is extremely reasonable as well. However, as a hosted service, it's out on the internet for the world to see. While Basecamp may take every precaution to ensure that our data is secure, the only guarantee is that the information isn't out there in the first place. The best place for it is locked tightly away in the bowels of our corporate or personal intranets.

Dated, Clunky Interfaces
-----
Mantis is awesome. Its interface sucks. The same can be said of ]project open[. Because these systems are so packed with functionality, it's difficult to find a place to put it all. At least, that's my theory. While function is certainly more important than form when it comes to this type of software, I see no reason that we can't meet somewhere in the middle.

Specialized Software Requirements
-----
Open Project is my favorite project management system to date. However, it's primary "drawback" is that it's written in Ruby On Rails. This means that if your server doesn't have it installed, you can't use it. While Ruby may be a common web technology, it's not omnipresent as of yet. The server fascists at my company refuse to install it for me, claiming absence of support. The average web hosting company doesn't have it. What you will find almost everywhere is some kind of LAMP stack.

Enter IProMS
=====
I would consider myself a beginner-to-intermediate level PHP developer. At my place of employment, we do not have PHP developers. I'm what they call a "rogue". The development groups, at least the one I work with most frequently, uses Version One. Ask them to add a project to it for you... go on, I dare you. Internal support uses Service Desk. They'll let me onboard, but:

- My department has to foot the bill for the seat license and
- Everyone who has to submit tickets through Service Desk hates it

Ruby...? Fuhgeddaboutit.

What I did manage to get, after several years of politio-corporate hopscotch, was a Unix server running PHP 5.3 and MySQL. 

I still have to justify my remaining employed and I still have to provide reporting on what I do on a daily basis. I'm currently using Eventum from Oracle as a ticket system, but it's just as clunky as Mantis. It does have highly flexible workflow capabilities, but you have to write them yourself. Also the reporting is terrible.

There are packages out there such as ProjectPier that are free and would install in my environment, but frankly I just don't like them. So in the absence of all other options, what's a guy to do? Reinvent the wheel, of course.

The Must-Haves
=====
After some serious soul-searching, I decided that if I was going to start "from scratch" and write my own ticketing and project management system, it would have to run on the most commonly found systems in the wild: a LAMP stack. It must meet the following high-level requirements:

- It must be completely free of charge. 
- It must run on any basic, reasonably up-to-date web server.
- It must not require any other software, such as Ruby or Composer.
- It must loosely follow an MVC model.
- It must be a downloadable, stand-alone package.

To this end, I have decided to proceed with Codeigniter 3. Love it or hate it, CI is a solid, functional, easily-implemented framework. I've also decided to go with the Stencil template system for Codeigniter and the Charisma bootstrap template.

License
=====
I think people should be able to do whatever the hell they want with this thing. Fork it, steal it, sell it... I don't care. Someone out there has to be able to do more with this than I can, I'm just trying to spark the flame. To that end, I'm not setting a license at this point because I don't know what the final product will look like.
