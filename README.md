# Ten Simple Rules for Helping Newcomers Become Contributors to Open Source Projects

Dan Sholler<sup>1</sup>,
Igor Steinmacher<sup>2</sup>,
Denae Ford<sup>3</sup>,
Mara Averick<sup>4</sup>,
Mike Hoye<sup>5</sup>,
Greg Wilson<sup>4</sup>  

1.  Berkeley Institute for Data Science / sholler.daniel@gmail.com  
2.  Northern Arizona University/ igor.steinmacher@nau.edu  
3.  North Carolina State University / dford3@ncsu.edu  
4.  RStudio, Inc. / {mara.averick, greg.wilson}@rstudio.com  
5.  Mozilla Corporation / mhoye@mozilla.com  

These authors contributed equally to this work.

## Abstract

In order to survive and thrive, a community needs to attract and retain
new members and help them be productive. The 10 simple rules outlined in
this paper describe ways to do this that are suitable for small and
medium-sized projects, based on current research, and have demonstrated
their effectiveness in several open source and open science software
projects.

## Author Summary

Research has always been a communal activity, but researchers have only
recently begun to pay attention to what we know about why some
communities thrive and others fail. Attracting contributors, retaining
them, and helping them be more productive have all been the subject of
intensive study. This paper presents 10 findings from those studies that
community leaders can apply immediately and explains why they work.

## Introduction

In order to survive and thrive, a community needs to attract new
members, retain them, and help them be productive contributors [qureshi2011]. As
openness becomes the norm in scientific research and software
development, knowing how to do this has become a necessary skill for
principal investigators and other project leaders. While every situation
is unique, a growing body of knowledge in sociology, anthropology,
education, and software engineering can guide decisions about what to do
to facilitate this.

But what exactly do we mean by "community"? In the case of open source
and open science, the most usual meaning is a "community of practice".
As defined by Lave and Wenger [lave1991,wenger1999], groups as diverse as knitting circles,
oncology researchers, and the organizers of amateur theatrical groups
share three key characteristics:

1.  Participants have a common purpose or product that they work on or
    toward.

2.  They are mutually engaged, *i.e.*, they assist and mentor each
    another.

3.  They develop shared resources and domain knowledge.

Brown [brown2019] specializes this to define a "community of effort" as,
"...a community formed in pursuit of a common goal. The
goal can be definite or indefinite in time, and may not be clearly
defined, but it is something that (generally speaking) the community is
aligned on." People working to preserve coral reefs in the face of
global climate change are an example of a more loosely connected
community of effort. There is no single central organization
coordinating their work, but the scientists who study coral reefs, the
environmentalists who work to protect them, and the citizens who support
them financially and politically are aware of each other's efforts,
coordinate with each other in various ad hoc ways, and are conscious of
contributing toward a shared purpose.

Several open source software projects are also communities of effort.
For example, Mozilla Firefox [mozilla] is composed of: a mix of paid
professionals, highly-involved volunteers, and occasional contributors
who create software, documentation, and tutorials while also organize
events, answer questions in online forums, mentor newcomers, and
advocate for open standards.

Every community of effort has its own unique features, but they have
enough in common to profit from one another's experience. The 10 rules
laid out below are based on studies of such communities and on the
authors' experience as members, leaders, and observers of them. Our
focus is on small and medium-sized projects, i.e., ones that have a
handful to a few dozen participants and are a few months to a few years
old, but do not (yet) have any formal legal standing such as
incorporation as a non-profit.

## Rule 1: Have and enforce a code of conduct.

The first and most important rule is to create explicit guidelines for
members of the community to follow. This helps ensure that everyone---not
just newcomers---will find the environment healthy and welcoming. Doing
this also sends a clear signal that the community actually has
standards: many potential contributors will be painfully familiar with
communities that don't, and are more likely to give yours a try if they
believe it is more than a troll-infested chat room. Explicit guidelines
also make the project more socially accessible to people from differing
cultural backgrounds, as it helps them understanding what expectations
are and how they may differ from what they are used to.

