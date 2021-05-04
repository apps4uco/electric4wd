# DBC

DBC file is a proprietary format that describes the data over a CAN bus. 

<http://socialledge.com/sjsu/index.php/DBC_Format>

<https://docs.openvehicles.com/en/latest/components/vehicle_dbc/docs/dbc-primer.html>

<https://www.csselectronics.com/screen/page/can-dbc-file-database-intro/language/en>

<http://read.pudn.com/downloads766/ebook/3041455/DBC_File_Format_Documentation.pdf>

ej.
~~~
VERSION "DBC Example 1.0"

BS_: 500000 : 0,0

BO_ 500 IO_DEBUG: 4 IO
 SG_ IO_DEBUG_test_unsigned : 0|8@1+ (1,0) [0|0] "" DBG
 SG_ IO_DEBUG_test_signed : 8|8@1- (1,-128) [0|0] "" DBG
 SG_ IO_DEBUG_test_float1 : 16|8@1+ (0.1,0) [0|0] "" DBG
 SG_ IO_DEBUG_test_float2 : 24|12@1+ (0.01,-20.48) [-20.48|20.47] "" DBG
 
 
BO_ 500 IO_DEBUG: 4 IO
 SG_ IO_DEBUG_test_enum : 8|8@1+ (1,0) [0|0] "" DBG

BA_ "FieldType" SG_ 500 IO_DEBUG_test_enum "IO_DEBUG_test_enum";

VAL_ 500 IO_DEBUG_test_enum 2 "IO_DEBUG_test2_enum_two" 1 "IO_DEBUG_test2_enum_one" ; 
~~~

## J1939

DBC Definition de J1939 500 Euros



<https://github.com/commaai/opendbc.git>


<https://docs.openvehicles.com/en/latest/components/vehicle_dbc/docs/dbc-primer.html>



# Librerias

## DBCC

dbcc can translate data base CAN files into Rust code. The generated code allows interacting with CAN signals in a type safe manner by e.g. matching against signal value enum types.

Fuente <https://crates.io/crates/dbcc/2.0.0>

## CanParse

A CAN signal and definition parser, written in Rust.

The goal of canparse is to provide a means of converting CAN frames into pre-defined signals, via CANdb definition input (DBC). One common application is the J1939 spec, which defines a set of common parameters for heavy-duty trucks and other vehicles. PgnLibrary is also included as an application of DBC, to give first-class support for the PGN/SPN schema.


Fuente <https://crates.io/crates/canparse>

<https://docs.rs/canparse/0.1.4/canparse/>

## DBC Codegen 

<https://crates.io/crates/dbc-codegen-cli>

<https://crates.io/crates/dbc-codegen>

## CAN DBC

<https://crates.io/crates/can-dbc/3.0.2>

