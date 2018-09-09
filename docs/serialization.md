---
title:  Serialization format
---


## Serialization

For the simple, flat structure described in the [data model](../model) a delimited-text format is appropriate.

Sepcifications:

1.  Text files will use UTF-8 encoding.
2.  Objects are separated by a unique string that is not allowed in the contents of annotations.  The default value for the object separator will be a newline character (`\n`, 0x0A).
4.  Properties of each object are separated by a second unique string that is not allowed in the contents of annotations.  The default value for the property separator will be a pound sign (hash tag, `#` 0x23).
2.  The first entry in the file is a header line with human-readable labels for the columns.  The structure of the header record is identical to the structure of data record.
