---
title:  Requirements for an end-user applications
---

## Back-end Requirements

1.  *Authentication*.  The application must require users to register with the application.  It should record a user name, a real name, and an email contact.
2.  *Persistent storage*.  The application must be able save annotations created by users.
3.  *Serialization*.  The application must support exporting the entire collection of annotations in the format [specified here](serialization).


## UI


1.  The application must allow users to register, and subsequently to authenticate  to the system before they can create new annotations.
1.  The application must allow users to provide a URN identifying an object to comment on.  In version 1, this will always be a text.
2.  The application must retrieve and display the text to comment on.
3.  The application must allow users to add and save comments.
4.  In saving comments, the application must create an appropriate version-specific CITE2 URN.  The version identifier should be determined from the user ID.
5.  The application should add a date stamp when a commet is created.
