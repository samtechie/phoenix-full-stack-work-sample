# Fly.io Full Stack Phoenix Hiring Project Notes

- ### What I built

  - I added the information displayed by the `flyctl status` command.
    I followed the exact styling of the _Process Groups_.
  - The app refreshes every 30 seconds to track any recent changes. Here LiveView shines because it will only update areas which have been changed.

- ### What I would improve

  - The tables for the other information are too wide and as a result you have to scroll sideways to see all the information which is not great for UX. This is something that can be improved perhaps by splitting the data and presenting it on different lines. This may be fine if you only have one occurrence of a data item i.e one row in the table for example for _Deployment Status_ but it may quickly break down if you have multiple occurrences as is the case for _Instances_. A potential solution could be displaying the data of each occurrence separately such that a user can clearly distinguish between occurrences.
  - Add an option to delete apps. I found myself having to go to the production app to be able to delete apps.
  - I would love to be able to see the running costs of each app quickly. An example of this could be a calculator that will enable one to select applications and be able to quickly see their current cost.
  - Displaying the deployment logs for each app. Here I wouldn't display all the logs but I could display the most recent logs which could be useful in debugging potential causes of an app crashing or misbehaving.
  - I would add tooltips explaining each data item such that users can get a better understanding of what they are looking at.
  - I would add an easy copy option for ids of VMs because I constantly found myself copying ids for use with some `flyctl` commands

- ### How I would determine if this feature is successful
  The first thing I would do is determine the goal of this feature. In this case for example the feature could be an alternative to running `flyctl status` in a terminal. If there is a way to measure the metrics of the people who use the terminal specifically to run the command versus those who use the feature. I could determine if the feature has succeeded in changing or influencing behavior. Another way I can track this is observing the people who copy the ids of VMS in the case that this functionality has been implemented in the feature.
