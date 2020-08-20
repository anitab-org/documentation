<h1>Pre-requisites for contributing towards Quality Assurance</h1>

1. Join [#quality-assurance](https://anitab-org.zulipchat.com/#narrow/stream/216325-quality-assurance) stream on Zulip. Tag @admins on Zulip to add you under the @qa-team tag.
2. Choose a [project](https://github.com/anitab-org)
   * Join the respective Zulip stream for that project
3. Setting up the environment of the project

   a. If testing dev environment (stage), you can use deployed versions. You need not setup up the dev environment locally.
      * [Mentorship Android](https://github.com/anitab-org/mentorship-android/tree/apk)
      * [Mentorship Flutter](https://github.com/anitab-org/mentorship-flutter/tree/apk)
      * [Mentoship Backend](https://mentorship-backend-temp.herokuapp.com/)
      * [Volunteer Management System](http://ec2-52-53-177-18.us-west-1.compute.amazonaws.com/en-us/)
      * [Portal](http://ec2-54-215-223-241.us-west-1.compute.amazonaws.com/)
      * [AnitaB.org Open Source Web](https://anitab-org.github.io/)
      
   b. If testing PRs, you have to setup the dev environment.
      * Mentorship Android:
        * [Dev Env Setup demo](https://anitab.zoom.us/rec/share/2uNHIJT-5EVJS7PzxVrWfK0oQtS1eaa81HdP-vVcyoErlalT9Mv00cK-ZvtOiMk?startTime=1589124944000)
        * [Dev Env Setup demo notes](https://docs.google.com/document/d/12D8356IenScM5DSRAITgg5X18tPZkRweXm_P-qmoQGY/edit)
        * [PR testing demo](https://anitab.zoom.us/rec/play/tJctd7j5rDk3SNWRtwSDUPUtW9XoJqis0iVL_fYFyBm1UyEKN1GmMrIaZ7RtkSCpQ2h7N8MOIMZc5wCD?startTime=1591118799000&_x_zm_rtaid=YOJgJH4BSZ65HhkWHNkhzg.1592773256165.ad77a44e5d4c2e726317ba090ee629b9&_x_zm_rhtaid=385)
      * Mentorship Flutter:
        * [Dev Environemnt Setup demo](https://anitab.zoom.us/rec/share/6MNVAO7pzE9OfNLP1m6EcJQrT6TgX6a81iRIrqAExUzyft37kQpq80KDeueJJKjY?startTime=1589108623000)
        * [Dev Environment Setup Notes](https://docs.google.com/document/d/1cLznYyN5VfVraN3swl81Yum1IXG3cyLyIdD85QOuGrY/edit?usp=sharing)
        * [PR testing demo](https://anitab.zoom.us/rec/play/vsEpIe2rpj03T9aSuQSDA_94W9W0J62shnAXqPINnUnmUXEHMAf0MOEVMOt-f8i1epVN8HeS5BurDHjH?startTime=1593537676000&_x_zm_rtaid=bRSfMzm_T4G4tNo7nBPtXQ.1593605707752.e181143531eb9176c6de82c23bf4f24a&_x_zm_rhtaid=490)
      * Mentorship Backend:
        * Dev Env Setup demo - [Recording 1](https://anitab.zoom.us/rec/share/2uNHIJT-5EVJS7PzxVrWfK0oQtS1eaa81HdP-vVcyoErlalT9Mv00cK-ZvtOiMk?startTime=1589121214000), [Recording 2](https://anitab.zoom.us/rec/share/2uNHIJT-5EVJS7PzxVrWfK0oQtS1eaa81HdP-vVcyoErlalT9Mv00cK-ZvtOiMk?startTime=1589121947000), [Recording 3](https://anitab.zoom.us/rec/share/2uNHIJT-5EVJS7PzxVrWfK0oQtS1eaa81HdP-vVcyoErlalT9Mv00cK-ZvtOiMk?startTime=1589122325000)
        * [Setup Notes](https://docs.google.com/document/d/1cOhwTMyo25n0sJLUfOjWTntzZwLTUTvCfL3fKJlKKmY/edit)
        * [Testing PR](https://github.com/anitab-org/mentorship-backend/blob/develop/docs/test-pr-guide.md#steps-to-test-a-pr)
      * VMS:
        * [Dev env setup demo](https://anitab.zoom.us/rec/share/xp1sE72v81xLRI3N81_VAa4ONZW8aaa81nBMq_UExE0n8GF03G1ifH1QShZHCvE7?startTime=1589115801000)
        * [Setup Notes](https://docs.google.com/document/d/1eJRmsf5lznb6Klym23P05qEb7vVLB9PWOlMm2ErRmXg/edit)
      * Portal:
        * [Dev env setup instructions](https://docs.google.com/document/d/1nL5c1xxse_ulHbjTgaHHv7XTIf41lQV0msYB7xesJGU/edit)
        * [Setup Notes](https://docs.google.com/document/d/1nL5c1xxse_ulHbjTgaHHv7XTIf41lQV0msYB7xesJGU/edit?usp=drivesdk)
      * AnitaB.org Open Source Web:
        * [Setup](https://github.com/anitab-org/anitab-org.github.io/blob/develop/README.md)
      * STEM Diverse TV:
        * [Setup](https://github.com/anitab-org/stem-diverse-android-tv/blob/master/README.md) 
    
4. Signup on the test management tool [TestQuality](https://anitab-org.testquality.com/signup). Ask on Zulip under #quality-assurance stream tagging @qa-team, to set up your account with the right permission to the project you have chosen.

<h3>How to test a PR?</h3>

1. Pick a PR from the project you have chosen which has the label `Needs Testing`.
2. Make sure the PR has 2 code review approvals before you start testing.
3. Go to the Issue that PR is fixing and follow the steps to reproduce that issue while you are under the develop branch.
4. Run the following commands to get to the PR branch, where <contributor> is the GitHub username of the contributor that submitted the PR:
  ```
  git clone https://github.com/<contributor>/mentorship-backend/
  git checkout <branch-name>
  ```
5. Verify the code addition/deletions in the PR.
6. Reproduce the issue and test the fix.
7. Leave a review comment on the PR using the following template:
  ```
  The changes made in this PR were tested locally. Following are the results:

  1. Code review - Done or Not Done

  2. All possible responses (positive and negative tests) were tested as below:

     * _Test1 Description_  
       _Screenshot/gif_:  
       _Expected Result_:  
       _Actual Result_:
     * _Test2 Description_  
       _Screenshot/gif_:  
       _Expected Result_:  
       _Actual Result_:  
       ...  
    
  3. Additional testcases covered:

     * _Test1 Description_  
       _Screenshot/gif_:  
       _Expected Result_:  
       _Actual Result_:
    
  4. Additional Comments:

  5. Status of PR Changed to: Needs Review or Ready to Merge.
  ```

<h1>Quality Assurance Guidelines</h1>

1. Choose a test scenario in the project you’ve chosen and execute it on either the PR or deployed version that is being tested.
   * Open issues under the respective github repo if you find any bugs.

2. Search on TestQuality if the Test Case is already documented. If not, document the testcase on TestQuality under the repective Test Plan and Test Suite. Here is a [demo](https://drive.google.com/file/d/1pkxCAPR9G3lYjUf_Ym8bmuglDWBdEU2c/view?usp=sharing).
   * Have the Test Case reviewed by another QA team member.

3. (Optional) Automate the Test Case, for example: [Mentorship Backend User Journey](https://github.com/anitab-org/mentorship-backend/pull/708).

4. If you decide to skip step 3, search if there is an existing issue to automate that test case. If not, open a issue with label `Quality Assurance`.

5. If you automate a Test case make sure you mark it as `Automated` on TestQuality.