An increasingly popular strategy for establishing guidelines is to adopt
a Code of Conduct. Empirical research on codes of conduct is still in
its infancy [tourani2017], but many projects such as rOpenSci [ropensci-coc],
NumPy [numpy-coc], and Project
Jupyter [jupyter-coc] have adopted the Contributor Covenant [covenant] or used other frameworks
such as SciPy's Code of Conduct [scipy-coc]. However, several questions around
reporting violations and enforcing rules remain open. What is the
appropriate mechanism for reporting violations? Who should receive
reports? What types of actions can projects take when a member of the
community violates the code? Projects may vary in how they address these
questions based on characteristics of size, technology choices, or human
resources (such as the presence of a community manager). However, some
must-haves are clear based on our collective experience and code of
conduct guides [aurora2019].

For instance, projects should designate at least one independent party
(i.e., an individual not employed by or otherwise deeply tied the
project) to receive and review reports. An independent party offers a
degree of objectivity and can help to protect reporters from hesitating
to report out of fear of retribution or damage to their reputation. When
possible, the independent party should be part of a more extensive code
of conduct committee made up of several people with varied
characteristics (e.g., gender identity, race, ethnicity, roles in the
community). Any member of the committee implicated in the incident
should be refused from reviewing the violations.

Project leaders should also develop some enforcement mechanisms and,
when safe for the reporter, publicize the enforcement decision.
Enforcing the code and announcing decisions are critical; otherwise, the
community will quickly recognize the code as meaningless. Committees can
consider several courses of action once investigations are complete:
verbal or written warnings, limits on access to project communication
avenues (e.g., Slack channels or mailing lists), or in severe cases,
suspension or expulsion from contributing to the project.

## Rule 2: Make governance and licensing explicit.

Raymond's "The Cathedral and the Bazaar" [raymond2001] described an egalitarian world
in which everyone could contribute equally to open projects. Two decades
later, we can see how unequal and unwelcoming the supposedly egalitarian
"bazaar" of open source can be if authority lies with those willing to
shout loudest and longest. As Bezroukov pointed out [bezroukov1999], Raymond ignored
the realities of how power arises, becomes concentrated in a few hands,
and is then used to perpetuate itself.

Bezroukov's criticism drew on Freeman's influential essay "The Tyranny
of Structurelessness" [freeman1972], which explained how an apparent lack of
structure in organizations "...too often disguised an
informal, unacknowledged and unaccountable leadership that was all the
more pernicious because its very existence was denied." The solution is
to make a project's governance explicit so that people know who makes
which decisions.

Large, well-established projects that incorporate as non-profits are
required to promulgate bylaws, such as those for the Python Software
Foundation [psf-bylaws]. What smaller projects should do is less well-documented,
but the "Social and Political Infrastructure" chapter of [fogel2005] describes two
models:

-   A "benevolent dictator" (who might better be called a
    "community-approved arbitrator") has final say, but their
    principal responsibility is to manage conversation to achieve
    consensus.

-   Elected representation and/or community votes on key issues. In the
    Carpentries, for example, anyone who satisfies any of the conditions
    below is considered a voting member of the organization [carpentries-bylaws]:
    
    1.  everyone who has completed instructor certification in the
        preceding year;
    
    2.  everyone who has completed certification in the last two years
        and taught at least one workshop;
    
    3.  everyone who has been certified for more than two years and has
        taught at least twice in that time; and
    
    4.  anyone who has made a significant contribution to lesson
        development, infrastructure, or other activities as determined
        by the Executive Council.

More complex models are possible [apache-governance], but the most important thing is to
decide on the rules well in advance of contentious issues emerging,
since tempers may already be running hot by the time this point is
reached.

As well as making governance explicit, it is essential that open source
projects are clear about licensing. Who can use the data collected by
the software for what purposes, and what attribution do they have to
give? How must they acknowledge the project and/or its contributors? Who
holds the copyright on contributed material? Most projects now place
this information in files called `LICENSE.md` and `CITATION.md` to make
them easy to find. Wherever they are put, the most important thing is to
make it clear before people begin contributing.

## Rule 3: Be welcoming.

As Fogel said [fogel2005], "If a project doesn't make a good first impression,
newcomers may wait a long time before giving it a second chance." Other
authors have empirically confirmed the importance of kind and polite
social environments in open source projects [singh2012,steinmacher2013,steinmacher2018a]. Therefore, projects should
not just say that they welcome new members: they should make a proactive
effort to foster positive feelings in them.

-   Post a welcome message on the project's social media pages, Slack
    channels, forums, or email lists. Projects might consider
    maintaining a dedicated "Welcome" channel or list, where a project
    lead or community manager writes a short post asking newcomers to
    introduce themselves.

