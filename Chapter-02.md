
## Basics of Bitcoin Cryptography

### First, Some Useful Definitions
- **bitcoin:** Without capitalization, is used to describe the currency and unit of account for the Bitcoin network.
- **Bitcoin:** With capitalization, is used to describe the concept, network, development project, and enthusiast community.
- **Bitcoin address:** A string of letters and numbers where bitcoin can be sent, similar to how one sends email to an email address.
- **transaction:** A record informing the network of a transfer of bitcoin from one bitcoin address to another.
- **blockchain:** The complete transaction ledger of the Bitcoin network, showing how bitcoin have been transferred from one address to another over time. The blockchain is a public record of all bitcoin transactions in chronological order.

> Think of a Bitcoin transaction as a single value transfer recorded in a ledger, a block as a page of transactions from the last ten minutes, and a blockchain as the whole ledger book.

## Βασικά της Κρυπτογραφίας του Bitcoin

### Πρώτα, Μερικοί Χρήσιμοι Ορισμοί
- **bitcoin:** Χωρίς κεφαλαία, χρησιμοποιείται για να περιγράψει το νόμισμα και τη μονάδα λογαριασμού για το δίκτυο Bitcoin.
- **Bitcoin:** Με κεφαλαία, χρησιμοποιείται για να περιγράψει την έννοια, το δίκτυο, το έργο ανάπτυξης και την κοινότητα ενθουσιωδών.
- **Διεύθυνση Bitcoin:** Μια σειρά από γράμματα και αριθμούς όπου μπορούν να σταλούν bitcoin, παρόμοια με το πώς στέλνουμε email σε μια διεύθυνση email.
- **Συναλλαγή:** Ένα αρχείο που ενημερώνει το δίκτυο για τη μεταφορά bitcoin από μία διεύθυνση bitcoin σε άλλη.
- **Blockchain:** Το πλήρες μητρώο συναλλαγών του δικτύου Bitcoin, που δείχνει πώς τα bitcoin έχουν μεταφερθεί από μία διεύθυνση σε άλλη με την πάροδο του χρόνου. Το blockchain είναι ένα δημόσιο αρχείο όλων των συναλλαγών bitcoin με χρονολογική σειρά.

> Σκεφτείτε μια συναλλαγή Bitcoin ως μια μεμονωμένη μεταφορά αξίας που καταγράφεται σε ένα μητρώο, ένα block ως μια σελίδα συναλλαγών από τα τελευταία δέκα λεπτά και ένα blockchain ως ολόκληρο το βιβλίο μητρώου.

## Bitcoin: Foundations and Cryptographic Technologies
Bitcoin is a collection of concepts and technologies that form the basis of a digital money ecosystem, including:
- A decentralized peer-to-peer network (enabled by the Bitcoin protocol)
- A public transaction ledger (the blockchain)
- A decentralized mathematical and deterministic currency issuance mechanism (distributed mining and the “Proof-of-Work” consensus algorithm)
- A decentralized transaction verification system (transaction script)

To achieve this, Bitcoin relies heavily on cryptographic technologies, such as:
- Hash functions (i.e. SHA-256 and RIPEMD-160)
- Public Key Cryptography (i.e. ECDSA – the Elliptic Curve Digital Signature Algorithm)

## Bitcoin: Θεμέλια και Κρυπτογραφικές Τεχνολογίες
Το Bitcoin είναι μια συλλογή από έννοιες και τεχνολογίες που αποτελούν τη βάση ενός οικοσυστήματος ψηφιακού χρήματος, περιλαμβάνοντας:
- Ένα αποκεντρωμένο δίκτυο peer-to-peer (ενεργοποιημένο από το πρωτόκολλο Bitcoin)
- Ένα δημόσιο μητρώο συναλλαγών (το blockchain)
- Ένας αποκεντρωμένος μηχανισμός έκδοσης νομίσματος με μαθηματική και ντετερμινιστική βάση (κατανεμημένη εξόρυξη και ο αλγόριθμος συναίνεσης “Proof-of-Work”)
- Ένα αποκεντρωμένο σύστημα επαλήθευσης συναλλαγών (σενάριο συναλλαγών)

Για να επιτύχει αυτό, το Bitcoin βασίζεται σε μεγάλο βαθμό σε κρυπτογραφικές τεχνολογίες, όπως:
- Συναρτήσεις κατακερματισμού (π.χ. SHA-256 και RIPEMD-160)
- Δημόσια Κλειδαριζόμενη Κρυπτογραφία (π.χ. ECDSA – ο Αλγόριθμος Ψηφιακής Υπογραφής Ελλειπτικής Καμπύλης)

## Bitcoin and Cryptography

