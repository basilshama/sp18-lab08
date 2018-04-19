Basil Abushama & Uriel Rodriguez -- bshama@berkeley.edu & urielrodriguez@berkeley.edu

### What's going on in `Mystery.sol`?

##### Answer:
It copies "calldatasize" bytes from position 0 to memory at position "o_code".

It calls the contract at "addr", the destination address, with gas "g", starting at location "o_code",
with inputs being "calldatasize" bytes long and outputs being 32 bytes long.

It then returns 32 bytes of memory starting from 0x40.