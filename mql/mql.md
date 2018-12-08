# MQL Commands
List of MQL commands on a business object. In all commands, T means type, N means Name, and R means revision of the business object.

## To add a business object.
```mql
MQL<1> add bus T N R policy <policyName> vault <vaultName>
```

## To add a business object and updating the attributes in a single command.
```mql
MQL<2> add bus T N R policy <policyName> vault <vaultName> "attribute name 1" "attribute 1 value" "attribute name 2" "attribute 2 value"
```

## To find the number business objects by using temp query bus.
```mql
MQL<3>eval expr ' count true ' on temp query bus "Part" * * where " originated > '01/01/1990' ";
```
549

## To find the number business objects that are connected to a business object.
```mql
MQL<4>eval expr ' count true ' on expand bus Part PRT-001 1;
```
7

## To know the current context
```mql
MQL<5>print context;
```
context vault eService Production person Test Everything

## To know how many users connected to eMatrix (sesssions).
```mql
MQL<6>sessions;
```

## To monitor memory usage...
```mql
MQL<7>monitor memory
```

## To know version of the software installed...
```mql
MQL<8>version;
```
V6R2009x

