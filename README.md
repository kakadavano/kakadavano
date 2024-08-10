import { createThirdwebClient, getContract } from "thirdweb";
import { defineChain } from "thirdweb/chains";

// create the client with your clientId, or secretKey if in a server environment
const client = createThirdwebClient({ 
  clientId: "YOUR_CLIENT_ID"
 });

// connect to your contract
const contract = getContract({ 
  client, 
  chain: defineChain(1919), 
  address: "0xdb9B731a5A83df780662108709A0ad02EceF656D"
});
