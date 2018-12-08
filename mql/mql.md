# MQL Commands
List of MQL commands on a business object. In all commands, T means type, N means Name, and R means revision of the business object.

## To add a business object. 
MQL<1> add bus T N R policy <policyName> vault <vaultName>

## To add a business object and updating the attributes in a single command.
MQL<2> add bus T N R policy <policyName> vault <vaultName> "attribute name 1" "attribute 1 value" "attribute name 2" "attribute 2 value"

## To find the number business objects by using temp query bus.
MQL<3>eval expr ' count true ' on temp query bus "Complaint" * * where " originated > '01/01/2009' ";
549

## To find the number business objects that are connected to a business object.
MQL<3>eval expr ' count true ' on expand bus Complaint CPT090000011 1;
7

## To know the current context
MQL<4>print context;
context vault eService Production person Test Everything

## To know how many users connected to eMatrix (sesssions).
MQL<13>sessions;
HimnishTechnologies\parin HimnishTechnologies\HT00001 mql.exe
HimnishTechnologies\parin HimnishTechnologies\HT00001 mql.exe
HimnishTechnologies\ajay  HimnishTechnologies\HT00002 business.exe


## To monitor memory usage...
MQL<21>monitor memory

Used heap 1689786 bytes, free heap 43008 bytes.

Matrix Memory Manager:

547220 bytes of memory allocated in 46 blocks, highwater= 570272 bytes
0 bytes of memory reserved in 0 blocks
JVM total memory: 5177344
JVM max memory: 133234688
JVM free memory: 4489456
JVM memory in use: 687888
JVM available processors: 2

## To know version of the software installed...
MQL<22>version;
V6R2009x.HF29

