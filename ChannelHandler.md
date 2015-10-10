# ChannelHandler

## ChannelHandler State

Given a ChannelPipeline, a ChannelHandler is supposed in one of the following states: handler added, handler removed or exception caught. 

When state transissions occur, corresponding callback methods with a channel handler will be invoked.
