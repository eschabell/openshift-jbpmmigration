Update: June 2018 moved to [Gitlab](https://gitlab.com/eschabell/openshift-jbpmmigration)


jBPM Migration Tooling on OpenShift 
===================================
Installing the jBPM Migration tool on OpenShift was never easier!

This git repository helps you get up and running quickly with the jBPM
Migration Tooling.


Install with one click
----------------------
[![Click to install OpenShift](http://launch-shifter.rhcloud.com/launch/light/Click to install.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=jbossas-7&initial_git_url=git@github.com:eschabell/openshift-jbpmmigration.git&name=jbpmmigration)


Manual setup on OpenShift
------------------------- 
Create a jbossas-7 application

    rhc app create jbpmmigration -t jbossas-7 --from-code git://github.com/eschabell/openshift-jbpmmigration.git

That's it, you can now checkout your application at:

    http://jbpmmigration-$your_domain.rhcloud.com/jbpmmigration_upload-0.7

USAGE NOTES:

You can submit a jBPM jPDL 3.2 process definition as an xml file upload, the
resulting page will show you first your submitted file (if all goes well) and
the resulting BPMN2 process definition. This can be cut and paste into your IDE
for formatting and testing against the jBPM5 editor(s).