-   Offer assistance in finding ways to make an initial contribution.

-   Direct the newcomer to project members who have a similar background
    or skill set so as to demonstrate fit to the newcomer.

-   Point the newcomer to essential project resources (e.g., the
    contribution guidelines).

-   Clearly identify work items they can start with. A growing number of
    projects explicitly tag bugs or issues as "suitable for newcomers",
    and ask established members not to fix them in order to ensure there
    are suitable places for new arrivals to start work.

Projects can further designate one or two members to serve as a
point-of-contact for each newcomer. Doing this may reduce the newcomer's
hesitancy to ask questions, particularly when they are told from the
outset that there are no dumb questions in the community.

## Rule 4: Help potential contributors evaluate if the project is a good fit.

People could contribute to many different projects; the first and most
important step in being welcoming is to help them determine whether your
project is a good fit for their interests and abilities. Their decision
to contribute can be related to reputation or external needs, but also
to a desire to learn or give back to the community. In all of these
cases, the more you help newcomers understand if this is the right
project for them, the more quickly they will either start contributing
or look elsewhere.

To do this, the project should explicitly state what the different types
of skills required are. This information should be easily accessible and
guide new members to the tasks they may handle. LibreOffice, for
example, provides a way for developers to filter available tasks by
required skills and difficulty [libreoffice-filtered].

The project should also help developers evaluate their skills, since
"basic Python skills" means very different things to different people.
Tools like My GitHub Resume [my-github-resume] and Visual Resume [sarma2016] that aggregate
information from previous contributions can help with this assessment,
while the OpenHatch project [openhatch] aggregated entry-level issues from a
variety of open source projects and classified them according to
language and other required skills to provide a one-stop portal for
finding appropriate projects.

## Rule 5: Develop forms of legitimate peripheral participation

A core concept in the theory of communities of practice is that of
legitimate peripheral participation (LPP) [lave1991,wenger1999]. Newcomers become members of
a community by participating in simple, low-risk tasks that further the
goals of the community. Through these peripheral activities, newcomers
become acquainted with the community's tasks, vocabulary, and governance
so that they can ease into the project.

In communities such as GitHub, core activities such as committing code
and submitting pull requests can be socially daunting for newcomers [steinmacher2015].
One way to encourage LPP in this case is to encourage newcomers to
submit issues to a repository when they notice a bug or to join the
dialog on recently submitted pull requests or issues. Another way is to
have newcomers help with documentation, particularly with translation
and localization, and a third (mentioned in Rule 3) is to mark some
issues as suitable for newcomers.

Building multiple ways of participating in a community demonstrates the
variety of approaches newcomers can take to join the community. This
further demonstrates that there is not just one way to make technical
contributions. For example, the main form of interaction in the
community on Stack Overflow is to ask a question and posting an answer,
but engaging in that type of interaction can present barriers some users
including an intimidating community size and fear of negative feedback [ford2016].
Thus, it is important to provide additional forms of participation. On
Stack Overflow, this is demonstrated through the ability to edit
questions and answer without the restriction of reputation points.
Developing a pathway to participation can decrease the presence of
barriers. In studying the evolution of how content is formed in these
communities [baltes2018], newcomers can better understand the norms of a community
and the best way to contribute [ford2018].

## Rule 6: Make knowledge findable and keep it up to date.

When starting to contribute to a project, newcomers need to learn their
way around it. However, newcomers to software projects are like
explorers who must orient themselves within an unfamiliar landscape [dagenais2010].
Thus, it is important to make sure that all necessary information is
accessible (or at least searchable) by newcomers during their first
steps.

Information that is spread out usually makes newcomers feel lost and
disoriented. Given the different possibilities of places to maintain
information (e.g., wikis, files in the repository, shared documents, old
tweets or Slack messages, and email archives), it is important to keep
information about a specific topic consolidated in a single place so
that newcomers do not need to navigate multiple data sources to find
what they need. The literature has shown that organizing the information
make newcomers more confident and oriented [steinmacher2016]. This organization is
something important for technical and process documentation but also for
communication channels. Another suggestion is, therefore, to stick to a
small number of communication channels and to clearly define the goals
for each of them.

