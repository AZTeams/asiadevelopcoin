AsiaDevelopCoin Core integration/staging tree
=====================================



What is AsiaDevelopCoin?
-------------------

AsiaDevelopCoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. AsiaDevelopCoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. AsiaDevelopCoin Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the AsiaDevelopCoin Core software.

License
-------

AsiaDevelopCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable.
regularly to indicate new official, stable release versions of AsiaDevelopCoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).



Specifications
--------------

<<<<<<< HEAD
Name: AsiaDevelopCoin
=======
Name: Asian Develop Coin
>>>>>>> 50dd2a9a990aab135c362f9763d18241575832d5

Ticker: ADC

PoW Algorithm: Scrypt

Block Reward: 5 ADC

Address letter: A

Multisig Address letter: 6

Maturity: 20 blocks

Difficulty Re-target: Every block

P2P Port: 31134

RPC Port: 31135

Total coin supply: 50 000 000



Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
