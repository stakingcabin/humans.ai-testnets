<div>
<h1 align="left" style="display: flex;"> Humans testnet humans_3000-23</h1>
</div>

# Restart validator three times during Mission 2

### Restart 1 - 2023 May 14 03:44:13

~~~bash
ubuntu@ip-172-31-31-181:~$ sudo systemctl restart humansd
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM INF service stop impl={"Logger":{},"Switch":{"Logger":{}}} module=pex msg={} server=node
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM INF service stop book=/home/ubuntu/.humansd/config/addrbook.json impl={"Logger":{}} module=p2p msg={} server=node
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM INF Closing rpc listener listener={"Listener":{}} server=node
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM INF Saving AddrBook to file book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node size=120
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM ERR Stopped accept routine, as transport is closed module=p2p numPeers=0 server=node
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM INF RPC HTTP server stopped err="accept tcp [::]:26657: use of closed network connection" module=rpc-server server=node
May 14 03:44:13 ip-172-31-31-181 humansd[23398]: 3:44AM ERR Error serving server err="accept tcp [::]:26657: use of closed network connection" server=node
May 14 03:44:13 ip-172-31-31-181 systemd[1]: humansd.service: Succeeded.
May 14 03:44:13 ip-172-31-31-181 systemd[1]: Stopped Humans Friction Node.
May 14 03:44:13 ip-172-31-31-181 systemd[1]: Started Humans Friction Node.
May 14 03:44:13 ip-172-31-31-181 humansd[23445]: 3:44AM INF Unlocking keyring
May 14 03:44:13 ip-172-31-31-181 humansd[23445]: 3:44AM INF starting ABCI with Tendermint
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF starting node with ABCI Tendermint in-process
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start impl=multiAppConn module=proxy msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start impl=EventBus module=events msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start impl=PubSub module=pubsub msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start impl=IndexerService module=txindex msg={} server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF ABCI Handshake App Info hash="g\x19z���\x05�p\x00�o���킒�8L�m�`��}���&" height=39305 module=consensus protocol-version=0 server=node software-version=0.2.1
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF ABCI Replay Blocks appHeight=39305 module=consensus server=node stateHeight=39305 storeHeight=39305
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF Completed ABCI Handshake - CometBFT and App are synced appHash="g\x19z���\x05�p\x00�o���킒�8L�m�`��}���&" appHeight=39305 module=consensus server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF This node is a validator addr=2839AC8B98EB0DD30FF85B5146EC9ECA5A4FC8A8 module=consensus pubKey=/z4qwKxn535R748+s2K/HKaQQo8ei4uoaG8P51J3nxg= server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF P2P Node ID ID=b9c1f8437819fa735c805dcbff8e149a2222d76c file=/home/ubuntu/.humansd/config/node_key.json module=p2p server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF Adding persistent peers addrs=[] module=p2p server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF Add our address to book addr={"id":"b9c1f8437819fa735c805dcbff8e149a2222d76c","ip":"0.0.0.0","port":26656} book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node
May 14 03:44:14 ip-172-31-31-181 humansd[23445]: 3:44AM INF service start impl=Node msg={} server=node
~~~

### Restart 2 - 2023 May 14 03:54:52

~~~bash
ubuntu@ip-172-31-31-181:~$ sudo systemctl restart humansd
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM INF service stop impl={"Logger":{},"Switch":{"Logger":{}}} module=pex msg={} server=node
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM INF service stop book=/home/ubuntu/.humansd/config/addrbook.json impl={"Logger":{}} module=p2p msg={} server=node
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM ERR Stopped accept routine, as transport is closed module=p2p numPeers=0 server=node
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM INF Closing rpc listener listener={"Listener":{}} server=node
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM INF Saving AddrBook to file book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node size=120
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM INF RPC HTTP server stopped err="accept tcp [::]:26657: use of closed network connection" module=rpc-server server=node
May 14 03:54:52 ip-172-31-31-181 humansd[23445]: 3:54AM ERR Error serving server err="accept tcp [::]:26657: use of closed network connection" server=node
May 14 03:54:52 ip-172-31-31-181 systemd[1]: humansd.service: Succeeded.
May 14 03:54:52 ip-172-31-31-181 systemd[1]: Stopped Humans Friction Node.
May 14 03:54:52 ip-172-31-31-181 systemd[1]: Started Humans Friction Node.
May 14 03:54:52 ip-172-31-31-181 humansd[23503]: 3:54AM INF Unlocking keyring
May 14 03:54:52 ip-172-31-31-181 humansd[23503]: 3:54AM INF starting ABCI with Tendermint
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF starting node with ABCI Tendermint in-process
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start impl=multiAppConn module=proxy msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start impl=EventBus module=events msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start impl=PubSub module=pubsub msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start impl=IndexerService module=txindex msg={} server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF ABCI Handshake App Info hash="&O���b��\x06@�\x03�w�:�\a9�\x1fZ?\x1b�L�]\x05�0B" height=39405 module=consensus protocol-version=0 server=node software-version=0.2.1
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF ABCI Replay Blocks appHeight=39405 module=consensus server=node stateHeight=39405 storeHeight=39405
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF Completed ABCI Handshake - CometBFT and App are synced appHash="&O���b��\x06@�\x03�w�:�\a9�\x1fZ?\x1b�L�]\x05�0B" appHeight=39405 module=consensus server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF This node is a validator addr=2839AC8B98EB0DD30FF85B5146EC9ECA5A4FC8A8 module=consensus pubKey=/z4qwKxn535R748+s2K/HKaQQo8ei4uoaG8P51J3nxg= server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF P2P Node ID ID=b9c1f8437819fa735c805dcbff8e149a2222d76c file=/home/ubuntu/.humansd/config/node_key.json module=p2p server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF Adding persistent peers addrs=[] module=p2p server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF Add our address to book addr={"id":"b9c1f8437819fa735c805dcbff8e149a2222d76c","ip":"0.0.0.0","port":26656} book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node
May 14 03:54:53 ip-172-31-31-181 humansd[23503]: 3:54AM INF service start impl=Node msg={} server=node
~~~