At the same time, outdated documentation may lead newcomers to a wrong
understanding of the project, which is also demotivating. While it may
be hard to keep documentation up-to-date, community members should
remove outdated information or, at least, clearly identify it as
outdated. Making newcomers aware of the absence or the status of a
document can save their time and set their expectations. By recognizing
the obsolescence of the information, communities may request help from
the newcomers as a way to foster their contribution.

## Rule 7: Provide an easy, complete, and up-to-date guide to contributing.

A project can guide newcomers toward desired practices by providing them
with "how to contribute" guidelines in easy-to-find, readily-available
places. Many projects follow GitHub's recommendation for placing such
information in a `CONTRIBUTING.md` file [github-rec]. Other projects, such as the
Apache Open Office Suite and rOpenSci, provide newcomer manuals and
learning modules accessed through a web interface [apache-guidelines,ropensci-guidelines]. Still others take a
more interactive approach; for example, the GNOME project's Newcomers
Guide [gnome-newcomers], walks potential contributors through the contribution pipeline:
choosing a project, acquiring and installing the necessary computing
tools, finding problems or choosing issues to work on, submitting
changes, and following up on feedback.

No matter how they are presented, such guidelines do more than just
describe how to contribute and help newcomers feel they are on equal
footing with veteran project members. First, their mere existence can
ease newcomers' hesitation about whether or not their work is sufficient
and suitable for the project. Second, they provide a centralized,
well-organized description of resources that a newcomer can consult
while learning to navigate the project's technical and social
environments [zanatta2017]. Guidelines also acclimate newcomers to the norms of work
and communication, particularly when items such as necessary computing
tools and codes of conduct are foregrounded.

Finally, such guidelines should be clear about how contributions will be
acknowledged and how they can be used. A pointer to the license and
citation documents (Rule 2) is a start, but a clear and objective
summary in plain language will be more helpful for newcomers.

Project decision-makers should keep in mind that their perceptions of
what constitutes clear, easy-to-find contribution guidelines may not
align with the perceptions of the newcomers themselves. Continual
reevaluation of the guidelines based on community member feedback is
essential to ensuring that contribution guidelines are achieving desired
effects and do not fall out of date (e.g., as technical and social
elements of the community change). Contributing to the contribution
guidelines is therefore an excellent opportunity for legitimate
peripheral participation.

## Rule 8: Use opportunities for in-person interaction, but with care.

Open source software projects often rely heavily on remote workers
communicating via text, audio, and video. Research on face-to-face and
audio/video-mediated communication is mixed with regard to their
comparative effectiveness [doherty1997,gallupe1990,nardi2002], but demonstrates that each form has benefits
and drawbacks. In-person interaction is valuable for uninterrupted,
synchronous dialog and helps to establish mutual understanding in a
streamlined way [omalley1996]. Projects can therefore benefit from engaging newcomers
in in-person interaction from time to time.

According to Huppenkothen and colleagues [huppenkothen2018], newcomers may particularly
benefit from hackweeks that, "...combine structured periods
focused on pedagogy (often with an emphasis on statistical and
computational techniques) and less structured periods devoted to hacks
and creative projects, with the goal of encouraging collaboration and
learning among people at various stages of their career." Building
newcomer-friendly events and activities into a hackweek might serve as
an effective approach for acclimating newcomers to the project and its
community as well as highlight the potential avenues for newcomer
contributions.

However, projects should exercise caution when asking newcomers to
communicate in person. First, potential contributors might shy away from
the project if they are introverted, suffer from social anxiety, or have
had bad experiences in the past in face-to-face settings. Establishing
and publicizing a Code of Conduct helps allay these concerns, but some
newcomers may still feel uncomfortable in group settings. In this case,
not going to a meetup may leave them feeling less a part of the
community.

Face-to-face communication also involves forms of information exchange
that are not easily captured and archived for all project members to
see. For example, collocated project members might hash out ideas on
whiteboards, by scribbling notes, or through informal chats. Even when
transcribing and/or taking photos of these is possible, important
contextual information may be lost [cherubini2007]. Decisions and changes may seem to
come out of nowhere when evaluated by a non-attendee, so project leads
should develop universally-accessible ways to communicate and explain
the results of in-person activities.

## Rule 9: Make it easy for newcomers to set up.