### Transactions
- A transaction is a record that informs the network of a transfer of funds or value from one owner to another.
  - Think of a transaction as a single line on a page in a notebook.
  - Think of a block as the page in that notebook.
  - Think of the blockchain as being equivalent to the entire notebook.
  - All the users are able to read, write, and get updated on what is written in this notebook.
- Ownership of bitcoin is established through the relationship between public keys and the digital signatures produced from the corresponding private keys.

## Bitcoin και Κρυπτογραφία

### Συναλλαγές
- Μια συναλλαγή είναι ένα αρχείο που ενημερώνει το δίκτυο για μια μεταφορά κεφαλαίων ή αξίας από έναν ιδιοκτήτη σε έναν άλλο.
  - Σκεφτείτε μια συναλλαγή ως μια μεμονωμένη γραμμή σε μια σελίδα σε ένα σημειωματάριο.
  - Σκεφτείτε ένα block ως τη σελίδα σε αυτό το σημειωματάριο.
  - Σκεφτείτε το blockchain ως ισοδύναμο με ολόκληρο το σημειωματάριο.
  - Όλοι οι χρήστες μπορούν να διαβάζουν, να γράφουν και να ενημερώνονται για το τι είναι γραμμένο σε αυτό το σημειωματάριο.
- Η ιδιοκτησία των bitcoin καθορίζεται μέσω της σχέσης μεταξύ δημόσιων κλειδιών και των ψηφιακών υπογραφών που παράγονται από τα αντίστοιχα ιδιωτικά κλειδιά.

## Digital Keys
A mathematically-related public-private key pair, created using the Elliptic Curve Digital Signature Algorithm (ECDSA):
1. **Private key (Privkey):** is essentially a randomly generated number that should be kept secret. It is used to generate digital signatures and confirm ownership, authorizing the spending of bitcoin.
2. **Public key (Pubkey):** Is generated from the private key using the elliptic curve multiplication process. When spending and receiving, the public key is represented by a bitcoin address.
   - "Think of the public key as similar to a bank account number and the private key as similar to the secret PIN, or signature on a check, that provides control over the account."
3. **Bitcoin Address:** An address is a unique identifier for the destination of a bitcoin payment, generated from and corresponding to a public key or script.
   - It is usually generated by applying the SHA-256 and RIPEMD-160 cryptographic hash functions in series, on the public key.
   - These addresses are encoded using Base58 encoding, which represents an address in a human-readable form of 58 alphanumeric characters.
   - Fun fact: There are 52 characters in the alphabet, if we include all upper and lower-case letters. There are also 10 numbers (0 through 9). To avoid confusion and copying errors, Satoshi removed 4 commonly mistaken characters from the address generation process: uppercase letter 'O' and number '0,' uppercase letter 'I' and lowercase letter 'l.'

## Ψηφιακά Κλειδιά
Ένα μαθηματικά συσχετισμένο ζεύγος δημόσιου-ιδιωτικού κλειδιού, που δημιουργείται χρησιμοποιώντας τον Αλγόριθμο Ψηφιακής Υπογραφής Ελλειπτικής Καμπύλης (ECDSA):
1. **Ιδιωτικό κλειδί (Privkey):** Είναι ουσιαστικά ένας τυχαία δημιουργημένος αριθμός που πρέπει να παραμένει μυστικός. Χρησιμοποιείται για τη δημιουργία ψηφιακών υπογραφών και για την επιβεβαίωση ιδιοκτησίας, εξουσιοδοτώντας τη δαπάνη bitcoin.
2. **Δημόσιο κλειδί (Pubkey):** Δημιουργείται από το ιδιωτικό κλειδί χρησιμοποιώντας τη διαδικασία πολλαπλασιασμού ελλειπτικής καμπύλης. Κατά την δαπάνη και τη λήψη, το δημόσιο κλειδί αναπαρίσταται από μια διεύθυνση bitcoin.
   - "Σκεφτείτε το δημόσιο κλειδί ως παρόμοιο με έναν αριθμό τραπεζικού λογαριασμού και το ιδιωτικό κλειδί ως παρόμοιο με το μυστικό PIN ή την υπογραφή σε μια επιταγή, που παρέχει έλεγχο στον λογαριασμό."