### Restart 3 - 2023 May 14 04:07:38

~~~bash
ubuntu@ip-172-31-31-181:~$ sudo systemctl restart humansd
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM INF service stop impl={"Logger":{},"Switch":{"Logger":{}}} module=pex msg={} server=node
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM INF service stop book=/home/ubuntu/.humansd/config/addrbook.json impl={"Logger":{}} module=p2p msg={} server=node
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM INF Closing rpc listener listener={"Listener":{}} server=node
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM INF Saving AddrBook to file book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node size=120
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM ERR Stopped accept routine, as transport is closed module=p2p numPeers=0 server=node
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM INF RPC HTTP server stopped err="accept tcp [::]:26657: use of closed network connection" module=rpc-server server=node
May 14 04:07:38 ip-172-31-31-181 humansd[23503]: 4:07AM ERR Error serving server err="accept tcp [::]:26657: use of closed network connection" server=node
May 14 04:07:38 ip-172-31-31-181 systemd[1]: humansd.service: Succeeded.
May 14 04:07:38 ip-172-31-31-181 systemd[1]: Stopped Humans Friction Node.
May 14 04:07:38 ip-172-31-31-181 systemd[1]: Started Humans Friction Node.
May 14 04:07:38 ip-172-31-31-181 humansd[23707]: 4:07AM INF Unlocking keyring
May 14 04:07:38 ip-172-31-31-181 humansd[23707]: 4:07AM INF starting ABCI with Tendermint
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF starting node with ABCI Tendermint in-process
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start impl=multiAppConn module=proxy msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start connection=query impl=localClient module=abci-client msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start connection=snapshot impl=localClient module=abci-client msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start connection=mempool impl=localClient module=abci-client msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start connection=consensus impl=localClient module=abci-client msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start impl=EventBus module=events msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start impl=PubSub module=pubsub msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start impl=IndexerService module=txindex msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF ABCI Handshake App Info hash="?�7΄��\x0f�\x01N�\t\f�$��,�V\x1cJ@χ~��3\x12)" height=39534 module=consensus protocol-version=0 server=node software-version=0.2.1
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF ABCI Replay Blocks appHeight=39534 module=consensus server=node stateHeight=39534 storeHeight=39534
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Completed ABCI Handshake - CometBFT and App are synced appHash="?�7΄��\x0f�\x01N�\t\f�$��,�V\x1cJ@χ~��3\x12)" appHeight=39534 module=consensus server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Version info abci=0.17.0 block=11 cmtbft_version=0.34.27 commit_hash= p2p=8 server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF This node is a validator addr=2839AC8B98EB0DD30FF85B5146EC9ECA5A4FC8A8 module=consensus pubKey=/z4qwKxn535R748+s2K/HKaQQo8ei4uoaG8P51J3nxg= server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF P2P Node ID ID=b9c1f8437819fa735c805dcbff8e149a2222d76c file=/home/ubuntu/.humansd/config/node_key.json module=p2p server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Adding persistent peers addrs=[] module=p2p server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Adding unconditional peer ids ids=[] module=p2p server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Add our address to book addr={"id":"b9c1f8437819fa735c805dcbff8e149a2222d76c","ip":"0.0.0.0","port":26656} book=/home/ubuntu/.humansd/config/addrbook.json module=p2p server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF service start impl=Node msg={} server=node
May 14 04:07:40 ip-172-31-31-181 humansd[23707]: 4:07AM INF Starting pprof server laddr=localhost:6060 server=node
~~~

