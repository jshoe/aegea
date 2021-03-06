Changes for v2.2.1 (2018-05-07)
===============================

-  Fix logic bug in aegea ssh username discovery

-  aegea build-ami: Ubuntu 18.04 compatibility

Changes for v2.2.0 (2018-05-03)
===============================

-  Get correct IAM username for cross-account SSH

-  Bump dependencies

Changes for v2.1.9 (2018-04-13)
===============================

-  Bump deps

Changes for v2.1.8 (2018-04-12)
===============================

-  Fixups for aegea deploy

Changes for v2.1.7 (2018-04-12)
===============================

-  Buildbox usability updates

Changes for v2.1.6 (2018-04-11)
===============================

-  Fix Python compat issue in key_fingerprint

Changes for v2.1.5 (2018-04-11)
===============================

-  Fix queue naming in aegea-deploy-pilot

Changes for v2.1.4 (2018-04-10)
===============================

-  Continue secrets migration

-  Fix splitting of deploy systemd unit names

Changes for v2.1.3 (2018-04-10)
===============================

-  Begin switching aegea secrets to secretsmanager

-  Add Lambda listing parsers

-  Bump deps and add common deps per @cschin request

-  Fix permissions in cloudinit rootfs.skel input

-  Accommodate IAM eventual consistency in instance profiles

Changes for v2.1.2 (2018-04-05)
===============================

-  Bump dependencies

Changes for v2.1.1 (2018-03-26)
===============================

-  Bump pip ami build dependencies

-  Add aegea scp

Changes for v2.1.0 (2017-12-20)
===============================

-  Beautify batch shellcode

-  aegea launch: add support for EBS volumes via --storage

-  aegea --log-level: Remove unneeded NOTSET level

-  Expand documentation

Changes for v2.0.9 (2017-11-21)
===============================

-  Fix version generation

Changes for v2.0.8 (2017-11-21)
===============================

-  aegea batch submit: Use S3 to stage execute payload

-  Enable newline formatting and excise comments in ebs shellcode

