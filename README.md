# Resource Plan State Automation
ServiceNow ITBM - Resource Plan State Automation

This functionality was created in the Flow Designer on the NY release. Its purpose is to automatically close all resource plans attached to a project when it is closed. For example purposes we populated the "End Date" field on the resource plan with the "Planned End Date" of the project upon closure. Keep in mind this is conceptual in nature and this workflow can be modified to fit your organizations needs.

There are 3 components developed in this update set:

1. A refrence field was created on the resource plan called project ('u_project'). The reason this is needed is because out of the box the field linking a resource plan to a project is not always defined in the task field. we address this linkage in with a workflow to populated this field.

2. Populate Project on RP - This flow populates the field above. See uploaded screenshot of the flow.

3. Close Resource Plans on PRJ - This flow completes the physical action of closing resource plans. See uploaded screenshot of the flow.
