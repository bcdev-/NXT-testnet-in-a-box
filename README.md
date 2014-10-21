Your own juicy Testnet for NXT!
====================
Just unpack the .tar.xz file, and start ./run.sh. You can also ./compile.sh if you want to make modifications to the code.

The genesis block distributes reward to two accounts:
"aaa" and "aab"
However, in the default database I've transferred all the founds from "aab" to "aaa".
To make a testnet with many peers, simply add peers into conf/nxt-default.properties to section "nxt.wellKnownPeers".

It's impossible to run many NXT clients on once computer, but you can easily get around this by running NXT in lxc.

Unfortunately, due to a bug in GUI, you need to start forging by running an API command:
http://localhost:7876/nxt?requestType=getForging&secretPhrase=aaa

See http://nxtstorm.org/index.php/How_to_create_your_own_testnet-in-a-box if you want to create your own genesis block.