3. **Διεύθυνση Bitcoin:** Μια διεύθυνση είναι ένας μοναδικός αναγνωριστικός κωδικός για τον προορισμό μιας πληρωμής bitcoin, που δημιουργείται και αντιστοιχεί σε ένα δημόσιο κλειδί ή σενάριο.
   - Συνήθως δημιουργείται εφαρμόζοντας τις συναρτήσεις κατακερματισμού SHA-256 και RIPEMD-160 σε σειρά, στο δημόσιο κλειδί.
   - Αυτές οι διευθύνσεις κωδικοποιούνται χρησιμοποιώντας την κωδικοποίηση Base58, η οποία αναπαριστά μια διεύθυνση σε μια μορφή 58 αλφαριθμητικών χαρακτήρων που είναι αναγνώσιμη από τον άνθρωπο.
   - Διασκεδαστικό γεγονός: Υπάρχουν 52 χαρακτήρες στο αλφάβητο, αν συμπεριλάβουμε όλα τα κεφαλαία και πεζά γράμματα. Υπάρχουν επίσης 10 αριθμοί (0 έως 9). Για να αποφευχθεί η σύγχυση και τα λάθη αντιγραφής, ο Satoshi αφαίρεσε 4 συνήθως συγκεχυμένους χαρακτήρες από τη διαδικασία δημιουργίας διευθύνσεων: το κεφαλαίο γράμμα 'O' και τον αριθμό '0,' το κεφαλαίο γράμμα 'I' και το πεζό γράμμα 'l.'

## Hash Functions
- A cryptographic hash function transforms data into a fixed-size digest, verifying data integrity. Any change in the input data results in a completely different hash output.
- Cryptographic hash functions are crucial in Bitcoin for verifying transaction integrity, securing bitcoin addresses, and in the Proof-of-Work (PoW) mining process.
- Bitcoin uses the SHA-256 hash function, generating a 256-bit (32-byte) output.
- Hash functions ensure block integrity and establish the chronological order of the blockchain by referencing the hash of the previous block.
- Key properties of hash functions:
  - Same input always produces the same hash.
  - Slight changes in input generate a completely different hash.
  - Hash collisions (different inputs generating the same hash) should not occur.
  - Hashes are difficult to reverse-engineer, enhancing security for commitment schemes.

## Συναρτήσεις Κατακερματισμού
- Μια κρυπτογραφική συνάρτηση κατακερματισμού μετατρέπει τα δεδομένα σε ένα σταθερού μεγέθους σύνολο, επιβεβαιώνοντας την ακεραιότητα των δεδομένων. Οποιαδήποτε αλλαγή στα εισερχόμενα δεδομένα έχει ως αποτέλεσμα ένα εντελώς διαφορετικό κατακερματισμό εξόδου.
- Οι κρυπτογραφικές συναρτήσεις κατακερματισμού είναι κρίσιμες στο Bitcoin για την επαλήθευση της ακεραιότητας των συναλλαγών, την ασφάλεια των διευθύνσεων bitcoin και στη διαδικασία εξόρυξης Proof-of-Work (PoW).
- Το Bitcoin χρησιμοποιεί τη συνάρτηση κατακερματισμού SHA-256, η οποία παράγει ένα σύνολο εξόδου 256-bit (32-byte).
- Οι συναρτήσεις κατακερματισμού εξασφαλίζουν την ακεραιότητα των μπλοκ και καθορίζουν τη χρονολογική σειρά του blockchain αναφέροντας τον κατακερματισμό του προηγούμενου μπλοκ.
- Κύρια χαρακτηριστικά των συναρτήσεων κατακερματισμού:
  - Το ίδιο εισερχόμενο πάντα παράγει τον ίδιο κατακερματισμό.
  - Ελαφρές αλλαγές στα εισερχόμενα παράγουν έναν εντελώς διαφορετικό κατακερματισμό.
  - Οι συγκρούσεις κατακερματισμού (διαφορετικά εισερχόμενα που παράγουν τον ίδιο κατακερματισμό) δεν πρέπει να συμβαίνουν.
  - Οι κατακερματισμοί είναι δύσκολο να αντιστραφούν, ενισχύοντας την ασφάλεια για τα σχήματα δέσμευσης.

## Public Key Cryptography
Public key cryptography, also known as asymmetric cryptography, is used in Bitcoin primarily for digital signatures, not for encrypting transaction data (since transaction details are publicly visible on the blockchain).
- Public key cryptography operates as a two key system:
  - The public key is used to encrypt a message.
  - The private key is used decrypt the message.
- Asymmetric encryption means the public key can be easily derived from the private key, but the private key is nearly impossible to derive from the public key.
- In Bitcoin, the Elliptic Curve Digital Signature Algorithm (ECDSA) is used to generate digital signatures that authenticate transactions, ensuring that only the holder of the private key can authorize the spending of Bitcoin.
  - The private key signs the transaction, authorizing the spending of Bitcoin.
  - The public key (revealed after spending) verifies the transaction's authenticity.

