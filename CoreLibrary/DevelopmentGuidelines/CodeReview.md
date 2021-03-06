# Code review guidelines



Doing static code reviews is a great way to improve code quality and share knowledge in a team.

- Read [this study](http://www.ibm.com/developerworks/rational/library/11-proven-practices-for-peer-review/) about code reviews at Cisco; lot of good tips there. Also, [this article](https://www.codeproject.com/Articles/1156196/Code-Review-Checklist) is an ideal and simple checklist that can be used for code review.
- It's best to use a tool for code review where you can give comment for specific lines in the code. [Bitbucket](https://bitbucket.org/) and [GitHub](https://github.com/) both offer code line commenting for commits and pull requests.
- When doing code review, not just look at the code lines but also try to understand the whole component you review pieces of. This way you can also give you opinion about higher-level architectural decisions.
- Pay attention to pinpoint all kinds of issues: e.g. architectural, logical, styling, maintainability issues all count.
- Don't just look at what's there but also think about what's missing (e.g. validation, error handling, access control...).
- If you see repeated issues with the code (e.g. the same mistake repeated all over the code base) then don't add the same comment multiple times. Either reference the other locations in a single comment (e.g. "This is also repeated in the other controllers here.") or if you're reviewing a bigger piece of code then collect such issues in a shared document (or a comment for the whole codebase if you tool allows it) and just reference them (e.g. "See CodeReview.docx #3").
- During the core review you can find issues of high importance, such as critical security problems. Apart from adding these to the affected piece of code also separately collect them to make them apparent.