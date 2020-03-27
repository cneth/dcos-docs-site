---
layout: layout.pug
navigationTitle: Release notes for 2.0.3
title: Release notes for 2.0.3
menuWeight: 0
excerpt: Release notes for DC/OS 2.0.3, including Open Source attribution, and version policy.
---
DC/OS&trade; 2.0.3 was released on 19 March 2020.

[button color="light" href="https://downloads.dcos.io/dcos/stable/2.0.3/dcos_generate_config.sh"]Download DC/OS Open Source[/button]

[button color="purple" href="https://downloads.mesosphere.com/dcos-enterprise/stable/2.0.3/dcos_generate_config.ee.sh"]Download DC/OS Enterprise* [/button]

Registered DC/OS Enterprise customers can access the DC/OS Enterprise configuration file from the [support website](https://support.mesosphere.com/s/downloads). For new customers, contact your sales representative or <a href="mailto:sales@mesosphere.io">sales@mesosphere.io</a> before attempting to download and install DC/OS Enterprise.

# Release Summary
DC/OS is a distributed operating system that enables you to manage resources, application deployment, data services, networking, and security in an on-premise, cloud, or hybrid cluster environment.

# DC/OS 

## Components

DC/OS 2.0.3 includes the following component versions:

- Apache&reg; Mesos&reg; 1.8.2-dev
- OpenSSL 1.1.1d	

### DC/OS Fixed and Improved Issues

- Fixed an issue where image pull in UCR was not working for nvcr.io (missing ‘service’/‘scope’ parameters). (COPS-5804)
- Fixed an issue where after a DC/OS upgrade, the executor resources used by tasks on the agent were being incorrectly counted against quota. (COPS-5725)
- DC/OS Admin Router now allows large packages of files, up to 32GB, to the Package Registry. (D2IQ-61233, COPS-5615)
- Fixed an issue where in some rare circumstances, after upgrading a cluster from DC/OS 1.11 to DC/OS 1.13 users were no longer able to launch tasks that use the UCR containerizer. (D2IQ-64507, COPS-5868)

# Marathon

## Components

DC/OS 2.0.3 includes the following Marathon&trade; component version:

- Marathon 1.8.239

### Marathon Fixed and Improved Issues

- Improved the expunge logic so that it evaluates in the same timely manner that unreachable inactive evaluates. (COPS-5617)