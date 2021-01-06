# Unit-18-Homework

### Create a repository, and instructions for launching the chain Create a README.md in your project directory and create documentation that explains how to start the network. Remember to include any environment setup instructions and dependencies. Be sure to include all of the geth flags required to get both nodes to mine and explain what they mean. Explain the configuration of the network, such as it's blocktime, chain ID, account passwords, ports, etc. Explain how to connect MyCrypto to your network and demonstrate (via screenshots and steps) and send a transaction. Upload the code, including the networkname.json and node folders.

To access and send funds over the chain4unit18 blockchain private test network, you need to open two gitbash command prompt windows and navigate in each to C:\Users\bhkar\BH_UW_Bellevue_Fintech\Unit 18 Homework. No environment dependancies are necesary to operate the network, at least on my machine. Then, you will initialize both nodes: in gitbash window 1, type:
./geth --datadir node1 --mine --minerthreads 1

This will initialize mining for that node. if necesary, node1 password = lalala

Then, in gitbash window 2, type:

./geth --datadir node2 --port 30304 --rpc --bootnodes "enode://305d20d3f72402091989ed5018ff460a075e2213fdfac4720d7af29c7b28e793ed6d223397066a83083a25805da9a92ccc9f23d13459483737034f350cb994cf@127.0.0.1:30303" --ipcdisable

this will initialize "looking for peers" for that node. if necesary, node2 password = lelele

The blocktime of this network is 15 seconds, and its chain ID is 699. There are currently two accounts on the network. To transact and veiw balances of these, open the MyCrypto desktop app.  

Public address of key 1:   0x97d09ce07f374268be29f47dddc061a68928ef54

Public address of key 2:   0xfe596dcfe83bb9a4b833f9fbce41a7f2b7fd48bf

The above public addresses are sufficient to view balances. To transact, you will need to log on using the private key, a login option which are the following, respectively:
remember, never share a REAL private key. this is for test ONLY. 

private key 1 = 0xe1b0f3c21be42dbac82a5b540808fe8077bfec591e423be7115fd9af8f455b73
private key 2: 

unlock a wallet using a privte key. ensure you are connected to chain4unit18 by selecting "change network" on left side. then, in the "to address" field, type public address of recipient. set a transation fee, then hit send transation. verify by searching for the hash with the "TX Status" on left side.



