# Cryptographic Hash Functions

Hash function accepts any length of data as an input and outputs fixed length data.

A Hash is a one-way mathematical function that is easy to calculate and very hard (nearly impossible) to reverse. It maps an input to an output.
While the calculation of the hash of a string with a cryptographic hash function is very fast, the reverse calculation is very complex and massively time-consuming.

SHA-256 is a hash function. It is considered as one of the most secured hashing algorithms. Three properties make SHA-256 this secure.

1. It is almost impossible to reconstruct the initial data from the hash value. A brute-force attack would need to make 2^256 attempts to generate the initial data.

2. Having two messages with the same hash value is extremely unlikely. With 2^256 possible hash values the likelihood of two being the same is infinitesimally small. (No collisions)

3. A minor change to the original data alters the hash value so much that it's not apparent the new hash value is derived from similar data. (Avalanche effect)

SHA-256 algorithm outputs a value that is 256 bits long for any given string. That is 64 digits long hexadecimal number. That output is looks like this, "5960926e848963182987de03af6f09bfc90ac76de090a67f76960d4f601f1c53".

Use cases of SHA-256:

- Blockchain
- Bitcoin
- SSL (Secure Sockets Layer) Certificates
