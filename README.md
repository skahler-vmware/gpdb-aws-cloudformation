First pass at a GPDB AWS cloud formation script

The script relies on an AMI with:
* a script to format and create a /data partition of the drive
* system options pre-tuned for GPDB
* GPDB already installed on the system

Issues
* IP conflicts if something in the node cluster is allocated a master ip, cluster deploy will rollback
  

Todo
* Variable for GPDB version which is pulled from download location
* install and init of GPDB itself
* install and init of GPCC
  
