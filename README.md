# Awesome Chef [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of amazingly awesome open source Chef resources. [Chef](http://chef.io) is a systems and cloud infrastructure automation framework that makes it easy to deploy servers and applications to any physical, virtual, or cloud location, no matter the size of the infrastructure.

## Table of Contents
  * [Basics](#basics)
  * [Cookbooks](#cookbooks)
  * [Resources](#resources)
  * [Podcasts](#podcasts)
  * [Chef handlers](#chef-handlers)
  * [Add-ons](#add-ons)
  * [Books](#books)
  * [Newsletters](#newsletters)
  * [Articles](#articles)

See [Contribution Guidelines](#contribution-guidelines)

## Basics
* [Chef (software)](https://en.wikipedia.org/wiki/Chef_(software)) - An article in Wikipedia.
* [An Overview](https://docs.chef.io/chef_overview.html) - by official chef.io.
* [Chef Workstation](https://docs.chef.io/workstation.html) - Knife, chef-repo, Chef DK etc by official chef.io.
* [Chef Server](https://docs.chef.io/chef_server.html) - Chef server components.
* [Chef Node](https://docs.chef.io/nodes.html) - How chef-client runs, run-list, node names, etc.
* [Cookbook](https://docs.chef.io/cookbooks.html) - What is a cookbook and its components (metadata, recipe, resource, attributes, templates, etc).
* [Attribute](https://docs.chef.io/attributes.html) - attibutes defined by type (default, normal, automatic), by useage (node, role, environment).
* [Resource](https://docs.chef.io/resources.html) - Chef resource which is a building block of a recipe.
* [Data Bag](https://docs.chef.io/data_bags.html) - Data bag and its usage.


## Cookbooks

> A cookbook is the fundamental unit of configuration and policy distribution in Chef. Each cookbook defines a scenario, such as everything needed to install and configure MySQL, and then it contains all of the components that are required to support that scenario. Chef maintains a collection of cookbooks that are important to Chef and are widely used by the Chef community. - [What is a cookbook?](https://supermarket.chef.io/cookbooks-directory)

### Docker
* [docker](https://github.com/chef-cookbooks/docker)

### Ruby
* [chruby](https://github.com/ichilton/chef_chruby_install)
* [rbenv](https://github.com/RiotGamesCookbooks/rbenv-cookbook) - configure [rbenv](https://github.com/rbenv/rbenv).
* [ruby_build](https://github.com/fnichol/chef-ruby_build)
* [rvm](https://github.com/martinisoft/chef-rvm)
* [unicorn](https://github.com/chef-cookbooks/unicorn) - Deprecated
* [xml::ruby](https://github.com/chef-cookbooks/xml#ruby) - Installs the nokogiri gem into Chef's Ruby environment.

### Java
* [java](https://github.com/agileorbit-cookbooks/java)
* [maven](https://github.com/chef-cookbooks/maven)
* [tomcat](https://github.com/chef-cookbooks/tomcat)
* [weblogic](https://github.com/universityofderby/chef-weblogic)

### PHP
* [composer](https://github.com/escapestudios-cookbooks/composer)
* [php](https://github.com/chef-cookbooks/php)

### Language Runtimes
* [erlang](https://github.com/chef-cookbooks/erlang)
* [nodejs](https://github.com/redguide/nodejs)
* [perl](https://github.com/chef-cookbooks/perl)
* [python](https://github.com/poise/python)

### Web Server
* [apache2](https://github.com/svanzoest-cookbooks/apache2) - Apache HTTP server v2.x.
* [nginx](https://github.com/miketheman/nginx)
* [passenger_apache2](https://github.com/chef-cookbooks/passenger_apache2) - [Passenger](https://www.phusionpassenger.com/library) for Apache2.

### Database
* [couchdb](https://github.com/wohali/couchdb-cookbook)
* [hadoop](https://github.com/caskdata/hadoop_cookbook) - Hadoop 2.0+.
* [mariadb](https://github.com/sinfomicien/mariadb)
* [mongodb](https://github.com/edelight/chef-mongodb)
* [mysql](https://github.com/chef-cookbooks/mysql)
* [percona](https://github.com/phlipper/chef-percona) - [Percona XtraDB Cluster](https://www.percona.com/software/mysql-database/percona-xtradb-cluster) and other components.
* [oracle](https://github.com/aririikonen/oracle)
* [postgresql](https://github.com/hw-cookbooks/postgresql)
* [redis](https://github.com/brianbianco/redisio)
* [riak](https://github.com/basho-labs/riak-chef-cookbook) - [Riak](http://basho.com/products/)

### Loadbalancer, Cache, Proxy and Message Queue
* [activemq](https://github.com/chef-cookbooks/activemq) - [ActiveMQ](http://activemq.apache.org/)
* [haproxy](https://github.com/hw-cookbooks/haproxy)
* [memcached](https://github.com/chef-cookbooks/memcached)
* [rabbitmq](https://github.com/jjasghar/rabbitmq)
* [varnish](https://github.com/rackspace-cookbooks/varnish)

### Web Applications
* [elasticsearch](https://github.com/elastic/cookbook-elasticsearch)
* [elkstack](https://github.com/rackspace-cookbooks/elkstack) - [ELK stack](https://www.elastic.co/webinars/introduction-elk-stack) Combine Elasticsearch, Logstash and Kibana.
* [gitlab](https://github.com/atomic-penguin/cookbook-gitlab)
* [jenkins](https://github.com/chef-cookbooks/jenkins)
* [postfix](https://github.com/chef-cookbooks/postfix)
* [wordpress](https://github.com/brint/wordpress-cookbook)

### Building/Installing Software
* [build-essential](https://github.com/chef-cookbooks/build-essential) - gcc, make, autoconf, bison, gettext etc.
* [git](https://github.com/chef-cookbooks/git)
* [xml](https://github.com/chef-cookbooks/xml) - Installs development package for [libxml](http://xmlsoft.org/).

### Service Discovery
* [consul](https://github.com/johnbellone/consul-cookbook) - [Hashicorp Consul](https://www.consul.io/)
* [consul-template](https://github.com/adamkrone/chef-consul-template)
* [etcd](https://github.com/chef-cookbooks/etcd) - [etcd](https://coreos.com/etcd/) is a distributed key value store that provides a reliable way to store data across a cluster of machines. 
* [zookeeper](https://github.com/SimpleFinance/chef-zookeeper) - [Apache Zookeeper](https://zookeeper.apache.org/)

### Logging/Monitoring
* [collectd](https://github.com/hectcastro/chef-collectd.git) - [Collectd](http://collectd.org)
* [datadog](https://github.com/DataDog/chef-datadog) - [DataDog](https://www.datadoghq.com/)
* [fail2ban](https://github.com/chef-cookbooks/fail2ban) - [Fail2ban](http://www.fail2ban.org/wiki/index.php/Main_Page)
* [grafana](https://github.com/dzautner/grafana-cookbook) - [Grafana](http://grafana.org/) (A Graphite Dashboard and Graph Editor)
* [graphite](https://github.com/hw-cookbooks/graphite) - [Graphite](http://graphite.wikidot.com/)
* [graphitus](https://github.com/kisoku/graphitus-chef) - [Graphitus](https://github.com/ezbz/graphitus)
* [graylog](https://github.com/Graylog2/graylog2-cookbook) - [Graylog](https://www.graylog.org/)
* [icinga](https://github.com/Bigpoint/icinga) - [Icinga](https://www.icinga.org/)/[CheckMK](https://mathias-kettner.de/check_mk.html)
* [kibana](https://github.com/realityforge/chef-kibana) - [Kibana](https://www.elastic.co/products/kibana)
* [logrotate](https://github.com/stevendanna/logrotate)
* [logstash](https://github.com/lusis/chef-logstash)
* [nagios](https://github.com/schubergphilis/nagios)
* [newrelic](https://github.com/escapestudios-cookbooks/newrelic)
* [newrelic_plugins](https://github.com/newrelic-platform/newrelic_plugins_chef)
* [munin](https://github.com/jesseadams/munin) - [Munin](http://munin-monitoring.org/)
* [monit](https://github.com/phlipper/chef-monit) - [Monit](https://mmonit.com/monit/)
* [rsyslog](https://github.com/chef-cookbooks/rsyslog)
* [sensu](https://github.com/sensu/sensu-chef) - [Sensu](https://sensuapp.org/)
* [splunk](https://github.com/BestBuy/splunk_cookbook) - [Splunk](http://www.splunk.com/)
* [zabbix](https://github.com/laradji/zabbix) - [Zabbix](http://www.zabbix.com/)

### Network/Security
* [iptables](https://github.com/chef-cookbooks/iptables)
* [ntp](https://github.com/gmiranda23/ntp)
* [openldap](https://github.com/chef-cookbooks/openldap)
* [openssh](https://github.com/chef-cookbooks/openssh)
* [openvpn](https://github.com/xhost-cookbooks/openvpn) 
* [resolver](https://github.com/chef-cookbooks/resolver) - Configures ```/etc/resolv.conf``` via attributes.
* [ssh-key](https://github.com/nickola/chef-ssh-keys) - Creates ```authorized_keys``` in user ```~/.ssh``` directory from a data bag (encrypted data bag supported).

### File System/Storage
* [ceph_cephfs](https://github.com/ceph/ceph-chef#ceph_cephfs)
* [nfs](https://github.com/atomic-penguin/cookbook-nfs)

## Resources
When you write wrapper cookbooks, use following resources. The list includes both Chef's built in resources and LWRP of community/open source cookbooks.

### Commands/Scripts
* [cron](https://docs.chef.io/resource_cron.html) - Chef builtin resource.
* [cron_d](https://github.com/chef-cookbooks/cron#cron_d) - LWRP to manage files in ```/etc/cron.d```
* [execute](https://docs.chef.io/resource_execute.html) - Chef builtin resource.
* [magic_shell_alias, magic_shell_environment](https://github.com/customink-webops/magic_shell#usage) - Create a command alias or shell environment variable.
* [script](https://docs.chef.io/resource_script.html) - Chef builtin resource.

### Files/Directories
* [ark](https://github.com/burtlo/ark#resources) - extract/build/configure.
* [cookbook_file](https://docs.chef.io/resource_cookbook_file.html) - Chef builtin resource.
* [directory](https://docs.chef.io/resource_directory.html) - Chef builtin resource.
* [file](https://docs.chef.io/resource_file.html) - Chef builtin resource.
* [link](https://docs.chef.io/resource_link.html) - Chef builtin resource.
* [remote_file](https://docs.chef.io/resource_remote_file.html) - Chef builtin resource.
* [rsync_serve](https://github.com/chef-cookbooks/rsync#resourcesproviders) - rsync server module.
* [s3_file](https://github.com/adamsb6/s3_file/#usage) - fetch files from AWS S3.
* [template](https://docs.chef.io/resource_template.html) - Chef builtin resource.
* [append_if_no_line, replace_or_add, delete_lines, add_to_list, delete_from_list](https://github.com/someara/line-cookbook#usage) - Edit lines in a file rather than replacing whole file.

### User Management/Authorization
* [group](https://docs.chef.io/resource_group.html) - Chef builtin resource.
* [user_ulimit](https://github.com/bmhatfield/chef-ulimit#usage) - [User limits](http://ss64.com/bash/ulimit.html) 
* [user](https://docs.chef.io/resource_user.html) - Chef builtin resource, manage user.
* [users_manage](https://github.com/chef-cookbooks/users#users_manage) - manage user using data bag search.
* [sudo](https://github.com/chef-cookbooks/sudo#lwrp)

### Security
* [certificate_manage](https://github.com/atomic-penguin/cookbook-certificate#resourcesproviders) - Manages x509 certificates and keys from encrypted Data Bags.
* [firewall](https://github.com/chef-cookbooks/firewall#firewall)
* [firewall_rule](https://github.com/chef-cookbooks/firewall#firewall_rule)
* [letsencrypt_certificate](https://github.com/schubergphilis/letsencrypt#usage) - Automatically get/renew free and trusted certificates from [Let's Encrypt](https://letsencrypt.org).
* [random_password](https://github.com/chef-cookbooks/openssl#random_password-opensslcookbookrandompassword) - useing openssl.
* [openssl_dhparam](https://github.com/chef-cookbooks/openssl#openssl_dhparam)
* [openssl_rsa_key](https://github.com/chef-cookbooks/openssl#openssl_rsa_key)
* [openssl_x509](https://github.com/chef-cookbooks/openssl#openssl_x509) - Generates self-signed, PEM-formatted x509 certificates.
* [selinux_state](https://github.com/skottler/selinux#selinux_state)
* [simple_iptables_rule](https://github.com/rtkwlf/cookbook-simple-iptables#simple_iptables_rule-resource)
* [ssh_known_hosts_entry](https://github.com/chef-cookbooks/ssh_known_hosts#lwrp)

### Deployment
* [git](https://docs.chef.io/resource_git.html) - Chef builtin resource.
* [deploy](https://docs.chef.io/resource_deploy.html) - Chef builtin resource.
* [application](https://github.com/poise/application)
* [application_git](https://github.com/poise/application_git)
* [application_javascript](https://github.com/poise/application_javascript)
* [application_nodejs](https://github.com/mburns/application_nodejs)
* [application_php](https://github.com/poise/application_php)
* [application_python](https://github.com/poise/application_python)
* [application_ruby](https://github.com/poise/application_ruby)

### Apache HTTP Server Config
* [php_fpm_pool](https://github.com/chef-cookbooks/php#php_fpm_pool)
* [web_app](https://github.com/svanzoest-cookbooks/apache2#web_app) - setup Apache HTTP server v2.x virtual host.

### Database Config/Management
* [database, mysql_database, postgresql_database](https://github.com/chef-cookbooks/database#examples)
* [flywaydb](https://github.com/dhoer/chef-flywaydb#examples)

### Packages/Package Repositories
* [package](https://docs.chef.io/resource_package.html) - Chef builtin resource.
* [apt_repository](https://github.com/chef-cookbooks/apt#resourcesproviders)
* [yum_repository](https://github.com/chef-cookbooks/yum#yum_repository)

### Service Management/Init System
* [runit_service](https://github.com/hw-cookbooks/runit#resourceprovider) - Configure [runit](http://smarden.org/runit/).
* [service](https://docs.chef.io/resource_service.html) - Chef builtin resource.
* [supervisor_service](https://github.com/poise/supervisor#resourcesproviders) - [(Python) supervisor](http://supervisord.org/).

### Operating System Configuration
* [hostsfile_entry](https://github.com/customink-webops/hostsfile#hostsfile-lwrp) - /etc/hosts file.
* [mount](https://docs.chef.io/resource_mount.html) - Chef builtin resource.
* [lvm_physical_volume](https://github.com/chef-cookbooks/lvm#lvm_physical_volume)
* [lvm_logical_volume](https://github.com/chef-cookbooks/lvm#lvm_logical_volume)
* [route](https://docs.chef.io/resource_route.html) - Chef builtin resource, manage system's routing table.
* [sysctl_param](https://github.com/svanzoest-cookbooks/sysctl/#using-lwrps) - set the kernel parameter.
* [vim](https://github.com/chef-cookbooks/vim)
* [zsh](https://github.com/chef-cookbooks/zsh)

## Chef for Windows
List of cookbooks and resources which supports windows.

### Application Cookbooks - Language Runtime
* [java](https://github.com/agileorbit-cookbooks/java)
* [php](https://github.com/chef-cookbooks/php)

### Application Cookbooks - Software
* [iis](https://supermarket.chef.io/cookbooks/iis) - Microsoft Internet Information Services.
* [sql_server](https://github.com/chef-cookbooks/sql_server) - Microsoft SQL Server 2008 R2 and Microsoft SQL Server 2012 server and client. 
* [7-zip](https://github.com/sneal/7-zip)

### Resources - Files/Directories
* [cookbook_file](https://docs.chef.io/resource_cookbook_file.html) - Chef builtin resource.
* [directory](https://docs.chef.io/resource_directory.html) - Chef builtin resource.
* [file](https://docs.chef.io/resource_file.html) - Chef builtin resource.
* [link](https://docs.chef.io/resource_link.html) - Chef builtin resource.
* [mount](https://docs.chef.io/resource_mount.html) - Chef builtin resource.
* [remote_file](https://docs.chef.io/resource_remote_file.html) - Chef builtin resource.
* [template](https://docs.chef.io/resource_template.html) - Chef builtin resource.

### Resources - Command Execution / Launching Software
* [batch](https://docs.chef.io/resource_batch.html) - Chef builtin resource, manage batch script.
* [windows_auto_run](https://github.com/chef-cookbooks/windows#windows_auto_run) - Configure an software to run at login.

### Resources - Package/Software Installation
* [chocolatey_package](https://docs.chef.io/resource_chocolatey_package.html) - Chef builtin resource. Manage packages using. [Chocolatey](https://chocolatey.org/) windows package management system.
* [env](https://docs.chef.io/resource_env.html) - Chef builtin resource, manage environment keys in Microsoft Windows.
* [powershell](https://github.com/chef-cookbooks/powershell)
* [reboot](https://docs.chef.io/resource_reboot.html) - Chef builtin resource.
* [windows_feature](https://github.com/chef-cookbooks/windows#windows_feature)
* [windows_package](https://docs.chef.io/resource_windows_package.html) - Chef builtin resource.

### Resources - OS configuration
* [user](https://docs.chef.io/resource_user.html) - Chef builtin resource, Windows compatible
* [windows_certificate](https://github.com/chef-cookbooks/windows#windows_certificate) - Installs a certificate into the Windows certificate store from a file.
* [windows_path](https://github.com/chef-cookbooks/windows#windows_path)
* [registry_key](https://docs.chef.io/resource_registry_key.html)
* [windows_registry](https://github.com/chef-cookbooks/windows#windows_registry)
* [windows_service](https://docs.chef.io/resource_windows_service.html) - Chef builtin resource.
* [windows_task](https://github.com/chef-cookbooks/windows#windows_task)

### Resources - Application configuration
* [sql_server_database](https://github.com/chef-cookbooks/database#examples)

## Chef handlers

> A handler is used to identify situations that may arise during a chef-client run, and to then instruct the chef-client how to handle these situations, should they occur. — [Handlers](https://docs.chef.io/handlers.html)

* [About Handlers](https://docs.chef.io/handlers.html) - Official reference page
* [Supermarket](https://supermarket.chef.io/tools?q=handler) - Handlers registered in [Supermarket](https://supermarket.chef.io/).
* [Chef Elapsed Time Handler](https://supermarket.chef.io/tools/20-chef-elapsed-time-handler) - A chef handler that reports on per-resource elapsed times in a simple graphical form.
* [Chef Datadog Handler](https://supermarket.chef.io/tools/chef-handler-datadog) - Get Chef stats directly into Datadog. Add the gem as an execution and report handler to your Chef run.
* [Chef SNS Handler](https://github.com/onddo/chef-handler-sns) - Chef report handler to send Amazon SNS notifications on failures or changes, includes IAM roles support.
* [Chef Users Handler](https://supermarket.chef.io/tools/chef-handler-users) - A dead simple Chef handler to report changes in users. Can send emails using the Pony gem.
* [Chef Zookeeper Handler](https://supermarket.chef.io/tools/chef-handler-zookeeper) - A simple Chef report handler to send notifications to ZooKeeper about Chef runs.
* [Chef Airbrake Handler](https://github.com/morgoth/airbrake_handler) - Chef handler for sending exceptions to Airbrake.
* [Chef Zabbix Handler](https://github.com/TYPO3-cookbooks/zabbix-custom-checks/blob/master/templates/chef-client/chef-client-handler.rb) - Send chef-client statistics to zabbix using a report handler.
* [Chef Campfire Handler](https://github.com/jjasghar/chef-handler-campfire) - Chef Exception & Reporting Handler for Campfire
* [Chef Cookbook Version Handler](https://github.com/juliandunn/cookbook_versions_handler) - This cookbook installs a Chef report handler to log the cookbooks and versions run on the node as part of the Chef run.
* [Chef Flowdock Handler](https://github.com/mmarschall/chef-handler-flowdock) - A Chef handler that collects exception and report handler data and reports it to Flowdock, a web-based team inbox and chat tool.
* [Chef Graphite Handler](https://github.com/imeyer/chef-handler-graphite) - Simple handler to send data to Graphite about your node's Chef runs, including elapsed time, total number of resources, number of resources updated, and success or failure.
* [Chef Graylog2/Gelf Handler](https://github.com/jellybob/chef-gelf/) - A Chef handler that reports to Graylog2 servers.
* [Chef Growl Handler](https://github.com/jtimberman/chef-handler-growl) - A simple Chef report handler using ruby_gntp to send growl notifications.
* [Chef HipChat Handler](https://github.com/mojotech/hipchat/blob/master/lib/hipchat/chef.rb) - A handler that collects exception and report handler data and then sends it as a Growl notification.
* [Chef IRC Snitch Handler](https://github.com/portertech/chef-irc-snitch) - An exception handler for OpsCode Chef runs, GitHub Gist & IRC.
* [Chef Librato Handler](https://github.com/bscott/chef-handler-librato) - A handler that sends Chef run metrics to Librato.
* [Chef Mail Handler](https://github.com/kisoku/chef-handler-mail) - A simple chef report handler that uses the Pony gem to send email reports generated from an Erubis template.
* [Chef Splunk Storm Handler](https://github.com/ampledata/chef-handler-splunkstorm) - A Chef Exception & Reporting Handler for Splunk Storm.
* [Chef Syslog Handler](https://github.com/jblaine/syslog_handler) - Syslog report and error handler for Chef.
* [Chef Updated Resources Handler](https://github.com/jtimberman/chef-handler-updated-resources) - Simple Report Handler of Updated Resources.

## Add-ons

* [Chef Rewind](https://github.com/bryanwb/chef-rewind) - Monkeypatch chef to edit existing resources in place.
* [Chef Sugar](https://github.com/sethvargo/chef-sugar) - Chef Sugar is a Gem & Chef Recipe that includes series of helpful sugar of the Chef core and other resources to make a cleaner, more lean recipe DSL, enforce DRY principles, and make writing Chef recipes an awesome experience!
* [Knife Spork](https://github.com/jonlives/knife-spork) - A workflow plugin to help many devs work with cookbooks and environments at once.
* [Knife Flip](https://github.com/jonlives/knife-flip) - A knife plugin to quickly move a node between environments.
* [Chef Whitelist](https://github.com/etsy/chef-whitelist) - Simple library to enable host based rollouts of changes.
* [Poise Appenv](https://github.com/poise/poise-appenv) - Helpers for application-specific envronment settings in Chef.
* [Chef-Guard](https://github.com/xanzy/chef-guard) - An add-on that protects your Chef server from untested and uncommitted (i.e. potentially dangerous) cookbooks.


## Podcasts

### Chef podcast

* [Food Fight Show](http://foodfightshow.org/) - The Podcast where DevOps chefs do battle.

### DevOps podcast

* [DevOps Cafe Podcast](http://devopscafe.org/) -
* [Ops All The Things!](http://www.opsallthethings.com/) - A Podcast about all things Operations, DevOps and Systems Administration.
* [Arrested DevOps](http://www.arresteddevops.com/) - There's always DevOps in the banana stand.

## Books

* [Chef Infrastructure Automation Cookbook](https://www.packtpub.com/networking-and-servers/chef-infrastructure-automation-cookbook) - For systems administrators and developers this book could revolutionize your cloud and server infrastructure through automation. Packed with real world situations and practical recipes, it’s a dazzling insight into Chef.
* [Customizing Chef](http://shop.oreilly.com/product/0636920032984.do) - Getting the Most Out of Your Infrastructure Automation. Take advantage of Chef’s highly customizable design to tackle specific automation issues that you can’t solve by simply using Chef’s tools, resources, and services out of the box.
* [Learning Chef](http://shop.oreilly.com/product/0636920032397.do) - A Guide to Configuration Management and Automation.
* [Test-Driven Infrastructure with Chef](http://shop.oreilly.com/product/0636920020042.do) - Bring behaviour-driven development to infrastructure as code.
* [Test-Driven Infrastructure with Chef, 2nd Edition](http://shop.oreilly.com/product/0636920030973.do) - Bring Behavior-Driven Development to Infrastructure as Code.
* [Managing Windows Servers with Chef](https://www.packtpub.com/networking-and-servers/managing-windows-servers-chef) - Harness the power of Chef to automate management of Windows-based systems using hands-on examples.
* [The chef-book](https://github.com/jjasghar/chef-book) - People Keep Asking Me How to Start With Chef.
* [Getting started with Chef](http://gettingstartedwithchef.com/) - Learn how to configure, manage and provision cloud servers with Chef by following practical examples with real world applications.

## Newsletters

* [UsingChef Newsletter](http://usingchef.com/) - This newsletter is intended for the Chef practitioner who uses Chef every day and wants to learn something new, make their lives easier, and stay up to date.

## Articles

* [Secrets Management and Chef](https://coderanger.net/chef-secrets/) - Everyone has secrets. Database passwords, API credentials, recovery questions. These secrets need to be stored somewhere, and then made available to servers that use them.
* [How to Write Reusable Chef Cookbooks, Gangnam Style](http://devopsanywhere.blogspot.fr/2012/11/how-to-write-reusable-chef-cookbooks.html) -

# Contribution Guidelines

Please ensure your pull request adheres to the following guidelines:

* Please search previous suggestions before making a new one, as yours may be a duplicate.
* Please make an individual pull request for each suggestion.
* Use the following format: \[RESOURCE\]\(LINK\) - DESCRIPTION.
* Keep descriptions short and simple.
* End all descriptions with a full stop/period.
* Check your spelling and grammar.
* New categories, or improvements to the existing categorisation are welcome.

Thank you for your suggestions!
