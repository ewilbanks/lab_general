

# To get an interactive node from head node:

`qsub -I -V -l nodes=1 -l walltime=00:10:00`

This specifies you want one node, for 10 minutes.  
-I means interactive
-V copies over your current environmental variables

# some resources
[UCSB quick start resource](http://csc.cnsi.ucsb.edu/sites/csc.cnsi.ucsb.edu/files/docs/csc_quickstart_0.pdf)
[PBS options explained well here, oak ridge national lab resource[(https://www.olcf.ornl.gov/for-users/system-user-guides/rhea/running-jobs/)


