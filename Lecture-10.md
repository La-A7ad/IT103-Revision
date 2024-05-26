Here is a comprehensive Q&A question bank based on the thorough analysis of the "Lecture 10 - Network Security Introduction" PDF.

---

### Lecture 10 - Network Security Introduction

**Q1: What is the definition of security in a system, application, or protocol?**
<details>
<summary>Answer</summary>
Security of a system, application, or protocol is always relative to a set of desired properties and an adversary with specific capabilities. For example, standard file access permissions in Linux and Windows are not effective against an adversary who can boot from a CD.
</details>

**Q2: What are the three primary security goals?**
<details>
<summary>Answer</summary>
The three primary security goals are Integrity, Confidentiality, and Availability.
</details>

**Q3: What is confidentiality in the context of network security?**
<details>
<summary>Answer</summary>
Confidentiality is the avoidance of unauthorized disclosure of information. It involves protecting data, providing access for those allowed to see it while disallowing others from learning anything about its content.
</details>

**Q4: What is encryption and its purpose in confidentiality?**
<details>
<summary>Answer</summary>
Encryption is the transformation of information using a secret called an encryption key, so that the transformed information can only be read using another secret called the decryption key.
</details>

**Q5: What is access control in network security?**
<details>
<summary>Answer</summary>
Access control refers to the rules and policies that limit access to confidential information to those people and/or systems with a “need to know,” determined by identity or role.
</details>

**Q6: What are the three common methods of authentication?**
<details>
<summary>Answer</summary>
The three common methods of authentication are: something the person has (e.g., smart card), something the person knows (e.g., password), and something the person is (e.g., fingerprint).
</details>

**Q7: What is the role of authorization in confidentiality?**
<details>
<summary>Answer</summary>
Authorization determines if a person or system is allowed access to resources based on an access control policy, preventing attackers from gaining unauthorized access.
</details>

**Q8: What is the importance of physical security in network security?**
<details>
<summary>Answer</summary>
Physical security establishes physical barriers to limit access to protected resources, including locks, windowless rooms, sound-dampening materials, and Faraday cages.
</details>

**Q9: Define integrity in the context of network security.**
<details>
<summary>Answer</summary>
Integrity is the property that information has not been altered in an unauthorized way.
</details>

**Q10: What are some tools used to ensure data integrity?**
<details>
<summary>Answer</summary>
Tools for ensuring data integrity include backups, checksums, and data correcting codes.
</details>

**Q11: What is availability in network security?**
<details>
<summary>Answer</summary>
Availability is the property that information is accessible and modifiable in a timely fashion by those authorized to do so.
</details>

**Q12: What are some tools used to ensure availability?**
<details>
<summary>Answer</summary>
Tools for ensuring availability include physical protections and computational redundancies.
</details>

**Q13: What does AAA stand for in network security concepts?**
<details>
<summary>Answer</summary>
AAA stands for Authenticity, Anonymity, and Assurance.
</details>

**Q14: What is assurance in the context of network security?**
<details>
<summary>Answer</summary>
Assurance refers to how trust is provided and managed in computer systems, depending on policies, permissions, and protections.
</details>

**Q15: What is authenticity and its primary tool?**
<details>
<summary>Answer</summary>
Authenticity is the ability to determine that statements, policies, and permissions issued by persons or systems are genuine. The primary tool for authenticity is digital signatures.
</details>

**Q16: What is anonymity in network security, and what are some tools to achieve it?**
<details>
<summary>Answer</summary>
Anonymity is the property that certain records or transactions are not attributable to any individual. Tools to achieve anonymity include aggregation, mixing, proxies, and pseudonyms.
</details>

**Q17: Define eavesdropping in the context of network threats and attacks.**
<details>
<summary>Answer</summary>
Eavesdropping is the interception of information intended for someone else during its transmission over a communication channel.
</details>

**Q18: What is alteration as a network threat?**
<details>
<summary>Answer</summary>
Alteration is the unauthorized modification of information, exemplified by a man-in-the-middle attack.
</details>

**Q19: What is a denial-of-service attack?**
<details>
<summary>Answer</summary>
Denial-of-service (DoS) is the interruption or degradation of a data service or information access, such as email spam filling up a mail queue.
</details>

**Q20: What does masquerading mean in network security?**
<details>
<summary>Answer</summary>
Masquerading is the fabrication of information that is purported to be from someone who is not the actual author.
</details>

**Q21: What is repudiation in the context of network threats?**
<details>
<summary>Answer</summary>
Repudiation is the denial of a commitment or data receipt, involving an attempt to back out of a contract or protocol.
</details>

**Q22: What is correlation and traceback in network security?**
<details>
<summary>Answer</summary>
Correlation and traceback involve integrating multiple data sources to determine the source of a particular data stream or piece of information.
</details>

**Q23: What is the principle of economy of mechanism?**
<details>
<summary>Answer</summary>
Economy of mechanism stresses simplicity in the design and implementation of security measures, facilitating understanding and verification.
</details>

**Q24: What does the principle of fail-safe defaults state?**
<details>
<summary>Answer</summary>
The principle of fail-safe defaults states that the default configuration of a system should have a conservative protection scheme, providing minimal access rights by default.
</details>

