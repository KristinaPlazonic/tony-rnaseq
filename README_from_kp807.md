
The readme instructions provided by OSC are very good and you should follow them. 

My only contribution is 
 - verifying that it works, and 
 - providing sample slurm batch file
 - testing modifying the form and 
 - adding default values to the form
 - adding some output files to the script to verify it works with input and output files. 

## Important URIs

- [Original source](https://github.com/OSC/ood-example-batch)
- Your path to the dev directory on Amarel should be `/home/kp807/ondemand/dev/example-batch`
- To access the app from ondemand go to https://ondemand.hpc.rutgers.edu/pun/dev/example-batch/
- To see video of the demo: https://www.youtube.com/watch?v=fI-yR5XQaAw&feature=youtu.be 

## Customizing your app
modify these files:

app/models/job.rb              -- this defines the paramters to the job as a class!!! - should be mirrored in form, show, index. 
template/main.sh.erb           -- this defines the main script!!
app/views/jobs/_form.html.erb  -- this defineds the form to input the parameters to the main script!!!
app/views/jobs/index.html.erb
app/views/jobs/show.html.erb


