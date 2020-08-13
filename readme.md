# ca-helpers

A small set of helpers as I try to create a root ca for each project I'm working on.

## Usage

### Creating your root ca

Usage: `./ca-become -c CA_FOR_SIGNING`

You'll have to add the root ca to your trust store

### Creating your signed certificates

Usage: `./ca-sign -d DOMAIN -c CA_FOR_SIGNING [ -a ALTERNATIVE_DOMAIN ]`

DOMAIN: the domain you want to sign the certificate for
ALTERNATIVE_DOMAIN: an optional second alternative domain for the certificate
CA_FOR_SIGNING: The CA_FOR_SIGNING you have used for creating your root ca