The experience of getting set up to work on a project---the moment they go
from "I want to help" to "I'm able to help" to "I'm helping"---is often a
contributor's first impressions of the experience of participating in
that community. This makes the developer setup process a critical moment
in your relationship with every new contributor, which in turn means
that any complexity or confusion at this point is a significant barrier
to participation [steinmacher2014]. By treating the process of getting involved with the
same care and attention you give to the product itself, you're making it
clear that you value those contributors' time and effort, and
forestalling reactions like this [steinmacher2018b]:

> I am still trying to build, because many errors occurred...
> I was expecting to move forward, because so far I did not have time to
> look at the source code... It is frustrating.

This work does not just benefit newcomers: it also helps retention of
existing intermittent contributors and the same work that makes your
project more accessible to new contributors today will do the same for
future you. Wheelchair ramps and the buttons that open heavy doors are
not just used by those in wheelchairs: they are just as helpful to
people with strollers or one too many bags of groceries. None of us are
ever more than a sprained ankle away from desperately wanting that
wheelchair ramp to be there. In that same vein, a drive failure will
someday force you to download a gigabyte of data and reinstall some
software, inevitably at the least convenient moment imaginable. There is
therefore a lot to be gained from automating as much of your setup
process you can and thoroughly documenting whatever you cannot.

## Rule 10: Follow up on success.

People in open source sometimes joke that a programmer is someone who
will do something for a laptop sticker that they would not do for a
hundred dollars. This joke acknowledges that gratitude and recognition
are the most powerful tools available for community builders and
maintainers. Our last rule is therefore as important as our first:
acknowledge newcomers' contributions and thank them for their work.
Every hour that someone has given your project may be an hour taken away
from their personal life or their official employment; recognize that
fact and make it clear that while more hours would be welcome, you do
not expect them to make unsustainable sacrifices.

This is also a good time to figure out where and how the newcomer might
help in the longer term. Once they have carried their first contribution
over the line, you and they are likely to have a better sense of what
they have to offer and how the project can help them. Helping newcomers
finding the next problem they might want to work on or pointing them at
the next thing they might enjoy reading is both helpful and supportive.
In particular, encouraging them to help the next wave of newcomers is
both a good way to recognize what they have learned, and an effective
way to pass it on.

Mentoring programs are a popular way to do this. However, their
effectiveness appears mixed. [fagerholm2014] found that, "...developers
receiving deliberate onboarding support through mentoring were more
active at an earlier stage than developers entering projects through
conventional means." In contrast, [labuschagne2015] found that, "...developers
who join an organization through these programs are half as likely to
transition into long-term community members than developers who do not
use these programs... although developers who do succeed
through these programs find them valuable."

One explanation for this disparity is that people become members of open
projects for different reasons, and hence respond to things like
mentoring programs in different ways. For example, Barcomb et
al. identified four types of episodic or intermittent contributors to
open source projects [barcomb2019], while Mäenpää et al. looked at how to reconcile
the competing yet complementary needs of stakeholders in hybrid
open/commercial projects [maenpaa2018]. More research is needed, but as openness
becomes the norm in research, doing it well becomes a core skill for
every researcher.

## Bibliography

[apache-governance] Foundation AS. The Apache Software Foundation: How It Works; Accessed March 27, 2019. https://www-us.apache.org/foundation/how-it-works.html.

[apache-guidelines] Foundation AS. Introduction to Contributing to Apache OpenOffice; Accessed February 16, 2019. https://openoffice.apache.org/orientation/intro-contributing.html.

[aurora2019] Aurora V, Gardiner M. How to Respond to Code of Conduct Reports. Version 1.1 ed. Frame Shift Consulting LLC; 2019.

[baltes2018] Baltes S, Dumani L, Treude C, Diehl S. The Evolution of Stack Overflow Posts: Reconstruction and Analysis. CoRR. 2018;abs/1811.00804.

[barcomb2019] Barcomb A, Stol KJ, Riehle D, Fitzgerald B. Why Do Episodic Volunteers Stay in FLOSS Communities? In: Proc. 2019 International Conference on Software Engineering (ICSE'19). ACM Press; 2019. 

[bezroukov1999] Bezroukov N. A Second Look at the Cathedral and the Bazaar; 1999. https://firstmonday.org/article/view/708/618.

[brown2019] Brown CT. Sustaining open source: thinking about communities of effort; Accessed March 21, 2019. http://ivory.idyll.org/blog/author/c-titus-brown.html.

[carpentries-bylaws] The Carpentries Bylaws; Accessed February 16, 2019. https://docs.carpentries.org/topic\_folders/governance/index.html.

[cherubini2007] Cherubini M, Venolia G, DeLine R, Ko AJ. Let's Go to the Whiteboard: How and Why Software Developers Use Drawings. In: Proc. 2007 Conference on Human Factors in Computing Systems (CHI'07). Association for Computing Machinery (ACM); 2007.

