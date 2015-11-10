jsk_common
===

[![Build Status](https://travis-ci.org/jsk-ros-pkg/jsk_common.svg?branch=master)](https://travis-ci.org/jsk-ros-pkg/jsk_common)
[![Read the Docs](https://readthedocs.org/projects/pip/badge/?version=latest)](https://jsk-common.readthedocs.org)
[![Slack](https://img.shields.io/badge/slack-jsk--robotics-e100e1.svg)](http://jsk-robotics.slack.com)
[![Join the chat at https://gitter.im/jsk-ros-pkg/jsk_common](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/jsk-ros-pkg/jsk_common?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Deb Build Status
------------

Package | Indigo (Saucy) | Indigo (Trusty) | Jade (Trusty) | Jade (Utopic) | Jade (Vivid)
------- | -------------- | --------------- | ------------- | ------------- | ------------
jsk_common (32-bit) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-indigo-jsk-common_binarydeb_saucy_i386)](http://jenkins.ros.org/job/ros-indigo-jsk-common_binarydeb_saucy_i386/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-indigo-jsk-common_binarydeb_trusty_i386)](http://jenkins.ros.org/job/ros-indigo-jsk-common_binarydeb_trusty_i386/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_trusty_i386)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_trusty_i386/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_utopic_i386)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_utopic_i386/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_vivid_i386)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_vivid_i386/) |
jsk_common (64-bit) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-indigo-jsk-common_binarydeb_saucy_amd64)](http://jenkins.ros.org/job/ros-indigo-jsk-common_binarydeb_saucy_amd64/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-indigo-jsk-common_binarydeb_trusty_amd64)](http://jenkins.ros.org/job/ros-indigo-jsk-common_binarydeb_trusty_amd64/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_trusty_amd64)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_trusty_amd64/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_utopic_amd64)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_utopic_amd64/) | [![Build Status](http://jenkins.ros.org/buildStatus/icon?job=ros-jade-jsk-common_binarydeb_vivid_amd64)](http://jenkins.ros.org/job/ros-jade-jsk-common_binarydeb_vivid_amd64/) |


Install
---
You can use `jsk.rosbuild` to setup your environment.


```sh
wget -q -O /tmp/jsk.rosbuild https://raw.github.com/jsk-ros-pkg/jsk_common/master/jsk.rosbuild
bash /tmp/jsk.rosbuild hydro
```

For hacker

```sh
wget -q -O /tmp/jsk.rosbuild https://raw.github.com/jsk-ros-pkg/jsk_common/master/jsk.rosbuild
bash /tmp/jsk.rosbuild --from-source hydro
```

For hrpsys user

```sh
wget -q -O /tmp/jsk.rosbuild https://raw.github.com/jsk-ros-pkg/jsk_common/master/jsk.rosbuild
bash /tmp/jsk.rosbuild --rtm hydro
```

For hrpsys hacker

```sh
wget -q -O /tmp/jsk.rosbuild https://raw.github.com/jsk-ros-pkg/jsk_common/master/jsk.rosbuild
bash /tmp/jsk.rosbuild --from-source --rtm hydro
```

`jsk.rosbuild` generates filesystem as follows:

```
~ --- ros
       + --- hydro_parent: Only availabe if --from-source option is enabled
              + --- src:   maintained by wstool
              + --- build: generated by catkin_tools
              + --- devel: generated by catkin_tools
       +--- hydro
             + --- src:    maintained by wstool
             + --- build:  generated by catkin_tools
             + --- devel:  generated by catkin_tools
```

Watch all the jsk github repositories.
===
Please use [this](http://jsk-github-watcher.herokuapp.com/)

Slack for JSK Lab members ![](https://upload.wikimedia.org/wikipedia/en/7/76/Slack_Icon.png)
=========================
You can login to [slack](https://slack.com/) from [here](https://jsk-robotics.slack.com).
You can create account using imi address.

[scudcloud](https://github.com/raelgc/scudcloud) is a desktop client for slack and you can install it
by following [instruction](https://github.com/raelgc/scudcloud#ubuntukubuntu-mint-and-debian).

You can restart travis and jenkins from slack's `#travis` channel.

Restart travis from slack
-------------------------
![](images/restart_travis.png)

Type `restart travis <job-id>` from slack#travis channel.

**N.B.: `<job-id>` is not the number of Pull-request.**

you can get `<job-id>` from Travis page.

- ![](images/PR_page.png)
- ![](images/Travis_page.png)

Restart docker from slack
-------------------------
![](images/restart_docker.png)

Type `restart docker` from slack#travis channel.
