# Improvements

- Replicated DNS is now no longer required.  While this seemed
  like a great idea at the time (a staple of BIND9 administration),
  BOSH proves to be a better way of replicating changes to
  multiple DNS masters.  Now, the `slave-dns` link is optional.
