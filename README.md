Uwucoin integration/staging tree
================================

Just creating a memecoin for fun. Learned alot about the inner-workings on Crypto's origins creating this. Definetly a super fun project. The full nodes/DNS Seeders are currently off, but they are running on DigitalOcean's IaaS droplets (Ubuntu 16.04). 

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2021-2021 UWUcoin Developers


What is Uwucoin?
----------------

Uwucoin is a fork of Litecoin  using scrypt as a proof-of-work algorithm.
 - 2.00 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Bitcoin.
 - 50 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Uwucoin client sofware, see http://www.uwucoin.org.

License
-------

Uwucoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test litecoin-qt.pro
    make -f Makefile.test
    ./uwucoin-qt_test

# uwucoin
