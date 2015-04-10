We love community submissions!

To get started, please <a href="https://www.clahub.com/agreements/OSBI/saiku">sign the Contributor License Agreement</a> so we can accept your pull requests. 

We develop using the git flow framework, please develop against the development branch, although how you develop against your own fork is up to you, pull requests against master will no longer be accepted.

For people developing directly in our repository please create feature branches, hot fix branches, and release branches, you can do this manually but we have a mavne plugin to make life easier:

== Feature Branches ==


== Hot Fix Branches ==

Hot fixes are releases forked from the latest release branch and merged back into master and development. After you have completed a hotfix a new release should be issued.

*Create a hot fix*
mvn jgitflow:hotfix-start

*Finish a hot fix*
mvn jgitflow:hotfix-finish -DkeepBranch -DnoHotfixBuild

== Release Branches ==

Release branches are created when the development branch is feature complete, if not bug free. Once a release branch has been created you are still free to fix bugs within the release branch.

*Create Release Branch*
mvn jgitflow:release-start

*Finish Release*
mvn jgitflow:release-finish -DnoReleaseBuild