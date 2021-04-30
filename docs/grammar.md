# Nyx Grammar

program       = statement*

statement     = expression

expression    = atom

atom          = number

number        = integer

integer       = HEX_PREFIX HEX_CHAR+
              | OCTAL_PREFIX OCTAL_CHAR+
              | BINARY_PREFIX BINARY_CHAR+
              | DIGIT+

HEX_PREFIX    = '0x' | '0X'
OCTAL_PREFIX  = '0o' | '0O'
BINARY_PREFIX = '0b' | '0B'
HEX_CHAR      = [0-9a-fA-F]
OCTAL_CHAR    = [0-7]
BINARY_CHAR   = [0-1]
DIGIT         = [0-9]