The idea of a decentralized QSL exchange system.

Paper QSLs are still a way to confirm QSOs. The main idea is to organize a system similar to paper QSLs, but in electronic form. 
Now some hams are using FREE HamTools by PA4R software, which allows sending QSL images to e-mail addresses published in callbooks, e.g. qrz.com.
However, these QSL images are virtually impossible to verify.

The main requirements for a QSL system are
  1. no need for central servers
  2. independence from political structures
  3. protection of the QSL against falsification (authenticity verification)
  4. use existing technologies for transport and storage of QSLs
  5. Possibility of automated QSL processing

Possible solutions.

The basic idea -- use as electronic QSL combination of QSL card image (not a mandatory element, but a person usually arouses positive emotions beautiful image) and a string in ADIF format with QSO data. 
Next in order:
1. follows the following points
2. protects QSL elements from falsification: electronic signature, for example, with the help of PGP algorithms (existing proven technology). This means that each element is signed with the private key of the sender.
3. QSL delivery method: e-mail (existing proven technology)
4. automatic QSL processing: verification of received QSL elements by published electronic key, processing of ADIF strings - all these are algorithmizable actions.

To realize the above points, it is necessary to
1. organizing the storage of public keys in callbooks, similar to the storage of email addresses there
2. software development of a specialized mail client that will allow
   a. receive e-mails with QSL elements
   b. Receive public keys associated with callsigns from callbooks
   c. store a call sign database (address book) containing e-mail addresses and public keys
   d. Verify the electronic signature of received QSL elements with the available public keys
   e. Export verified QSLs to logging software. Verify that received QSLs match the log -- a function of the logging software.
   f. Generating and exporting (or e-mailing) a award application, which is a file of the application itself (format to be specified) and an attached set of QSLs in the form of previously received ADIF strings with corresponding electronic signature files.
4. development of a award manager software, which should allow
   a. import (receive by e-mail) the award application with the attached set of QSLs in the form of ADIF strings and electronic signatures on them
   b. receive public keys associated with call signs from callbooks
   c. Store a call sign database (address book) containing e-mail addresses and public keys.
   d. verify the electronic signature of received QSL elements with the available public keys
   e. verify the award conditions according to the QSL data received with the application and make a decision on the result of the award conditions fulfillment
   f. export of necessary data for diploma creation (printing, electronic version, etc.).


Disadvantages of this system:
1. an agreement with callbook server owners is required to store additional data
2. development of software and data formats is required
3. the need to coordinate with the authors of hardware log software formats for storing and importing the original QSL (received parts and electronic signatures to them)
4. the need to manually form and send applications for diplomas.However, at unification of the file format describing the conditions of diploma program execution it will be possible to do it automatically.
5. the need to be responsible for your data (public and private keys, QSL, logbook, etc.).

The advantages of this system are
1. independence from centralized services that are subject to hacking (see LoTW) and politics (see eQSL and hamlog.online).
2. Use of existing technologies that have proven themselves over time (e-mail, electronic signature).

