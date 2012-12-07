#Voices
##Overview##
Voter turnout in Canada is almost a full 20% lower than it's peak in 1963. Across all demographics, Canadians are more likely to have a facebook account then they are to vote. Canadians under 30 are the least likely demographic to vote, and yet a 2005 Statcan study found that 70% of young Canadians are involved in some form of non-voting political behavior. Why? The main reason appears to be apathy. Canadians, especially young Canadians, simply don't care enough about politics to bother with voting. I propose that a major reason for this is that it is incredibly difficult to find out what your politicians are actually doing. For a generation of people able to access almost any piece of information in seconds, our political system can seem decidedly archaic.

**Voices aims to change that.** Voices will be a comprehensive application system that will keep Canadians informed about their government's precedings. The idea is simple: a web based application for desktops, laptops, tablets, and smartphones, integrated with social media, that provides a citizen with a profile detailing upcoming motions in their legislatures. A user can specify their personal opinion on the motion. Summaries of the issues should be short and neutral, with links to fuller text and related articles. In addition, a summary of the past week will be presented, detailing the outcome of the motions voted upon and summarizing how that citizen's representatives voted.

**Politicians benefit too.** Those that choose to opt in will recieve a similar weekly breakdown detailing the opinions of their consitutuents.

##Details##
The Voices project technically will consist of two main sections:
  - An open backend API that will expose data about government precedings to the entire internet for anyone to use
      - Will likely be built with node.js and MongoDB in order to facillitate flexibilty, scaling, and ease of development
      - Will serve data from multiple sources, such as online news aggregators and official government sites
      - Will likely be hosted on Heroku, at least in the short term.
  - A collection of applications for all devices that will use the backend to deliver meaningful experiences to users
      - The mobile clients will likely be built with PhoneGap in order to reuse as much code ss possible and keep a consistent experience across devices

Development of Voices will be done primarily by student volunteers, and will take input from politicians, users, and other project stakeholders.
      
##Rules##
- **Voices must remain neutral.** All data presented directly in the application must be as neutral as possible and should not attempt to explain anything through a politicized lense
- **The data must be open.** The backend system that provides data to the Voices applications will be an open API that will allow others to iterate and innovate.
- **Voices applications must be free.** Any cost, no matter how small, is prohibitive to somebody. Excluding people from the political process is in direct opposition to the goals of this project.

##Roadmap##
1. Discuss the Voices project with people at various levels of government in order to decide on a logical launching point. The choices right now appear to be a) starting at the municipal level in order to build a core group of testers and validate the idea *or* b) go for broke and hack out a solution that works at the federal level and drive use post-development
2. Find data sources. Titles, summaries, relevant news articles, and the like all need to come from somewhere; the sources will depend on the launching point chosen in item 1.
3. Stage mockups of front-end clients. The clients will be staged in such a manner to fit the data obtained from step 2. The mockups will be used in order to help drive interest in the project, and will be an integral part of the next few steps.
3. Build out a comprehensive backend API. Finalize node.js and MongoDB as the tools of choice, and scaffold up a solution. The backend should be built to fit the mockups.
4. Build out the user profiling system, including account structure and social media integration. This might be within the same server application as the data-server, or not. TBD.
4. Build out clients. The clients can be built by different teams for different platforms, however the backend API usage, branding, and overall workflow must remain consistent across platforms
5. Test with a small group of users, ideally centered around a few politicians, in order to get quick feedback to iterate on.
6. Obtain funding for scaling. **If at all possible, funding should come from anonymous donations.**
7. Scale