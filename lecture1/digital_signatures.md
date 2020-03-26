## Digital Signatures

![Signatures requirements](./img/signatures.png)

#### But how we can turn it into digital form?

![Digital Signatures Api](./img/api_signatures.png)

![Requirements](./img/require_signatures.png)

#### What is really means "can't forge signatures"? It's easy to understand after looking at image below.

![Attacker game](./img/game.png)
Both have public key. The attacker sends different messages and gets the sign of each document. And he's going to send over what he claims is a signature on that message. The challenger is going to run the verify algorithm, use the public verification key on that message, and the signature that the attacker provided, and is going to check whether it verifies. And if it does verify, if this returns true, then the attacker wins, the attacker has forged a message.

#### In other words we want to make the attacker chances to be neglected.

## Practical part
![Practical stuff](./img/practical_sign.png)

### Bitcoin uses [ECDSA](https://uk.wikipedia.org/wiki/Elliptic_Curve_Digital_Signature_Algorithm) standart,  relies on hairy math and good randomness is essential!
