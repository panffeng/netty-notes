# ByteBuf

ByteBuf is derived from ByteBuffer included in java.nio. It is the data container for reading and writing operations. 

A stellar feature of netty is zero-copy. The feature strongly relies on implementation of ByteBufs to avoid both data copying and unnecessary resource overhead.

## Data containers

ByteBuf helps smooth the process of reading and writing streams.

## Supports for zero-copy feature

1. DirectByteBuf is employed to interact with I/O thread. Access to data via Unsafe class to direcly address any possible space in JVM requires no copying to finish data transporting.
2. CompositeByteBuf combines different ByteBufs into an integrated one by concatenating pointers without actually moving underlining data.

The other support for zero-copy comes from FileRegion to achieve zero-copy file transfer even though depending on operating systems and JRE.

