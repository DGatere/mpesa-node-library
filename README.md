# mpesa-node-library
**M-Pesa Library for Node.js using REST API**

This package is intended to assist Node.js developers to use the M-Pesa API.

Before using the transaction API set the consumer key and consumer secret from <br>My Apps > Select App > copy Consumer Key and Consumer Secret and paste within quotes:

<<<<<<< HEAD
`const consumer_key = 'INSERT CONSUMER KEY HERE';`<br>
`const consumer_secret = 'INSERT CONSUMER SECRET HERE';`
=======
const consumer_key = 'INSERT CONSUMER KEY HERE';

const consumer_secret = 'INSERT CONSUMER SECRET HERE';
>>>>>>> 4dc8ae0091e21c196a59fa6f176c4ee74de06757

On the security function set your security credential value as specified within quotes:<br>
`let bufferToEncrypt = new Buffer("ENTER SECURITY CREDENTIAL TEXT HERE");`

**Usage**

**B2C Request**

This initiates a business to customer transactions from a company (short code) to end users (mobile numbers) of their services.

<<<<<<< HEAD
B2C(initiatorName, commandId, amount, partyA, partyB, remarks, queueUrl, resultUrl, occasion)<br>
Example: `mpesa.B2C('testapi', 'BusinessPayment', '100', '600133', '254708374149', 'test', 'http://randomurl.com', 'http://randomurl2.com');`
=======
B2C(initiatorName, commandId, amount, partyA, partyB, remarks, queueUrl, resultUrl, occasion)
Example: mpesa.B2C('testapi', 'BusinessPayment', '100', '600133', '254708374149', 'test', 'http://randomurl.com', 'http://randomurl2.com');
>>>>>>> 4dc8ae0091e21c196a59fa6f176c4ee74de06757

**B2B Request**

This initiates a business to business transaction between one company to another.<br>
B2B(initiator, commandId, senderId, receiverId, amount, partyA, partyB, accountRef, remarks, queueUrl, resultUrl, occasion)<br>
Example: `mpesa.B2B('testapi', 'BusinessPayBill', '4', '4', '1000', '600133', '600000', 'BusinessA', 'test', 'http://randomurl.com','http://randomurl2.com', 'test');`

<<<<<<< HEAD
=======
B2B(initiator, commandId, senderId, receiverId, amount, partyA, partyB, accountRef, remarks, queueUrl, resultUrl, occasion)
Example: mpesa.B2B('testapi', 'BusinessPayBill', '4', '4', '1000', '600133', '600000', 'BusinessA', 'test', 'http://randomurl.com', 'http://randomurl2.com', 'test');
>>>>>>> 4dc8ae0091e21c196a59fa6f176c4ee74de06757
