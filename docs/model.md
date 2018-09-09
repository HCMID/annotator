---
title:  Data models
---


## Annotations

An *annotation* is an association of two citable units:  the unit that is annotated, and the annotation.

For  scholarship in the humanities, we use URNs to identify citable entities.  (For background on technology-independent, machine-actionable citation of scholarly resources, see <http://cite-architecture.github.io/>).  At its simplest, then, an annotation can be expressed by pairing two URNs.


## Data model for an annotation authoring application

An application for creating annotations does not require much additional information:  the contents of the annotation, and a time stamp.    The application can manage a collection of objects composed of:


1.  a URN identifying the thing annotated (e.g., for a passage of text, a CTS URN).  The URN should include a version identifier specifying the specific version of the text or object that is being annotated.
2.   a CITE2 URN identifying the annotation. This will also include a specific version identifier.
3.  content of annotation
4.  time stamp


There is no need to include metadata such as authorship in this structure:  instead, that can be be managely separately by associating it with a particular version of the collection of annotations.
