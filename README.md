# ci-trigger

CI Trigger Congigurations

--------------------------------------------------

## Filters

### Commit comment

[CI Skip](https://github.com/srz-zumix/ci-skip)

### Event

### Branch

Branch: branch name filter.
Branch(PR): pull request (BASE|HEAD) branch name filter, link if there is a separate setting.
Paths: path filter.
Config: where to set.
Skip push/pr: skip duplicate trigger push and PR.

|CI|Branch|Branch(PR)|Skip push/pr|Config|
|:--|:--|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com/docs/branches/)|:ballot_box_with_check:|BASE|[:ballot_box_with_check:](https://www.appveyor.com/docs/how-to/filtering-commits/)|YAML|
|[Azure Pipelines](https://docs.microsoft.com/ja-jp/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#branches)|:ballot_box_with_check:|||[GUI](https://docs.microsoft.com/en-us/azure/devops/pipelines/troubleshooting/troubleshooting?view=azure-devops#overridden-yaml-trigger-setting),YAML|
|[Bitrise](https://www.bitrise.io)|:ballot_box_with_check:|||GUI|
|[Buddy](https://buddy.works)||||
|[CircleCI](https://circleci.com/docs/ja/2.0/configuration-reference/#filters)|:ballot_box_with_check:|||YAML|
|[Cirrus CI](https://cirrus-ci.org/guide/writing-tasks/#supported-functions)|:ballot_box_with_check:|||YAML|
|[Codefresh](https://codefresh.io/docs/docs/configure-ci-cd-pipeline/triggers/git-triggers/)|[:ballot_box_with_check:](https://codefresh.io/docs/docs/configure-ci-cd-pipeline/triggers/git-triggers/)|||GUI|
|[CodeShip Basic](https://documentation.codeship.com/general/projects/build_trigger/)|:ballot_box_with_check:|||GUI,YAML|
|[CodeShip Pro](https://documentation.codeship.com/pro/builds-and-configuration/steps/#limiting-steps-to-specific-branches-or-tags)|:ballot_box_with_check:|||GUI,YAML|
|[Drone](https://docs.drone.io/pipeline/triggers/)|:ballot_box_with_check:|||YAML|
|[GitHub Actions](https://help.github.com/en/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestbranchestags)|:ballot_box_with_check:|||YAML|
|[RezorOps](https://docs.razorops.com/config/spec/#trigger)|:ballot_box_with_check:|||GUI,YAML|
|[Scrutinizer](https://scrutinizer-ci.com)||
|[Semaphore 2.0](https://docs.semaphoreci.com/reference/conditions-reference/)|:ballot_box_with_check:|||YAML|
|[Shippable](http://docs.shippable.com/platform/workflow/config/)|:ballot_box_with_check:|||YAML|
|[Travis CI](https://docs.travis-ci.com/user/customizing-the-build#building-specific-branches)|:ballot_box_with_check:|||YAML|
|[wercker](https://devcenter.wercker.com/development/workflows/creating-a-workflow/#tag-filtering)|:ballot_box_with_check:|||GUI|

--------------------------------------------------

#### Status

HEAD: feature/hoge
BASE: XXX

|CI|master|${CI}/feature|
|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com/docs/how-to/filtering-commits/#skip-commits)|[![Build status](https://ci.appveyor.com/api/projects/status/llmsixpmf2e7jy4k/branch/master?svg=true)](https://ci.appveyor.com/project/srz-zumix/ci-trigger)|[![Build status](https://ci.appveyor.com/api/projects/status/llmsixpmf2e7jy4k/branch/appveyor/feature?svg=true)](https://ci.appveyor.com/project/srz-zumix/ci-trigger)|
|[Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/?view=vsts)|[![Build Status](https://dev.azure.com/srz-zumix/ci-specs/_apis/build/status/ci-trigger?branchName=master)](https://dev.azure.com/srz-zumix/ci-specs/_build/latest?definitionId=11&branchName=master)|[![Build Status](https://dev.azure.com/srz-zumix/ci-specs/_apis/build/status/ci-trigger?branchName=azp%2Ffeature)](https://dev.azure.com/srz-zumix/ci-specs/_build/latest?definitionId=11&branchName=azp%2Ffeature)|
|[Bitrise](http://devcenter.bitrise.io/tips-and-tricks/skip-a-build/)|[![Build Status](https://app.bitrise.io/app/888b3fc92ca7352c/status.svg?token=1zo_JkiGKmgbqRGxtLdieQ&branch=master)](https://app.bitrise.io/app/888b3fc92ca7352c)||
|[Buddy](https://buddy.works/knowledge/deployments/how-use-commit-commands)|[![buddy pipeline](https://app.buddy.works/zumixcpp/ci-branch-filter/pipelines/pipeline/127277/badge.svg?token=5e58135ab4831252209e7b1fe75bfe9de669b0dc7e95ed4316eebad2187d59a0 "buddy pipeline")](https://app.buddy.works/zumixcpp/ci-branch-filter/pipelines/pipeline/127277)||
|[Circle CI](https://circleci.com/docs/1.0/skip-a-build/)|[![CircleCI](https://circleci.com/gh/srz-zumix/ci-branch-filter/tree/master.svg?style=svg)](https://circleci.com/gh/srz-zumix/ci-branch-filter/tree/master)||
|[Cirrus CI](https://cirrus-ci.org/guide/writing-tasks/#conditional-task-execution)|[![Cirrus Build Status](https://api.cirrus-ci.com/github/srz-zumix/ci-branch-filter.svg?branch=master)](https://cirrus-ci.com/github/srz-zumix/ci-branch-filter/master)||
|[Codefresh](https://docs.codefresh.io/v1.0/docs/conditional-execution-of-steps)|[![Codefresh build status]( https://g.codefresh.io/api/badges/build?repoOwner=srz-zumix&repoName=ci-branch-filter&branch=master&pipelineName=ci-branch-filter&accountName=srz-zumix&type=cf-1)]( https://g.codefresh.io/repositories/srz-zumix/ci-branch-filter/builds?filter=trigger:build;branch:master;service:5a8d6d36d78094000162db49~ci-branch-filter)||
[Codeship](https://documentation.codeship.com/general/projects/skipping-builds/)|[ ![Codeship Status for srz-zumix/ci-branch-filter](https://app.codeship.com/projects/00a08490-f92d-0135-3ab5-029b8e2f450f/status?branch=master)](https://app.codeship.com/projects/278452)||
|[Drone Cloud](https://cloud.drone.io/)|[![Build Status](https://cloud.drone.io/api/badges/srz-zumix/ci-branch-filter/status.svg)](https://cloud.drone.io/srz-zumix/ci-branch-filter)||
|[GitHub Actions](https://github.com/features/actions)|[![GitHub Actions Status](https://github.com/srz-zumix/iutest/workflows/GitHub%20Actions/badge.svg?branch=master)](https://github.com/srz-zumix/iutest/actions)||
|RazorOps|[![Build Status](https://api.razorops.com/apps/purple-frog-6791/badge.svg?branch=master)](https://dashboard.razorops.com/apps/purple-frog-6791/workflows)|[![Build Status](https://api.razorops.com/apps/purple-frog-6791/badge.svg?branch=razorops%2Ffeature)](https://dashboard.razorops.com/apps/purple-frog-6791/workflows)|
|[Scrutinizer](https://scrutinizer-ci.com/docs/guides/skipping_a_build_via_commit_message)|[![Build Status](https://scrutinizer-ci.com/g/srz-zumix/ci-branch-filter/badges/build.png?b=master)](https://scrutinizer-ci.com/g/srz-zumix/ci-branch-filter/build-status/master)||
|[Semaphore CI 2.0](https://docs.semaphoreci.com/article/146-skip-building-some-commits-with-ci-branch-filter)|[Build](https://srz-zumix.semaphoreci.com/projects/ci-branch-filter)||
|[Shippable](http://docs.shippable.com/ci/skip-builds/)|[![Run Status](https://api.shippable.com/projects/5a8d7f96d0386507000fbc70/badge?branch=master)](https://app.shippable.com/github/srz-zumix/ci-branch-filter)||
|[Travis CI](https://docs.travis-ci.com/user/customizing-the-build/#building-specific-branches)|[![Build Status](https://travis-ci.com/srz-zumix/ci-branch-filter.svg?branch=master)](https://travis-ci.com/srz-zumix/ci-branch-filter)||
|[wercker](http://devcenter.wercker.com/docs/faq/how-can-i-skip-a-build#hs_cos_wrapper_name)|[![wercker status](https://app.wercker.com/status/95dc13c5815e10848c9c7bafbba37e62/s/master "wercker status")](https://app.wercker.com/project/byKey/95dc13c5815e10848c9c7bafbba37e62)||

### Paths

|CI|Paths|Config|
|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com/docs/how-to/filtering-commits/)|:ballot_box_with_check:|YAML|
|[Azure Pipelines][]|-|-|
|[Bitrise](https://devcenter.bitrise.io/builds/selective_builds/)|:ballot_box_with_check:|GUI|
|[Buddy][]||||
|[CircleCI][]|-|-|
|[Cirrus CI](https://cirrus-ci.org/guide/writing-tasks/#supported-functions)|:ballot_box_with_check:|YAML|
|[Codefresh](https://codefresh.io/docs/docs/configure-ci-cd-pipeline/triggers/git-triggers/)|:ballot_box_with_check:|GUI|
|[CodeShip Basic][]|-|-|
|[CodeShip Pro][]|-|-|
|[Drone][]|-|-|
|[GitHub Actions](https://help.github.com/en/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestpaths)|:ballot_box_with_check:|YAML|
|[RezorOps](https://docs.razorops.com/config/spec/#trigger)|:ballot_box_with_check:|GUI|
|[Scrutinizer](https://scrutinizer-ci.com)||
|[Semaphore](https://docs.semaphoreci.com/reference/conditions-reference/#change_in)|beta|YAML|
|[Shippable][]|-|-|
|[Travis CI](https://travis-ci.community/t/how-to-skip-jobs-based-on-the-files-changed-in-a-subdirectory/2979/11)|workaround|AML|
|[wercker][]|||

## PullRequest Comment Command

[Comment assistance tampermonkey user script](https://github.com/srz-zumix/TampermonkeyUserScripts)

|CI|Command|Note|
|:--|:--|:--|
|[AppVeyor](https://status.appveyor.com/#)||
|[Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml#comment-triggers)|/AzurePipelines run \[pipeline-name\]|For brevity, you can comment using /azp instead of /AzurePipelines.|
|[Bitrise](https://www.bitrise.io)||
|[Buddy](https://buddy.works)||
|[CircleCI](https://status.circleci.com/)||
|[Cirrus CI](https://cirrus-ci.org/)||
|[Codefresh](https://codefresh.io/)||
|[Codeship](https://codeship.com/)||
|[Drone Cloud](https://cloud.drone.io/)||
|[GitHub Actions](https://www.githubstatus.com/)||
|[Razorops](https://razorops.com/)||
|[Scrutinizer](https://scrutinizer-ci.com)||
|[Semaphore CI 2.0](https://status.semaphoreci.com/)||
|[Shippable](http://shippable.com)||
|[Travis CI](https://travis-ci.com/)||
|[wercker](http://status.wercker.com/)||

## Webhook

[Appcircle]:https://appcircle.io/
[AppVeyor]:https://www.appveyor.com
[Azure Pipelines]:https://azure.microsoft.com/ja-jp/services/devops/pipelines/
[Bitrise]:https://www.bitrise.io
[Buddy]:https://buddy.works
[CircleCI]:https://circleci.com
[Cirrus CI]:https://cirrus-ci.org/
[Codefresh]:https://codefresh.io/
[Codeship]:https://codeship.com/
[Drone]:https://cloud.drone.io/
[GitHub Actions]:https://help.github.com/en/articles/about-github-actions
[Peakflow]:https://www.peakflow.io/
[Razorops]:https://razorops.com/
[Scrutinizer]:https://scrutinizer-ci.com
[Semaphore]:https://semaphoreci.com/product
[Shippable]:http://shippable.com
[Travis CI]:https://travis-ci.com/
[wercker]:http://www.wercker.com/
