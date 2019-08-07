---
layout: layout.pug
navigationTitle:  Multiple Clusters
title: Multiple Clusters
menuWeight: 3
excerpt: Using DC/OS to manage multiple clusters
---

Organizations typically deploy and manage multiple DC/OS clusters. Multiple clusters are used for isolation (e.g., testing vs production), accommodating geographic distribution, and so on. DC/OS multiple cluster operations make management and access of multiple DC/OS clusters easy for both operators and users.

DC/OS has two categories of operations for managing multiple clusters:

- **[Cluster connection](/mesosphere/dcos/1.12/administering-clusters/multiple-clusters/cluster-connections/)** - operations allow you to set up connections, authenticate, and attach to clusters to enable access to the cluster from the CLI.
- **[Cluster link](/mesosphere/dcos/1.12/administering-clusters/multiple-clusters/cluster-links/)** - operations allow you to create and remove links between clusters. Once you have authenticated to a cluster, in the CLI you can seamlessly attach to a linked cluster without having to repeat the connection and authentication steps. In the UI if the clusters share an [SSO provider](/mesosphere/dcos/1.12/security/ent/sso/) you can easily switch between linked clusters.