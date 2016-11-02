# EPM

[![Join the chat at https://gitter.im/ethpm/Lobby](https://badges.gitter.im/ethpm/Lobby.svg)](https://gitter.im/ethpm/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Ethereum Packaging Specification


## Use Cases

The following use cases were used to guide the specification.

1. Code with zero deployed instances.
    1. Reusable base contracts.
2. Code with one or more addresses.
    1. Libraries: Installation of the package involves having an importable interface for the library and linking against the proper address during deployment.
    2. Contracts: Installation of the package involves having an importable interface and some manner of templating in the proper addresses into the local source code prior to compilation as well as other non-contract code that may interact with the installed contract.


It is worth pointing out that the *Library* and *Contract* use cases are functionally the same.  Once [Solidity issue #242](https://github.com/ethereum/solidity/issues/242) has been addressed this distinction may no longer need to exist.
