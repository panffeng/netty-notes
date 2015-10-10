# Channel

> A [Channel](https://docs.oracle.com/javase/7/docs/api/java/nio/channels/Channel.html) represents an open connection to an entity such as a hardware device, a file, a network socket, or 
> a  program  component  that  is  capable  of  performing  one  or  more  distinct  I/O 
> operations, for example reading or writing. 

## Channel state
A channel with netty has an internal state representing the lifecyle. Those states include registered channel, active channel, inactive channel and unregistered channel.