-  kill processes using the filesystem before unmounting (#34)

Changes for v2.0.7 (2017-11-20)
===============================

-  aegea batch watch: fix logic error when job fails before starting

Changes for v2.0.6 (2017-11-20)
===============================

-  Disable custom Batch AMIs by default

Changes for v2.0.5 (2017-11-20)
===============================

-  Make sure version is updated when rolling release

Changes for v2.0.4 (2017-11-20)
===============================

-  Fix broken release

Changes for v2.0.3 (2017-11-19)
===============================

-  Bump tweak dependency with upstream fix

Changes for v2.0.2 (2017-11-17)
===============================

-  Undo changes that had to do with tweak breakage

-  fix another typo that was breaking job launch (#33)

Changes for v2.0.1 (2017-11-16)
===============================

-  fix batch: newlines and percent characters have special meaning (#32)

Changes for v2.0.0 (2017-11-15)
===============================

-  Further ameliorate the volume attach/detach polling issues (#31)

-  Limit time we wait for aws detach to succeed before deleting volume
   (#30)

-  Make exception catching more specific

Changes for v1.0.1 (2017-09-15)
===============================

Fix for batch API breaking changes (#25)

Changes for v1.10.0 (2017-09-11)
================================

-  Set default nofile to 100000; lint fixes

-  aegea batch submit: Add ability to specify ulimits nofile to
   conatiner and also adding sensible default (#24)

-  Change aegea-deploy service to serve as template, add custom make
   targets, using one queue per (org, name, branch, instanceid)

-  Add iam-role argument to build

Changes for v1.9.18 (2017-08-16)
================================

-  aegea batch watch: Do not crash if log stream does not exist yet

Changes for v1.9.17 (2017-06-15)
================================

Merge pull request #22 from wholebiome/build-timeout Extend timeout for
AMI builds Added timeout to loop, default much longer Fix tests

Changes for v1.9.16 (2017-06-01)
================================

-  Add file missed in 0c99863

Changes for v1.9.15 (2017-06-01)
================================

-  Fix logic error in parameter naming

Changes for v1.9.14 (2017-05-29)
================================

-  Temporarily disable batch custom AMI

Changes for v1.9.13 (2017-05-29)
================================

-  Minor refactor in batch

-  Ensure default selection of batch instances has instance storage

-  Begin aegea lambda ls, aegea rm --lambda

-  Tab complete log levels

-  Avoid using pkgutil for introspection

Changes for v1.9.12 (2017-05-14)
================================

-  Batch bug fixes and begin support for custom Batch ECI AMIs

Changes for v1.8.4 (2017-02-02)
===============================

-  Install process robustness improvements

-  Install documentation improvements

Changes for v1.8.3 (2017-02-01)
===============================

-  Don't symlink aegea in bin to avoid pip uninstall bugs

Changes for v1.8.2 (2017-02-01)
===============================

-  Resume interrupted release

Changes for v1.8.1 (2017-02-01)
===============================

-  Resume interrupted release

Changes for v1.8.0 (2017-02-01)
===============================

-  Installation documentation and robustness improvements

-  Batch API and mission-specific improvements

Changes for v1.7.4 (2017-01-26)
===============================

-  aegea batch: automatic setup of builder IAM policies

-  aegea batch submit --job-role: automatic setup of job IAM roles

-  aegea batch submit --storage: EBS volume manager

-  Autocomplete column titles in listing subcommands where a resource is
   available

-  Autoconfigure a VPC if all VPCs including the default VPC were
   deleted

-  Asset loader: offload rootfs.skel to S3 when user-data exceeds 16K
   limit

-  Arvados updates

-  Make missions dir doc link relative (#9)

-  Display statusReason in aegea batch ls and aegea batch watch

Changes for v1.7.3 (2017-01-18)
===============================

-  Add automatic configuration for route53 private DNS

-  Various improvements to aegea batch

-  Work around autoloader import issue seen on some Python 2.7 versions

-  aegea build\_ami: improve progress and error messages

Changes for v1.7.2 (2017-01-13)
===============================

-  Fix makefile shell assumption

-  Batch WIP

Changes for v1.7.1 (2017-01-13)
===============================

-  Test and release infra improvements

-  Batch docs

Changes for v1.7.0 (2017-01-10)
===============================

-  aegea-build-image-for-mission now builds ECR images by default

-  Integration work for Batch

Changes for v1.6.3 (2017-01-08)
===============================

-  Add ELB SG configurator, aegea-rebuild-public-elb-sg

-  Add awscli to deps

Changes for v1.6.2 (2017-01-06)
===============================

-  ELB deploy: set default target group name properly

-  Make sure wheel is installed before attempting setup

-  Aegea batch submit: Begin CWL support

-  Aegea batch watch: amend log line dup fix

Changes for v1.6.1 (2017-01-03)
===============================

-  Improvements to aegea batch

Changes for v1.6.0 (2016-12-30)
===============================

-  Aegea EFS refactor

-  Aegea batch

-  Add IP Ranges API

-  Add aegea buckets cors placeholder

-  Aegea bucket lifecycle

-  Test and release infrastructure improvements

Changes for v1.5.1 (2016-11-14)
===============================

-  Fogdog mission: add environment placeholder

-  Begin timestamp backport

-  Propagate base AMI metadata in build\_image

Changes for v1.5.0 (2016-11-10)
===============================

-  Implement aegea rds snapshot

-  Only use pager with pretty-printed tables

-  Add Amazon Linux AMI locator

-  Use -w0 for auto col width table formatter

-  aegea zones update: support multiple updates

-  Cosmetic and documentation fixes

Changes for v1.4.0 (2016-11-02)
===============================

-  aegea-build-ami-for-mission: skip make if no Makefile
-  Begin FogDog mission
-  Arvados config support; improve config file handling
-  Don't fail cloud-init on account of expected ssh failure
-  Run ssh-add from aegea launch
-  aegea elb create bugfix
-  Fix ELB behavior when TG is present
-  Simplify arg forwarding in build\_ami

Changes for v1.3.0 (2016-10-20)
===============================

-  Support running core aegea on Ubuntu 14.04 vendored Python

-  Improve freeform cloud-config-data passing

-  Fix pager; introduce --auto-col-width table formatter

-  List security groups in elb listing

-  Break out and begin buildout of aegea ebs subcommand

-  Begin improving rds listings

-  Improve DNS zone repr

-  New protocol to check out local tracking branch in aegea deploy

-  aegea elb create: configurable health check path

-  Key cloud-init files manifest by file path to avoid duplicates

Changes for v1.2.2 (2016-10-08)
===============================

-  ELB provisioning and listing improvements

Changes for v1.2.1 (2016-10-07)
===============================

-  Aegea deploy fixups

Changes for v1.2.0 (2016-10-05)
===============================

-  Online documentation improvements

-  aegea zones: begin ability to edit records from command line

-  Begin support for recursive git clone deploy keys (#4)

-  Pretty-print dicts and lists as json in tables

-  Logic fixes in elb create command

Changes for v1.1.1 (2016-09-27)
===============================

-  Initial support for arvados mission

Changes for v1.1.0 (2016-09-27)
===============================

-  Begin work on missions

-  aegea-deploy-pilot: admit dashes in branch name via service name

-  Fix bug where tweak overwrote config file supplied via environment

-  Online documentation improvements

Changes for v1.0.0 (2016-09-22)
===============================

-  Aegea build\_image renamed to build\_ami
-  Aegea tag, untag
-  Doc improvements
-  Ubuntu 14.04 compatibility and role improvements
-  docker-event-relay reliability improvements
-  Remove snapd from default loadout
-  aegea volumes: display attachment instance names
-  aegea-deploy-pilot: Deploy on SIGUSR1

-  Initial support for flow logs
-  Pretty-print and perform whois lookups for aegea security\_groups
-  aegea ls security\_groups: break out protocol into its own column
-  Print security group rules in aegea ls security\_groups
-  List security groups in aegea ls
-  Print zone ID in aegea zones
-  Aegea deploy reliability improvements: use per-pid queues
-  Aegea launch reliability improvements: Back off on polling the EC2
   API

Changes for v0.9.8 (2016-08-23)
===============================

-  Update release script
-  Config updates
-  Sort properly while formatting datetimes
-  Continue ALB support

Changes for v0.9.7 (2016-08-17)
===============================

-  Add babel and format relative dates
-  Add aegea elb create
-  Changes in support of app deploy infrastructure
-  Add R default mirror config
-  IAM principal lists now report attached policies

Changes for v0.9.6 (2016-08-14)
===============================

Continue release script

Changes for v0.9.5 (2016-08-14)
===============================

Continue release script

Version 0.7.0 (2016-05-29)
--------------------------
- Introduce rds subcommand

Version 0.6.0 (2016-05-29)
--------------------------
- Rollup: many changes

Version 0.5.0 (2016-05-05)
--------------------------
- Rollup: many changes

Version 0.4.0 (2016-04-19)
--------------------------
- aegea audit implementation (except section 4)
- numerous image improvements

Version 0.3.0 (2016-04-12)
--------------------------
- Rollup: many changes

Version 0.2.3 (2016-03-30)
--------------------------
- Rollup: many changes

Version 0.2.1 (2016-03-12)
--------------------------
- Begin tracking version history
- Expand test suite
