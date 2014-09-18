# Awesome Chef

> [Chef](http://getchef.com) is a systems and cloud infrastructure automation framework that makes it easy to deploy servers and applications to any physical, virtual, or cloud location, no matter the size of the infrastructure.. — [Chef](http://docs.getchef.com/)

--
A curated list of amazingly awesome open source Chef resources.

* [Awesome Chef](#awesome-chef)
  * [Cookbooks](#Cookbooks)
  * [Podcasts](#podcasts)
  * [Chef handlers](#chef-handlers)
  * [Add-ons](#add-ons)


## Cookbooks

> A cookbook is the fundamental unit of configuration and policy distribution in Chef. Each cookbook defines a scenario, such as everything needed to install and configure MySQL, and then it contains all of the components that are required to support that scenario. Chef maintains a collection of cookbooks that are important to Chef and are widely used by the Chef community. - [What is a cookbook?](https://supermarket.getchef.com/cookbooks-directory)


### Official and community Cookbooks

* [Supermarket](https://supermarket.getchef.com/cookbooks-directory) - Find, explore and view Chef cookbooks for all of your ops needs.

### Others (or alternative) Cookbooks

* [Collectd cookbook](https://github.com/hectcastro/chef-collectd.git) - A Chef cookbook to install [Collectd](http://collectd.org).
* [Graphitus cookbook](https://github.com/kisoku/graphitus-chef) - Chef cookbooks for [Graphitus](https://github.com/ezbz/graphitus)
* [Grafana cookbook](https://github.com/dzautner/grafana-cookbook) - A chef cookbook for [Grafana](http://grafana.org/) (A Graphite Dashboard and Graph Editor)
* [Icinga/Check MK cookbook](https://github.com/Bigpoint/icinga) - Chef cookbook for [Icinga](https://www.icinga.org/)/[CheckMK](https://mathias-kettner.de/check_mk.html)

## Podcasts

### Chef podcast

* [Food Fight Show](http://foodfightshow.org/) - The Podcast where DevOps chefs do battle

### DevOps podcast

* [DevOps Cafe Podcast](http://devopscafe.org/) - 
* [Ops All The Things!](http://www.opsallthethings.com/) - A Podcast about all things Operations, DevOps and Systems Administration
* [Arrested DevOps](http://www.arresteddevops.com/) - There's always DevOps in the banana stand

## Chef handlers

> A handler is used to identify situations that may arise during a chef-client run, and to then instruct the chef-client how to handle these situations, should they occur. — [Handlers](https://docs.getchef.com/handlers.html)

* [About Handlers](https://docs.getchef.com/handlers.html) - Official reference page
* [Supermarket](https://supermarket.getchef.com/tools?utf8=%E2%9C%93&q=handler) - Handlers registered in [Supermarket](https://supermarket.getchef.com/).
* [Chef Elapsed Time Handler](https://supermarket.getchef.com/tools/20-chef-elapsed-time-handler) - A chef handler that reports on per-resource elapsed times in a simple graphical form.
* [Chef Datadog Handler](https://supermarket.getchef.com/tools/chef-handler-datadog) - Get Chef stats directly into Datadog. Add the gem as an execution and report handler to your Chef run.
* [Chef SNS Handler](https://github.com/onddo/chef-handler-sns) - Chef report handler to send Amazon SNS notifications on failures or changes, includes IAM roles support.
* [Chef Users Handler](https://supermarket.getchef.com/tools/chef-handler-users) - A dead simple Chef handler to report changes in users. Can send emails using the Pony gem.
* [Chef Zookeeper Handler](https://supermarket.getchef.com/tools/chef-handler-zookeeper) - A simple Chef report handler to send notifications to ZooKeeper about Chef runs.
* [Chef Airbrake Handler](https://github.com/morgoth/airbrake_handler) - Chef handler for sending exceptions to Airbrake.
* [Chef Zabbix Handler](https://github.com/TYPO3-cookbooks/zabbix-custom-checks/blob/master/templates/default/chef-client/chef-client-handler.rb) - Send chef-client statistics to zabbix using a report handler
* [Chef Campfire Handler](https://github.com/jjasghar/chef-handler-campfire) - Chef Exception & Reporting Handler for Campfire
* [Chef Cookbook Version Handler](https://github.com/juliandunn/cookbook_versions_handler) - This cookbook installs a Chef report handler to log the cookbooks and versions run on the node as part of the Chef run.
* [Chef Flowdock Handler](https://github.com/mmarschall/chef-handler-flowdock) - A Chef handler that collects exception and report handler data and reports it to Flowdock, a web-based team inbox and chat tool.
* [Chef Graphite Handler](https://github.com/imeyer/chef-handler-graphite) - Simple handler to send data to Graphite about your node's Chef runs, including elapsed time, total number of resources, number of resources updated, and success or failure.
* [Chef Graylog2/Gelf Handler](https://github.com/jellybob/chef-gelf/) - A Chef handler that reports to Graylog2 servers.
* [Chef Growl Handler](https://github.com/jtimberman/chef-handler-growl) - A simple Chef report handler using ruby_gntp to send growl notifications
* [Chef HipChat Handler](https://github.com/mojotech/hipchat/blob/master/lib/hipchat/chef.rb) - A handler that collects exception and report handler data and then sends it as a Growl notification.
* [Chef IRC Snitch Handler](https://github.com/portertech/chef-irc-snitch) - An exception handler for OpsCode Chef runs, GitHub Gist & IRC.
* [Chef Mail Handler](https://github.com/kisoku/chef-handler-mail) - A simple chef report handler that uses the Pony gem to send email reports generated from an Erubis template.
* [Chef Splunk Storm Handler](https://github.com/ampledata/chef-handler-splunkstorm) - A Chef Exception & Reporting Handler for Splunk Storm
* [Chef Syslog Handler](https://github.com/jblaine/syslog_handler) - Syslog report and error handler for Chef.
* [Chef Updated Resources Handler](https://github.com/jtimberman/chef-handler-updated-resources) - Simple Report Handler of Updated Resources.

## Add-ons

* [Chef Rewind](https://github.com/bryanwb/chef-rewind) - Monkeypatch chef to edit existing resources in place
* [Chef Sugar](https://github.com/sethvargo/chef-sugar) - Chef Sugar is a Gem & Chef Recipe that includes series of helpful sugar of the Chef core and other resources to make a cleaner, more lean recipe DSL, enforce DRY principles, and make writing Chef recipes an awesome experience!
