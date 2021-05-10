# Pull request lifecycle

→ PR Template is necessary
→ PR needs to link to the issue #
	→ Issue needs to be validated (at least 1 person from the “core team” of the project)
	→ Issue needs to be assigned to the person who submitted the PR 

**Status: Needs Review**

→ Minimum Reviews = 2 PR Reviews from any person (at least 1 PR Review from a Maintainer)
	→ if successful, 
	Status Change → Label “Status: Needs Testing”
→ if not successful, the Reviewer pings the author to let them know where PR failed. Contributor is responsible for making changes.
		Status Change → Label “Status: Changes Requested”

**Status: Needs Testing**

→ Minimum QA = 1 QA report (using [this template](quality-assurance.md#how-to-test-a-pr)) from any person (except the author)
→ If successful, 
		Status Change → Label “Status: Ready to Merge”
→ If not successful, QA pings author to let them know where PR failed. Contributor is responsible for making changes.
	Status Change → Label “Status: Changes Requested”

**Status: Ready to Merge**

→ Minimum Final Check = Code Owners are responsible for making sure the PR went through the whole process. If true, then they merge. If false, they decide what’s best.  
→ Code Owners (“release managers”) can be Admins, Maintainers, Open Source Ambassadors, or Open Source Program Mentors. They are -invite only- by Admins.
