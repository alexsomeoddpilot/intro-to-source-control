## Source Code

In computing, source code is any collection of computer instructions (possibly with comments) written using some human-readable computer language, usually as text. The source code of a program is specially designed to facilitate the work of computer programmers, who specify the actions to be performed by a computer mostly by writing source code.

[Source Code - Wiki][wiki-source]

## Open Source

In production and development, open source as a development model promotes a universal access via free license to a product's design or blueprint, and universal redistribution of that design or blueprint, including subsequent improvements to it by anyone.

Researchers view open source as a specific case of the greater pattern of Open Collaboration, "any system of innovation or production that relies on goal-oriented yet loosely coordinated participants, who interact to create a product (or service) of economic value, which they make available to contributors and non-contributors alike".

Open source gained hold with the rise of the Internet, and the attendant need for massive retooling of the computing source code. Opening the source code enabled a self-enhancing diversity of production models, communication paths, and interactive communities. The open-source software movement arose to clarify the environment that the new copyright, licensing, domain, and consumer issues created.
 
Generally, open source refers to a computer program in which the [source code](#source-code) is available to the general public for use and/or modification from its original design. Open-source code is typically a collaborative effort where programmers improve upon the source code and share the changes within the community so that other members can help improve it further.

All of our development work is based on open source libraries which include Webkit, Unix, Apache, PHP, Javascript, jQuery, Wordpress, etc.

[Open Source - Wiki][wiki-osource]

## Closed Source

Proprietary software or closed source software is computer software licensed under exclusive legal right of the copyright holder with the intent that the licensee is given the right to use the software only under certain conditions, and restricted from other uses, such as modification, sharing, studying, redistribution, or reverse engineering. Usually the source code of proprietary software is not made available.

Most (if not all) of the development work we currently produce is closed source. Source code is not publicly available for our projects.

[Closed Source - Wiki][wiki-csource]

## What is a version/revision control system?

Revision control, also known as version control and source control is the management of changes to documents, computer programs, large web sites, and other collections of information. Changes are usually identified by a number or letter code, termed the ["commit"](#commit). Each revision is associated with a timestamp and the person making the change. Revisions can be [compared](#diff), restored, and with some types of files, [merged](#merge).

As teams design, develop and deploy software, it is common for multiple versions of the same software to be deployed in different sites and for the software's developers to be working simultaneously on updates. Bugs or features of the software are often only present in certain versions (because of the fixing of some problems and the introduction of others as the program develops). Therefore, for the purposes of locating and fixing bugs, it is vitally important to be able to retrieve and run different versions of the software to determine in which version(s) the problem occurs. It may also be necessary to develop two versions of the software concurrently (for instance, where one version has bugs fixed, but no new features (branch), while the other version is where new features are worked on (trunk).

At the simplest level, developers could simply retain multiple copies of the different versions of the program, and label them appropriately. This simple approach has been used on many large software projects. While this method can work, it is inefficient as many near-identical copies of the program have to be maintained. This requires a lot of self-discipline on the part of developers, and often leads to mistakes. Consequently, systems to automate some or all of the revision control process have been developed.

[Revision Control - Wikipedia][wiki-revisioncontrol]

## What is Git?

Git thinks of data like a set of snapshots of a mini filesystem. Every time you [commit](#commit), or save the state of your project in Git, it basically takes a picture of what all your files look like at that moment and stores a reference to that snapshot. To be efficient, if files have not changed, Git doesn’t store the file again—just a link to the previous identical file it has already stored.

Most operations in Git only need local files and resources to operate — generally no information is needed from another computer on your network. Because you have the entire history of the project right there on your local disk, most operations seem almost instantaneous.

When you do actions in Git, nearly all of them only add data to the Git database. It is very difficult to get the system to do anything that is not undoable or to make it erase data in any way. As in any VCS, you can lose or mess up changes you haven’t committed yet; but after you commit a snapshot into Git, it is very difficult to lose, especially if you regularly push your database to another repository.

This makes using Git a joy because we know we can experiment without the danger of severely screwing things up.

[Getting Started - Git][git-basics]

## What is Bitbucket?

Bitbucket is a is a web-based hosting service for projects that use [Git](#what-is-git) revision control systems.

Bitbucket is distinct in that it offers:

* Unlimited private ([closed source](#closed-source)) repositories
* Limited user accounts per repository

[Bitbucket - Wikipedia][wiki-bitbucket]

## Repositories

## Commit

A commit is the making of a set of tentative changes permanent. In the context of revision control, "commit" refers to submitting the latest changes of the source code to the repository, and making these changes part of the head revision of the repository.

[Commit - Wikipedia][wiki-commit]

In the context of Git, commits are snapshots of changes to the files in a project. As changes are made to the code, these changes are commited, and the results are displayed as [diffs](#diff) between commits.

## Diff

A diff is a file comparison utility that outputs the differences between two files. Diff is line-oriented rather than character-oriented in that it tries to determine the smallest set of deletions and insertions to create one file from the other. 

The `diff` command displays the changes made in a standard format, such that both humans and machines can understand the changes and apply them: given one file and the changes, the other file can be created. Typically, diff is used to show the changes between two versions of the same file.

The output is called a "diff", or a patch, since the output can be applied with the Unix program patch. The output of similar file comparison utilities are also called a "diff"; like the use of the word "grep" for describing the act of searching, the word diff is used in jargon as a verb for calculating any difference.

[Diff - Wikipedia][wiki-diff]

## Branch

Branching is the duplication of an object under revision control so that modifications can happen in parallel along both branches.

Branching also generally implies the ability to later merge or integrate changes back onto the parent branch. Often the changes are [merged](#merge) back to the trunk, even if this is not the parent branch. A branch not intended to be merged (e.g. because it has been relicensed under an incompatible license by a third party, or it attempts to serve a different purpose) is usually called a fork.

[Branching - Wikipedia][wiki-branch]

## Fork

In software engineering, a project fork happens when developers take a copy of source code from one software package and start independent development on it, creating a distinct piece of software. The term often implies not merely a development [branch](#branch), but a split in the developer community, a form of schism.

Free and open-source software is that which, by definition, may be forked from the original development team without prior permission without violating any copyright law. However, licensed forks of proprietary software (e.g. Unix) also happen.

[Fork - Wikipedia][wiki-fork]

## Issue Tracking System

An issue tracking system is a computer software package that manages and maintains lists of issues, as needed by an organization. Consistent use of an issue or bug tracking system is considered one of the "hallmarks of a good software team".

A ticket element or issue, within an issue tracking system, is a running report on a particular problem, its status, and other relevant data. Tickets have a unique reference number, also known as a case, issue or call log number which is used to allow the user or help staff to quickly locate, add to or communicate the status of the user's issue or request.

[Issue Tracking - Wikipedia][wiki-issue]

Basecamp "Todos" are a rudimentary issue tracking system. Bitbucket and Github offer a more nuanced issue tracking system.

[wiki-bitbucket]: http://en.wikipedia.org/wiki/Bitbucket
[wiki-revisioncontrol]: http://en.wikipedia.org/wiki/Revision_control
[git-basics]: http://git-scm.com/book/en/Getting-Started-Git-Basics
[wiki-source]: http://en.wikipedia.org/wiki/Source_code
[wiki-osource]: http://en.wikipedia.org/wiki/Open_source
[wiki-csource]: http://en.wikipedia.org/wiki/Closed_source
[wiki-commit]: http://en.wikipedia.org/wiki/Commit_(data_management)
[wiki-diff]: http://en.wikipedia.org/wiki/Diff
[wiki-branch]: http://en.wikipedia.org/wiki/Branching_(revision_control)
[wiki-fork]: http://en.wikipedia.org/wiki/Fork_(software_development)
[wiki-issue]: http://en.wikipedia.org/wiki/Issue_tracking_system
