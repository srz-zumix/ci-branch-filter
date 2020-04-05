# ci-branch-filter

CI Trigger filter examples.

--------------------------------------------------

## Filters

|CI|Branch|Paths|Config|
|:--|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com)||||
|[Azure Pipelines](https://azure.microsoft.com/ja-jp/services/devops/pipelines/)|:ballot_box_with_check:||
|[Bitrise](https://www.bitrise.io)|:ballot_box_with_check:|[:ballot_box_with_check:](https://devcenter.bitrise.io/builds/selective_builds/)|GUI|
|[Buddy](https://buddy.works)|||
|[CircleCI](https://circleci.com/pricing/)|||
|[Cirrus CI](https://cirrus-ci.org/)|[:ballot_box_with_check:](https://cirrus-ci.org/guide/writing-tasks/#supported-functions)|[:ballot_box_with_check:](https://cirrus-ci.org/guide/writing-tasks/#supported-functions)|
|[Codefresh](https://codefresh.io/)|||
|[Codeship](https://codeship.com/)||
|[Drone](https://cloud.drone.io/)||
|[GitHub Actions](https://help.github.com/en/articles/about-github-actions)|[:ballot_box_with_check:](https://help.github.com/en/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestbranchestags)|[:ballot_box_with_check:](https://help.github.com/en/actions/reference/workflow-syntax-for-github-actions#onpushpull_requestpaths)|YAML|
|[Scrutinizer](https://scrutinizer-ci.com)||
|[Semaphore 2.0](https://semaphoreci.com/product)|||
|[Semaphore 2.0](https://semaphoreci.com/product)|||
|[Shippable](http://shippable.com)||
|[Travis CI](https://travis-ci.com/)|
|[wercker](http://www.wercker.com/)||


--------------------------------------------------

## CI Matrix

|CI|master|feature|||
|:--|:--|:--|:--|:--|
|[AppVeyor](https://www.appveyor.com/docs/how-to/filtering-commits/#skip-commits)|[![Build status](https://ci.appveyor.com/api/projects/status/yagkbieyahgxx7cd?svg=true)](https://ci.appveyor.com/project/srz-zumix/ci-branch-filter)||||
|[Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/?view=vsts)|[![Build Status](https://dev.azure.com/srz-zumix/ci-branch-filter/_apis/build/status/ci-branch-filter-CI)](https://dev.azure.com/srz-zumix/ci-branch-filter/_build/latest?definitionId=6)|||||
|[Bitrise](http://devcenter.bitrise.io/tips-and-tricks/skip-a-build/)|[![Build Status](https://app.bitrise.io/app/888b3fc92ca7352c/status.svg?token=1zo_JkiGKmgbqRGxtLdieQ&branch=master)](https://app.bitrise.io/app/888b3fc92ca7352c)|||||
|[Buddy](https://buddy.works/knowledge/deployments/how-use-commit-commands)|[![buddy pipeline](https://app.buddy.works/zumixcpp/ci-branch-filter/pipelines/pipeline/127277/badge.svg?token=5e58135ab4831252209e7b1fe75bfe9de669b0dc7e95ed4316eebad2187d59a0 "buddy pipeline")](https://app.buddy.works/zumixcpp/ci-branch-filter/pipelines/pipeline/127277)|||||
|[Circle CI](https://circleci.com/docs/1.0/skip-a-build/)|[![CircleCI](https://circleci.com/gh/srz-zumix/ci-branch-filter/tree/master.svg?style=svg)](https://circleci.com/gh/srz-zumix/ci-branch-filter/tree/master)||| | |
|[Cirrus CI](https://cirrus-ci.org/guide/writing-tasks/#conditional-task-execution)|[![Cirrus Build Status](https://api.cirrus-ci.com/github/srz-zumix/ci-branch-filter.svg?branch=master)](https://cirrus-ci.com/github/srz-zumix/ci-branch-filter/master)||| | |
|[Codefresh](https://docs.codefresh.io/v1.0/docs/conditional-execution-of-steps)|[![Codefresh build status]( https://g.codefresh.io/api/badges/build?repoOwner=srz-zumix&repoName=ci-branch-filter&branch=master&pipelineName=ci-branch-filter&accountName=srz-zumix&type=cf-1)]( https://g.codefresh.io/repositories/srz-zumix/ci-branch-filter/builds?filter=trigger:build;branch:master;service:5a8d6d36d78094000162db49~ci-branch-filter)|||||
[Codeship](https://documentation.codeship.com/general/projects/skipping-builds/)|[ ![Codeship Status for srz-zumix/ci-branch-filter](https://app.codeship.com/projects/00a08490-f92d-0135-3ab5-029b8e2f450f/status?branch=master)](https://app.codeship.com/projects/278452)|||||
|[Drone Cloud](https://cloud.drone.io/)|[![Build Status](https://cloud.drone.io/api/badges/srz-zumix/ci-branch-filter/status.svg)](https://cloud.drone.io/srz-zumix/ci-branch-filter)|||||
|[GitHub Actions](https://github.com/features/actions)|[![GitHub Actions Status](https://github.com/srz-zumix/iutest/workflows/GitHub%20Actions/badge.svg?branch=master)](https://github.com/srz-zumix/iutest/actions)|||||
|[Scrutinizer](https://scrutinizer-ci.com/docs/guides/skipping_a_build_via_commit_message)|[![Build Status](https://scrutinizer-ci.com/g/srz-zumix/ci-branch-filter/badges/build.png?b=master)](https://scrutinizer-ci.com/g/srz-zumix/ci-branch-filter/build-status/master)|||||
|[Semaphore CI](https://semaphoreci.com/docs/how-to-skip-building-for-some-commits-with-ci-branch-filter.html)|[![Build Status](https://semaphoreci.com/api/v1/srz_zumix/ci-branch-filter/branches/master/badge.svg)](https://semaphoreci.com/srz_zumix/ci-branch-filter)|||||
|[Semaphore CI 2.0](https://docs.semaphoreci.com/article/146-skip-building-some-commits-with-ci-branch-filter)|[Build](https://srz-zumix.semaphoreci.com/projects/ci-branch-filter)|||||
|[Shippable](http://docs.shippable.com/ci/skip-builds/)|[![Run Status](https://api.shippable.com/projects/5a8d7f96d0386507000fbc70/badge?branch=master)](https://app.shippable.com/github/srz-zumix/ci-branch-filter)|||||
|[Travis CI](https://docs.travis-ci.com/user/customizing-the-build/#building-specific-branches)|[![Build Status](https://travis-ci.com/srz-zumix/ci-branch-filter.svg?branch=master)](https://travis-ci.com/srz-zumix/ci-branch-filter)|||| |
|[wercker](http://devcenter.wercker.com/docs/faq/how-can-i-skip-a-build#hs_cos_wrapper_name)|[![wercker status](https://app.wercker.com/status/95dc13c5815e10848c9c7bafbba37e62/s/master "wercker status")](https://app.wercker.com/project/byKey/95dc13c5815e10848c9c7bafbba37e62)||| | |

