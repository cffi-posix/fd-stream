# fd-stream

fd-stream streams are `(unsigned-byte 8)` cl-stream streams
using `unistd:read`, `unistd:write` and `unistd:close` to
operate on Unix file descriptors.

## Class: fd-stream

### Generic: stream-fd *fd-stream* => *fd*
Returns the file descriptor of FD-STREAM.

## Class: fd-input-stream
A buffered input stream using UNISTD:READ.

### Function: fd-input-stream *fd* => *stream*
Creates an input stream for file descriptor *fd*.

## Class: fd-output-stream
A buffered output stream using UNISTD:WRITE.

### Function: fd-output-stream *fd* => *stream*
Creates an output stream for file descriptor *fd*.

## Class: fd-io-stream
A buffered input/output stream using UNISTD:READ and UNISTD:WRITE.

### Function: fd-io-stream *fd* => *stream*
Creates an input/output stream for file descriptor *fd*.
