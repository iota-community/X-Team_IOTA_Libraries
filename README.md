<p align="center">
  <br>
  <a href="https://www.iota.org">
    <img src="https://images.ctfassets.net/xit7f234flxz/2UaYq5cR53ANDAKRT4HYWT/a4d962d037954adef7d0aa9a2e944a26/iota-small-logo.png"/>
  </a>
</p>

<h1 align="center"><a href="https://www.iota.org"> IOTA Libraries Initiative</a></h1>

<p align="center">The IOTA Libraries Initiative is aimed to provide help, guidance, and spotlight to the IOTA Developer Community.</p>

<p align="center">
  <a title="MIT License" href="LICENSE">
    <img src="https://img.shields.io/github/license/gridsome/gridsome.svg?style=flat-square&label=License&colorB=6cc24a">
  </a>
  <a title="Follow on Twitter" href="https://twitter.com/iotatoken">
    <img src="https://img.shields.io/twitter/follow/iotatoken.svg?style=social&label=Follow%20@iotatoken">
  </a>
  <br>
  <br>
</p>


## 🌳 IOTA Libraries Initiative

The **IOTA Libraries Initiative** is a collaborative effort to help people in the IOTA Community by introducing consistent workflows around the IOTA Libraries with content, and open source contributions.

### Chrysalis updates
Due to the switch to binary, the new transaction/message format, deprecation of bundles and re-usable addresses it makes little sense to keep building on top of the old libraries
Chrysalis and Coordicide allow us to start from scratch and now we can work together to understand how we can take advantage of this situation to address previously mentioned pain points.

### The new higher level client libraries

- A new client library that uses the same API, naming, abstractions and functionalities in all supported languages
One source of truth, a main implementation in Rust with bindings to other languages
- Sensible defaults, everything that can be optional will be optional
- No specific knowledge required; You don’t need to know all the details about IOTA to work with it due to the smart defaults
- The technical details are covered in the lower level libs, it's an abstraction layer

### New features
- Built-in support for node quorum and auto-setting node information inspired by Trinity
- No more manual byte/tryte conversions, UTF-8 by default instead of ASCII
- Easy to use and understandable features with the least amount of configuration needed for the majority of the use-cases
- “Trapdoors” for use-cases where you do need to have something non-standard.
- Pluggable signers instead of seeds possible
- It’s not final yet, waiting for final details on how transactions will look

### Example
Old:

```
api = Iota(adapter='https://nodes.comnet.thetangle.org:443')
msg = TryteString.from_unicode(‘Hey There!’)
addr = Address(‘ADDRESS999...’)
tx = ProposedTransaction(message=msg, address=addr, value=0)
api.send_transfer(transfers=[tx], min_weight_magnitude=10)
```

New:
```
api = IOTA(network=’comnet’)
api.send(‘ADDRESS999...’, message=’Hey There!’)
```

IOTA is an open-source distributed ledger technology that allows [connected devices](https://en.wikipedia.org/wiki/Connected_Devices) to transfer data and [IOTA tokens](https://docs.iota.org/docs/getting-started/0.1/clients/token) among each other for zero fees.

## 🎯 Initiative Goals

The IOTA Libraries will be the starting point for anyone and anything interacting with the IOTA network and are therefore important. It’s important to us that everyone can work with them regardless of how advanced a certain use case is or how simple it should be. That’s why we involve you in this early phase to help us shape these libraries into the most easy to use and most powerful libraries you can think of.
We are currently focused on improving the IOTA Experience around the following goals:

- Quality Assurance/Review
- Documentation
- Code samples development
- Improvements to module/libraries

### Quality Assurance/Review

Quality Assurance/Review goal includes making sure that the releases are easily usable, has no obvious bugs or pitfalls that might turn developers off from trying further once they run into them, make sure that the examples we provide are clear and work for the most common use cases the release is aimed at.

 > - [IOTA Libraries Feedback (A)](https://github.com/iota-community/X-Team-IOTALibraries/issues/1)
 > - [Provide feedback on the Wallet library draft (A)](https://github.com/iota-community/X-Team-IOTALibraries/issues/3)

### Documentation

Documentation goal includes everything related to writing, curating, and sharing content around with solid documentation at every launch, that is kept up-to-date, well-written explanations of tangible use cases to stimulate developer interest

> - [ ]
> - [ ]

### Code samples development

Code samples development goal includes Code examples and well-presented PoCs to kick start devs Create a list of RFP’s for the EDF to fund Open-Source development

> - [ ] [Define the list of the first programming languages to port the new libraries to (A)](https://github.com/iota-community/X-Team-IOTALibraries/issues/2)
> - [ ]

###  Improvements to module/libraries

Improvements to module/libraries goal includes Developer-friendly APIs at launch Solid comms both at release and after release (e.g. spotlight for community projects using each of libs)

> - [ ]
> - [ ]

## 🤔 How Can You Get Involved?

Show your interest by adding your information with an issue here on github and join the IOTA Experience Team on the [IOTA Discord](https://discord.iota.org).

## 👥 What to expect?

Meet with IOTA Foundation members to exchange ideas, give and receive feedback for the chosen goal(s).

This initiative is possible thanks to the contribution of the IOTA Community members and participants will be invited to participate in feedback collecting and evaluating sessions to further push the capabilities of the IOTA Experience Teams. 
