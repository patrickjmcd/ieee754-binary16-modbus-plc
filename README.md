# IEEE Binary16 Modbus PLC Conversion

Developed by Patrick McDonagh

## Usage

This program converts an unsigned integer (UINT) data type to an IEEE-754
Binary16 (also called Float16) half-precision floating point number. Since
Rockwell Automation PLC's do not have a half-precision floating point number
data type, the data is stored in a REAL (32-bit) data type.

This program operates as two separate User-Defined Functions within Connected
Components Workbench. In order to use the function, just import
Controller.Micro820.Micro820.ReverseUINT.7z and
Controller.Micro820.Micro820.WordToFloat16.7z into your project. Run the
conversion on a tag of type WORD using the following:

```
float16_output := WordToFloat16(word_tag);
```

## Source Code

The source code for the functions can be viewed by importing the archive files
or by examining the .stf files in this repository.