[covenant] Contributor Covenant; Accessed February 14, 2019. https://www.contributor-covenant.org/.

[dagenais2010] Dagenais B, Ossher H, Bellamy RKE, Robillard MP, de Vries JP. Moving Into a New Software Project Landscape. In: Proc. 2010 International Conference on Software Engineering (ICSE'10). ACM Press; 2010.

[doherty1997] Doherty-Sneddon G, OMalley C, Garrod S, Anderson A, et al. Face-to-face and video-mediated communication: A comparison of dialogue structure and task performance. Journal of Experimental Psychology: Applied. 1997;3(2):105--125. doi:10.1037/1076-898x.3.2.105.

[fagerholm2014] Fagerholm F, Guinea AS, Münch J, Borenstein J. The role of mentoring and project characteristics for onboarding in open source software projects. In: Proc. 2014 International Symposium on Empirical Software Engineering and Measurement (ESEM'14). ACM Press; 2014.

[fogel2005] Fogel K. Producing Open Source Software: How to Run a Successful Free Software Project. O'Reilly Media; 2005.

[ford2016] Ford D, Smith J, Guo PJ, Parnin C. Paradise Unplugged: Identifying Barriers for Female Participation on Stack Overflow. In: Proc. 2016 ACM SIGSOFT International Symposium on Foundations of Software Engineering (FSE'16). FSE 2016. ACM Press; 2016. p. 846--857.

[ford2018] Ford D, Lustig K, Banks J, Parnin C. "We Don't Do That Here": How Collaborative Editing with Mentors Improves Engagement in Social Q\&A Communities. In: Proc. 2018 CHI Conference on Human Factors in Computing Systems. CHI 2018; 2018. p. 608:1--608:12.

[freeman1972] Freeman J. The Tyranny of Structurelessness. The Second Wave. 1972;2(1).

[gallupe1990] Gallupe RB, McKeen JD. Enhancing Computer-Mediated Communication: An experimental investigation into the use of a Group Decision Support System for face-to-face versus remote meetings. Information & Management. 1990;18(1):1--13. doi:10.1016/0378-7206(90)90059-q.

[github-rec] GitHub. Setting Guidelines for Repository Contributors; Accessed February 16, 2019. https://help.github.com/articles/setting-guidelines-for-repository- contributors/.

[gnome-newcomers] GNOME Newcomers' Guide; Accessed February 16, 2019. https://wiki.gnome.org/Newcomers/SubmitContribution.

[huppenkothen2018] Huppenkothen D, Arendt A, Hogg DW, Ram K, VanderPlas JT, Rokem A. Hack weeks as a model for data science education and collaboration. Proc National Academy of Sciences. 2018;115(36):8872--8877. doi:10.1073/pnas.1717196115.

[jupyter-coc] Jupyter P. Code of Conduct; Accessed February 14, 2019. https://github.com/jupyter/governance/blob/master/conduct/code\_of\_conduct.md.

[labuschagne2015] Labuschagne A, Holmes R. Do Onboarding Programs Work? In: Proc. 2015 Working Conference on Mining Software Repositories (MSR'15). IEEE; 2015.

[lave1991] Lave J, Wenger E. Situated Learning: Legitimate Peripheral Participation. Cambridge University Press; 1991.

[libreoffice-filtered] Foundation TD. LibreOffice Easy Hacks by Required Skill; Accessed March 21, 2019. https://wiki.documentfoundation.org/Development/EasyHacks/by\_Required\_Skill.

[mozilla] Foundation M. Mozilla Firefox; Accessed March 21, 2019. https://www.mozilla.org/en-US/.

[my-github-resume] Coallier D. My GitHub Resume; Accessed March 21, 2019. https://resume.github.io/.

[nardi2002] Nardi BA, Whittaker S. The place of face-to-face communication in distributed work. In: Hinds P, Kiesler S, editors. Distributed Work. MIT Press; 2002. p. 83--110.

[numpy-coc] Community S. NumPy Code of Conduct; Accessed February 14, 2019. https://www.numpy.org/devdocs/dev/conduct/code\_of\_conduct.html.

[omalley1996] O'Malley C, Langton S, Anderson A, Doherty-Sneddon G, Bruce V. Comparison of face-to-face and video-mediated interaction. Interacting with Computers. 1996;8(2):177--192. doi:10.1016/0953-5438(96)01027-2.

[openhatch] OpenHatch; Accesssd March 27 2019. http://openhatch.org/.

[psf-bylaws] Python Software Foundation Bylaws; Accessed February 16, 2019. https://www.python.org/psf/bylaws/.

[qureshi2011] Qureshi I, Fang Y. Socialization in open source software projects: A growth mixture modeling approach. Organizational Research Methods. 2011;14(1):208--238.

[raymond2001] Raymond ES. The Cathedral and the Bazaar; 2001.

[ropensci-coc] rOpenSci Code of Conduct; Accessed February 14, 2019. https://ropensci.org/code-of-conduct/.

[ropensci-guidelines] rOpenSci Packages: Develpoment, Maintenance, and Peer Review; Accessed February 16, 2019. https://ropensci.github.io/dev\_guide/.

[sarma2016] Sarma A, Chen X, Kuttal S, Dabbish L, Wang Z. Hiring in the Global Stage: Profiles of Online Contributions. In: Proc. 2016 IEEE International Conference on Global Software Engineering. ICGSE 2016. Institute of Electrical and Electronics Engineers (IEEE); 2016.

[scipy-coc] SciPy Code of Conduct; Accessed February 14, 2019. https://docs.scipy.org/doc/scipy/reference/dev/conduct/code\_of\_conduct.html.

[singh2012] Singh V. Newcomer integration and learning in technical support communities for open source software. In: Proc. 2012 ACM International Conference on Supporting Group Work - GROUP'12. ACM Press; 2012.

[steinmacher2013] Steinmacher I, Wiese I, Chaves AP, Gerosa MA. Why do newcomers abandon open source software projects? In: Proc. 2013 International Workshop on Cooperative and Human Aspects of Software Engineering (CHASE'13). Institute of Electrical and Electronics Engineers (IEEE); 2013.

[steinmacher2014] Steinmacher I, Wiese I, Conte T, Gerosa M, Redmiles D. The Hard Life of Open Source Software Project Newcomers. In: Proc. 2014 International Workshop on Cooperative and Human Aspects of Software Engineering (CHASE'14). ACM Press; 2014.

[steinmacher2015] Steinmacher I, Conte T, Gerosa MA, Redmiles D. Social Barriers Faced by Newcomers Placing Their First Contribution in Open Source Software Projects. In: Proc. 2015 ACM Conference on Computer Supported Cooperative Work & Social Computing. CSCW 2015. ACM Press; 2015.

[steinmacher2016] Steinmacher I, Conte TU, Treude C, Gerosa MA. Overcoming open source project entry barriers with a portal for newcomers. In: Proc. 2016 International Conference on Software Engineering (ICSE'16). ACM Press; 2016.

[steinmacher2018a] Steinmacher I, Pinto G, Wiese IS, Gerosa MA. Almost There: A Study on Quasi-Contributors in Open-Source Software Projects. In: Proc. 2018 International Conference on Software Engineering (ICSE'18). ACM Press; 2018.

[steinmacher2018b] Steinmacher I, Treude C, Gerosa MA. Let Me In: Guidelines for the Successful Onboarding of Newcomers to Open Source Projects. Software. 2018;doi:10.1109/MS.2018.110162131.

[tourani2017] Tourani P, Adams B, Serebrenik A. Code of Conduct in Open Source Projects. In: Proc. 2017 International Conference on Software Analysis, Evolution and Reengineering (SANER'17). IEEE; 2017.

[wenger1999] Wenger E. Communities of Practice: Learning, Meaning, and Identity. Cambridge University Press; 1999.

[zanatta2017] Zanatta AL, Steinmacher I, Machado LS, de Souza CRB, Prikladnicki R. Barriers Faced by Newcomers to Software-Crowdsourcing Projects. Software. 2017;34(2):37--43. doi:10.1109/ms.2017.32.
