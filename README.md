## Description
This project is a private messaging application written entirely in Java, developed for personal and educational purposes with the goal of experimenting with basic cybersecurity and secure communication concepts.
The software allows users to create temporary private rooms, each with a predefined lifetime. Access to a room is only possible by knowing the unique code generated at the moment of its creation, making communication sessions ephemeral by design.
Several features were intentionally never fully implemented or deeply refined, such as an advanced administrative console, extensive message customization, or flexible room lifetime configuration. The project was never intended for production use, but rather as a controlled learning environment to explore networking, cryptography, and basic defensive strategies.
The application has never been tested in a real deployment, as it requires an SSL socket configuration. For cryptographic purposes, it relies on a self-signed certificate, suitable for experimentation but not for real-world secure systems.
The entire codebase is written and commented in Italian, reflecting its didactic and personal nature.


## Security and Cryptography Overview:
The application implements a basic secure communication model based on well-known cryptographic primitives:

  - Diffie–Hellman key exchange to securely establish a shared secret between peers.

  - Derivation of a 256-bit AES key from the shared secret.

  - Message encryption using AES-256 in GCM mode, providing confidentiality and authentication.

  - Communication over SSL sockets using a self-signed certificate.


## Features
The project includes a combination of implemented features and conceptual prototypes, designed to explore security-related ideas rather than user experience.
Note that some additional features were planned but left incomplete, as the primary focus of the project was conceptual experimentation.

  - Creation of temporary private rooms with limited lifetime.

  - Access control through unique room codes.

  - Encrypted messaging via AES-256-GCM.

  - Generation of occasional fake messages to simulate a constant and misleading information flow.

  - Message padding to enforce a fixed encrypted message length, mitigating basic traffic analysis.

  - Elementary checks aimed at detecting or mitigating simple DoS-like behaviors.


## Disclaimer
This software:

  - Is not production-ready.

  - Has never undergone a security audit.

  - Uses self-signed certificates.

  - Was developed exclusively for educational purposes.

  - It should not be used in real-world scenarios where security, privacy, or reliability are critical.


## License
This project is licensed under the [GNU GPL v3.0](./LICENSE).


## Social media
Huge thanks to all future supporters and bug reporters!
Feel free to check out my social links:

https://x.com/TommonPavou (X)

https://modrinth.com/user/TommonPavou (Modrinth)

https://www.instagram.com/tommonpavou_official/ (Instagram)
