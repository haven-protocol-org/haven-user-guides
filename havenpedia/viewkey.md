---
terms: ["view-key", "view-keys"]
summary: "one of two sets of private and public cryptographic keys that each account has, with the private view key required to view all transactions related to the account"
---

### The Basics

One of two sets of private and public cryptographic keys that each account has, with the private view key required to view all transactions related to the account.

Haven features an opaque blockchain (with an explicit allowance system called the @view-key), in sharp contrast with transparent blockchains used by any other cryptocurrency not based on CryptoNote. Thus, Haven is said to be "private, optionally transparent".

Every Haven address has a private viewkey which can be shared.  By sharing a viewkey, a person is allowing access to view every incoming transaction for that address.  However, outgoing transactions cannot be reliably viewed as of June 2017. Therefore, the balance of a Haven address as shown via a viewkey should not be relied upon.
