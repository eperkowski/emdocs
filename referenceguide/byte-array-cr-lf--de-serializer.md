
Serializes data terminated by CR+LF
Reads data in an <code>InputStream</code> to a <code>byte[]</code>; data must be terminated by <code>\r\n</code> (not included in resulting <code>byte[]</code>).

Writes a <code>byte[]</code> to an <code>OutputStream</code> and adds <code>\r\n</code>.


Id
Name that uniquely identifies this flow component.

<i>Required</i>


Max message size
The maximum supported message size (in bytes) for this (de)serializer.

Default is <i>2048</i> (2 KiB).

To avoid memory exhaustion due to a badly behaved client (one that does not adhere to the protocol of the configured serializer), this (de)serializer imposes a maximum message size. If the size is exceeded by an incoming message, an exception will be thrown. The default maximum message size is 2048 bytes, and can be increased by setting the <i>maxMessageSize</i> property.

