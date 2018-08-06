# How to braid
## Get a user account
The cluster we'll primarily use is Braid.  Check out our Slack channel #compute for details 
about how to get your account.  Other good contact folks are 
 http://csc.cnsi.ucsb.edu/acct

To ssh into the cluster you need to either be using a campus network (e.g. physically on campus) or you need to be running the campus VPN.  Info on how to use VPN is below.  
http://www.ets.ucsb.edu/services/campus-vpn

You will need your UCSBnetID to log in.  If you don't have a ucsb campus id for some reason, we can get you access as a University Affiliate by sending an email to Paul Weakliem <weakliem@cnsi.ucsb.edu>, Fuzzy Rogers <fuz@ucsb.edu>  and stating that you are a member/collaborator of my group that needs access.  *Please cc me on any such email.*  To create your account, they will need your date of birth and the last 4 digits of your SSN if you have one.


## Log in
you must either be on a campus network or using the UCSB VPN.  
VPN information:
`ssh username@braid.cnsi.ucsb.edu`

## Make your life easy and don't type long ssh commands and enter passwords all the time... 
[make an alias to avoid typing whole username and server id](https://scotch.io/tutorials/how-to-create-an-ssh-shortcut)

[a useful cheatsheet for avoiding passwords: SSH onto an HPC](https://alexiswl.github.io/ASimpleNanoporeTutorial/basic_shell_logging.html)


# Do's and Don'ts on braid
## Don't run on the head node.  
 
 Either grab an interactive session on a compute node to quickly noodle around with something.  
 Or submit a job properly.  Examples of both are below, as are some learning resources.
 
## To get an interactive session on a compute node
`qsub -I -V -l nodes=1:ppn=2 -l walltime=00:10:00`
This specifies you want an interactive session two processors on a single node, for 10 minutes.
How?
* `-I` means interactive
* `-V` copies over your current environmental variables
* `nodes=1` you want a single node(`nodes=1`), 
* `ppn=2` you want two processors
* `walltime=00:10:00` for 10 minutes (massively overestimating time needed will slow your position in queue)  

### when you're done
type `exit` to kill the job and free up that space in queue

## some resources
[UCSB quick start resource](http://csc.cnsi.ucsb.edu/sites/csc.cnsi.ucsb.edu/files/docs/csc_quickstart_0.pdf)

[PBS options explained well here, oak ridge national lab resource](https://www.olcf.ornl.gov/for-users/system-user-guides/rhea/running-jobs/)
