# ignore

`Usage: ignore REGEX COMMAND [ARG...]`

Any lines matching the regular expression will be removed from the command's standard error stream.  

If the standard error stream is then empty, exit status is 0; otherwise it is that of the command.  

Usage of anchors (`^` for line beginning and `$` for line end) is recommended; otherwise error messages may be unintentionally removed.  
For example, an empty regular expression (like `ignore ""`) will ignore any error.
