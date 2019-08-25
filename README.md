# Shared Secret Repository

This git repo holds encrypted secret tokens for varies services in development by my self. 

All secrets are stored in `pass` encrypted files. 

## Scope

The secrets are consumed by the lightweight services I built for varies purposes to make life easier/harder,
qualification principle is simple:

  * has expiry date less than 6 month
  * rotates at most every 3 month
  * randomly generated and lenghthy (16+ chars)
  * is not production ready
  * is not shared with any 3rd-party entities
  

## Concerns

The Owner of this repo is aware of:

  * This repo is open to the world, everyone with/wihout an account can access this repo at any time
  * Though encrypted, metadata still adds entropy
  * `enc-algo` chosen today may become weak at any point in the future

## Metadata obfuscation, e.g. git-remote-gcrypt

The owner of this repo believes in openness, and signed to accept the risk of the leaked entropy introduced by the metadata.
