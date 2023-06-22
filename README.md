# BASIC Templating Language

This is a templating language for BASIC. It is dependent on using my implementation of hashmaps. This is part of my general TCL utilities.

## Usage

```
*
    EQU ENV.SIZE TO 5000
    DIM ENV(ENV.SIZE)
*
    MAT ENV = ''
*
    CALL MAP.SET(MAT ENV,ENV.SIZE,'NAME','Bob')
*
    TEMPLATE = '<div>Hello {{ NAME }}</div>'
    CALL RENDER(MAT ENV,ENV.SIZE,TEMPLATE,RESULT)
    PRINT RESULT
*
* END OF PROGRAM
*
END
```

Outputs:

```
<div>Hello Bob</div>
```

## Installation

Installation can be done by using NPM. You can also manually install the below programs.

```
NPM INSTALL BP RENDER https://raw.githubusercontent.com/Krowemoh/basic-template-language/main/RENDER
NPM INSTALL BP RAW.RENDER https://raw.githubusercontent.com/Krowemoh/basic-template-language/main/RAW.RENDER
NPM INSTALL BP RAW.RENDER https://raw.githubusercontent.com/Krowemoh/basic-template-language/main/EVALUATE
```