**Q25: Explain the principle of complete mediation.**
<details>
<summary>Answer</summary>
Complete mediation requires that every access to a resource must be checked for compliance with a protection scheme, ensuring that permissions are current and valid.
</details>

**Q26: What is the principle of open design in security?**
<details>
<summary>Answer</summary>
Open design states that the security architecture and design of a system should be publicly available, relying on keeping cryptographic keys secret, not the design itself.
</details>

**Q27: Describe the principle of separation of privilege.**
<details>
<summary>Answer</summary>
Separation of privilege dictates that multiple conditions should be required to achieve access to restricted resources or perform certain actions.
</details>

**Q28: What is the least privilege principle in network security?**
<details>
<summary>Answer</summary>
The least privilege principle states that each program and user should operate with the minimum privileges necessary to function, reducing potential damage from security breaches.
</details>

**Q29: What does the least common mechanism principle entail?**
<details>
<summary>Answer</summary>
The least common mechanism principle entails minimizing mechanisms that allow resource sharing among users to prevent security problems.
</details>

**Q30: Explain the principle of psychological acceptability.**
<details>
<summary>Answer</summary>
Psychological acceptability states that user interfaces should be well designed and intuitive, with security settings adhering to user expectations.
</details>

**Q31: What is the work factor principle in network security?**
<details>
<summary>Answer</summary>
The work factor principle compares the cost of circumventing a security mechanism with the attacker's resources, ensuring appropriate security measures.
</details>

**Q32: What does the principle of compromise recording state?**
<details>
<summary>Answer</summary>
Compromise recording states that sometimes it is more desirable to record the details of an intrusion than to prevent it, using systems like internet-connected surveillance cameras.
</details>

**Q33: What are access control matrices?**
<details>
<summary>Answer</summary>
Access control matrices are tables defining permissions, with rows associated with subjects (users, groups, systems) and columns associated with objects (files, directories, devices), and cells indicating access rights.
</details>

**Q34: What are access control lists (ACLs)?**
<details>
<summary>Answer</summary>
Access control lists (ACLs) define, for each object, a list enumerating all the subjects with access rights to the object and specifying their permissions.
</details>

**Q35: What are capabilities in access control?**
<details>
<summary>Answer</summary>
Capabilities take a subject-centered approach to access control, defining the list of objects a subject has access to and the specific rights for each object.
</details>

**Q36: What is role-based access control (RBAC)?**
<details>
<summary>Answer</summary>
Role-based access control (RBAC) defines roles and specifies access control rights for these roles, rather than for individual subjects directly.
</details>

**Q37: What is the purpose of encryption in cryptographic concepts?**
<details>
<summary>Answer</summary>
Encryption allows two parties, typically called Alice and Bob, to establish confidential communication over an insecure channel subject to eavesdropping.
</details>

**Q38: How does the Caesar Cipher work?**
<details>
<summary>Answer</summary>
The Caesar Cipher replaces each letter

 with the one "three over" in the alphabet.
</details>

**Q39: What are symmetric cryptosystems?**
<details>
<summary>Answer</summary>
Symmetric cryptosystems use a shared secret key for both encryption and decryption.
</details>

**Q40: What is public-key cryptography?**
<details>
<summary>Answer</summary>
Public-key cryptography uses separate keys for encryption and decryption, with a public key for encryption and a private key for decryption.
</details>

**Q41: What are digital signatures in cryptography?**
<details>
<summary>Answer</summary>
Digital signatures use public-key encryption to sign a message, ensuring authenticity and nonrepudiation.
</details>

**Q42: What are cryptographic hash functions and their properties?**
<details>
<summary>Answer</summary>
Cryptographic hash functions are checksums on a message with properties of being one-way (easy to compute, hard to reverse) and collision-resistant (hard to find two messages with the same hash).
</details>

**Q43: What are message authentication codes (MACs)?**
<details>
<summary>Answer</summary>
Message authentication codes (MACs) allow for data integrity if the communicating parties share a secret key, by computing a hash of the message and the secret key.
</details>

**Q44: What are digital certificates?**
<details>
<summary>Answer</summary>
Digital certificates are digitally signed bindings between an identity and a public key, issued by a certificate authority (CA).
</details>

**Q45: How are passwords used in network security?**
<details>
<summary>Answer</summary>
Passwords are short sequences of characters used for authentication by proving knowledge of a secret.
</details>

**Q46: What makes a password strong?**
<details>
<summary>Answer</summary>
A strong password includes UPPER/lower case characters, special characters, and numbers.
</details>

**Q47: What are the considerations for password complexity and length?**
<details>
<summary>Answer</summary>
Password complexity involves using a combination of numbers, UPPER/lower case characters, and special characters. Password length increases the number of possible combinations, making it harder to crack.
</details>

**Q48: What is social engineering in the context of network security?**
<details>
<summary>Answer</summary>
Social engineering involves techniques like pretexting, baiting, and quid pro quo to trick individuals into revealing confidential information or performing insecure actions.
</details>

---

This question bank covers all the key points from the lecture and includes detailed questions and answers to help in thoroughly understanding the material.