## Δημόσια Κλειδαριζόμενη Κρυπτογραφία
Η δημόσια κλειδαριζόμενη κρυπτογραφία, γνωστή και ως ασύμμετρη κρυπτογραφία, χρησιμοποιείται κυρίως στο Bitcoin για ψηφιακές υπογραφές και όχι για την κρυπτογράφηση δεδομένων συναλλαγών (καθώς οι λεπτομέρειες των συναλλαγών είναι δημόσια ορατές στο blockchain).
- Η δημόσια κλειδαριζόμενη κρυπτογραφία λειτουργεί ως σύστημα δύο κλειδιών:
  - Το δημόσιο κλειδί χρησιμοποιείται για την κρυπτογράφηση ενός μηνύματος.
  - Το ιδιωτικό κλειδί χρησιμοποιείται για την αποκρυπτογράφηση του μηνύματος.
- Η ασύμμετρη κρυπτογράφηση σημαίνει ότι το δημόσιο κλειδί μπορεί να προκύψει εύκολα από το ιδιωτικό κλειδί, αλλά το ιδιωτικό κλειδί είναι σχεδόν αδύνατο να προκύψει από το δημόσιο κλειδί.
- Στο Bitcoin, ο Αλγόριθμος Ψηφιακής Υπογραφής Ελλειπτικής Καμπύλης (ECDSA) χρησιμοποιείται για τη δημιουργία ψηφιακών υπογραφών που αυθεντικοποιούν τις συναλλαγές, διασφαλίζοντας ότι μόνο ο κάτοχος του ιδιωτικού κλειδιού μπορεί να εξουσιοδοτήσει την δαπάνη των Bitcoin.
  - Το ιδιωτικό κλειδί υπογράφει τη συναλλαγή, εξουσιοδοτώντας τη δαπάνη των Bitcoin.
  - Το δημόσιο κλειδί (που αποκαλύπτεται μετά τη δαπάνη) επαληθεύει τη γνησιότητα της συναλλαγής.

### Digital Signatures
Digital signatures are used to authenticate Bitcoin transactions by ensuring only the owner of the private key can authorize spending.
- When making a Bitcoin payment, a transaction (T) is constructed, and a subset (M) of the transaction data is signed using the private key, generating values R and S.
- To verify the transaction, the public key (Kpub) and the signature are used to calculate a point (P) on the elliptic curve. If the x-coordinate of P equals R, the signature is valid without revealing the private key.
- Each transaction transfers bitcoin from the current owner's address to the new owner’s address, authorized by a digital signature.
- The Bitcoin network tracks the entire transaction history, allowing anyone to verify ownership of bitcoin without access to private keys.
- Bitcoin wallets store the private-public key pairs, which are used to access and manage funds, though the wallet itself does not contain any actual bitcoin.

### Ψηφιακές Υπογραφές
Οι ψηφιακές υπογραφές χρησιμοποιούνται για την αυθεντικοποίηση των συναλλαγών Bitcoin διασφαλίζοντας ότι μόνο ο κάτοχος του ιδιωτικού κλειδιού μπορεί να εξουσιοδοτήσει τη δαπάνη.
- Όταν πραγματοποιείται μια πληρωμή Bitcoin, δημιουργείται μια συναλλαγή (T) και ένα υποσύνολο (M) των δεδομένων της συναλλαγής υπογράφεται χρησιμοποιώντας το ιδιωτικό κλειδί, παράγοντας τις τιμές R και S.
- Για την επαλήθευση της συναλλαγής, το δημόσιο κλειδί (Kpub) και η υπογραφή χρησιμοποιούνται για τον υπολογισμό ενός σημείου (P) στην ελλειπτική καμπύλη. Αν η συντεταγμένη x του P ισούται με R, η υπογραφή είναι έγκυρη χωρίς να αποκαλύπτεται το ιδιωτικό κλειδί.
- Κάθε συναλλαγή μεταφέρει bitcoin από τη διεύθυνση του τρέχοντος κατόχου στη διεύθυνση του νέου κατόχου, εξουσιοδοτημένη από μια ψηφιακή υπογραφή.
- Το δίκτυο Bitcoin παρακολουθεί όλο το ιστορικό συναλλαγών, επιτρέποντας σε οποιονδήποτε να επαληθεύσει την ιδιοκτησία των bitcoin χωρίς πρόσβαση στα ιδιωτικά κλειδιά.
- Τα πορτοφόλια Bitcoin αποθηκεύουν τα ζεύγη ιδιωτικών-δημόσιων κλειδιών, τα οποία χρησιμοποιούνται για την πρόσβαση και τη διαχείριση κεφαλαίων, αν και το ίδιο το πορτοφόλι δεν περιέχει κανένα πραγματικό bitcoin.

