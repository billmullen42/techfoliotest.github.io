---
layout: essay
type: essay
title: UX Design for a Desktop App
date: 2017-05-19
labels:
  - User Experience
  - Design Planning
---

This summer, I and 6 other students will be building a desktop application in Electron to allow users to easily create and maintain TechFolios profiles. Our first task is to identify pain points in the existing TechFolios  experience, using Github.

As a walkthrough I created a new project entry and uploaded a new essay. I am also drawing on my previous experience with TechFolios, including a résumé update about 3 weeks ago.

We had already discussed [preliminary app requirements](https://github.com/techfolios/designer), but I have tried to keep my suggestions broad to remain relevant with any requirements changes during development. Below I used the term "editor" to refer to a context in the new app where the user is editing information - this may end up being multiple contexts such as project-editor context and profile-editor context, but will be distinct from viewing the live profile and distinct from the potential "preview" context.

## Pain points that can be addressed

It should be clear from the editor which items in the bio file will be displayed in the resume file, and elsewhere. Currently, some fields appear in multiple areas of the profile, and some are not displayed in the live profile at all.

The editor should detect and highlight invalid syntax at all times. Currently, users are notified after the fact via email if syntax errors in the last commit prevent an update to the live profile, and users must locate these errors manually.

The status of essays and projects should be clear. Ideally, the desktop app would allow users to edit unpublished drafts and maintain multiple unpublished versions. It should be clear how to publish an essay or project, and always clear what the status (published or unpublished) of each is. Currently, it is difficult and confusing to have unpublished versions in a profile, and most users would opt to save drafts locally. Having local drafts may make it difficult to convert format from Word, for example, into a publishable format.

As a related issue, during my walkthrough I noticed that when I click on my newest essay it downloads a file, rather than linking to the essay page, as I expected, because I had left out the ".md" file extension. Error prevention should be a key goal.

Overall, TechFolios does well in its use of terminology. For some areas of the bio/resume, the suggested use of some fields could be clearer. For example, the default bio includes a languages/frameworks section, which also allows for sub-items that will appear in parentheses in the resume. The app should make the interface more similar to the final appearance, so that the functionality is clear. Additionally, example resumes that make use of the parentheses and resume tips would help users understand what sort of information should go where.

TechFolios has many options for image size and placement. Our editor should allow users familiar with html tags to use them, but we should provide a few good default options with the underlying html hidden from the user.

In a few cases, when TechFolio's didn't do what I wanted it to to, it revealed something that TechFolio's could do if desired. Some of these might be customizable options, which advanced users could make use of. But this desktop app is geared specifically at simplicity and streamlining, and should accomodate new and inexperienced users over advanced users. And given short development time, we should err on the side of simplicity over customizability.

Should be able to export resume file to other file formats (e.g. Word) easily, to facilitate job applications and consistency.
