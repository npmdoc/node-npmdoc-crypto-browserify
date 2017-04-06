# api documentation for  [crypto-browserify (v3.11.0)](https://github.com/crypto-browserify/crypto-browserify)  [![npm package](https://img.shields.io/npm/v/npmdoc-crypto-browserify.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-crypto-browserify) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-crypto-browserify.svg)](https://travis-ci.org/npmdoc/node-npmdoc-crypto-browserify)
#### implementation of crypto for the browser

[![NPM](https://nodei.co/npm/crypto-browserify.png?downloads=true)](https://www.npmjs.com/package/crypto-browserify)

[![apidoc](https://npmdoc.github.io/node-npmdoc-crypto-browserify/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-crypto-browserify_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-crypto-browserify/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-crypto-browserify/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-crypto-browserify/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dominic Tarr",
        "email": "dominic.tarr@gmail.com",
        "url": "dominictarr.com"
    },
    "browser": {
        "crypto": false
    },
    "bugs": {
        "url": "https://github.com/crypto-browserify/crypto-browserify/issues"
    },
    "dependencies": {
        "browserify-cipher": "^1.0.0",
        "browserify-sign": "^4.0.0",
        "create-ecdh": "^4.0.0",
        "create-hash": "^1.1.0",
        "create-hmac": "^1.1.0",
        "diffie-hellman": "^5.0.0",
        "inherits": "^2.0.1",
        "pbkdf2": "^3.0.3",
        "public-encrypt": "^4.0.0",
        "randombytes": "^2.0.0"
    },
    "description": "implementation of crypto for the browser",
    "devDependencies": {
        "hash-test-vectors": "~1.3.2",
        "pseudorandombytes": "^2.0.0",
        "standard": "^5.0.2",
        "tape": "~2.3.2",
        "zuul": "^3.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "3652a0906ab9b2a7e0c3ce66a408e957a2485522",
        "tarball": "https://registry.npmjs.org/crypto-browserify/-/crypto-browserify-3.11.0.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "9fabcbd78209a99c7c624d1509d389b00e8d733f",
    "homepage": "https://github.com/crypto-browserify/crypto-browserify",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dominictarr",
            "email": "dominic.tarr@gmail.com"
        },
        {
            "name": "cwmma",
            "email": "calvin.metcalf@gmail.com"
        },
        {
            "name": "dcousens",
            "email": "email@dcousens.com"
        },
        {
            "name": "jprichardson",
            "email": "jprichardson@gmail.com"
        },
        {
            "name": "indutny",
            "email": "fedor@indutny.com"
        }
    ],
    "name": "crypto-browserify",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/crypto-browserify/crypto-browserify.git"
    },
    "scripts": {
        "browser": "zuul --browser-version $BROWSER_VERSION --browser-name $BROWSER_NAME -- test/index.js",
        "standard": "standard",
        "test": "npm run standard && npm run unit",
        "unit": "node test/"
    },
    "version": "3.11.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module crypto-browserify](#apidoc.module.crypto-browserify)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher (cipher, password, options)](#apidoc.element.crypto-browserify.Cipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher.super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Cipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipher (cipher, password, options)](#apidoc.element.crypto-browserify.Decipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Decipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.DiffieHellman)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.DiffieHellmanGroup)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Hash (algorithm, options)](#apidoc.element.crypto-browserify.Hash)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Hmac (hmac, key, options)](#apidoc.element.crypto-browserify.Hmac)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Sign (algorithm, options)](#apidoc.element.crypto-browserify.Sign)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Verify (algorithm, options)](#apidoc.element.crypto-browserify.Verify)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createCipher (cipher, password, options)](#apidoc.element.crypto-browserify.createCipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createCipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.createCipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createCredentials ()](#apidoc.element.crypto-browserify.createCredentials)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createDecipher (cipher, password, options)](#apidoc.element.crypto-browserify.createDecipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createDecipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.createDecipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.createDiffieHellman)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.createDiffieHellmanGroup)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createECDH (curve)](#apidoc.element.crypto-browserify.createECDH)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createHash (algorithm, options)](#apidoc.element.crypto-browserify.createHash)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createHmac (hmac, key, options)](#apidoc.element.crypto-browserify.createHmac)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createSign (algorithm, options)](#apidoc.element.crypto-browserify.createSign)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createVerify (algorithm, options)](#apidoc.element.crypto-browserify.createVerify)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>getCiphers ()](#apidoc.element.crypto-browserify.getCiphers)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>getDiffieHellman (name)](#apidoc.element.crypto-browserify.getDiffieHellman)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>getHashes ()](#apidoc.element.crypto-browserify.getHashes)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>listCiphers ()](#apidoc.element.crypto-browserify.listCiphers)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>pbkdf2 (password, salt, iterations, keylen, digest, callback)](#apidoc.element.crypto-browserify.pbkdf2)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>pbkdf2Sync (password, salt, iterations, keylen, digest)](#apidoc.element.crypto-browserify.pbkdf2Sync)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>privateDecrypt (options, buffer)](#apidoc.element.crypto-browserify.privateDecrypt)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>privateEncrypt (options, buffer)](#apidoc.element.crypto-browserify.privateEncrypt)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>prng ()](#apidoc.element.crypto-browserify.prng)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>pseudoRandomBytes ()](#apidoc.element.crypto-browserify.pseudoRandomBytes)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>publicDecrypt (options, buffer)](#apidoc.element.crypto-browserify.publicDecrypt)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>publicEncrypt (options, buffer)](#apidoc.element.crypto-browserify.publicEncrypt)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>randomBytes ()](#apidoc.element.crypto-browserify.randomBytes)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>rng ()](#apidoc.element.crypto-browserify.rng)
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Cipheriv.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Decipher.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Decipheriv.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellmanGroup.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Hash.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>Hmac.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellman.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>createSign.prototype
1.  object <span class="apidocSignatureSpan">crypto-browserify.</span>createVerify.prototype

#### [module crypto-browserify.Cipher](#apidoc.module.crypto-browserify.Cipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher (cipher, password, options)](#apidoc.element.crypto-browserify.Cipher.Cipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_)

#### [module crypto-browserify.Cipher.prototype](#apidoc.module.crypto-browserify.Cipher.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Cipher.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Cipher.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Cipher.prototype.final)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Cipher.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Cipher.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Cipher.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Cipher.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Cipher.prototype.update)

#### [module crypto-browserify.Cipher.super_](#apidoc.module.crypto-browserify.Cipher.super_)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_.super_)

#### [module crypto-browserify.Cipheriv](#apidoc.module.crypto-browserify.Cipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Cipheriv.Cipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipheriv.super_)

#### [module crypto-browserify.Cipheriv.prototype](#apidoc.module.crypto-browserify.Cipheriv.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Cipheriv.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Cipheriv.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Cipheriv.prototype.final)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Cipheriv.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Cipheriv.prototype.update)

#### [module crypto-browserify.Decipher](#apidoc.module.crypto-browserify.Decipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipher (cipher, password, options)](#apidoc.element.crypto-browserify.Decipher.Decipher)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Decipher.super_)

#### [module crypto-browserify.Decipher.prototype](#apidoc.module.crypto-browserify.Decipher.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Decipher.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Decipher.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.final)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>finaltol (outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.finaltol)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Decipher.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Decipher.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Decipher.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Decipher.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.update)

#### [module crypto-browserify.Decipheriv](#apidoc.module.crypto-browserify.Decipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Decipheriv.Decipheriv)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.</span>super_ (options)](#apidoc.element.crypto-browserify.Decipheriv.super_)

#### [module crypto-browserify.Decipheriv.prototype](#apidoc.module.crypto-browserify.Decipheriv.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Decipheriv.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Decipheriv.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.final)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>finaltol (outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.finaltol)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Decipheriv.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.update)

#### [module crypto-browserify.DiffieHellmanGroup](#apidoc.module.crypto-browserify.DiffieHellmanGroup)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.DiffieHellmanGroup)

#### [module crypto-browserify.DiffieHellmanGroup.prototype](#apidoc.module.crypto-browserify.DiffieHellmanGroup.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.computeSecret)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>generateKeys (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.generateKeys)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getGenerator (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getGenerator)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPrime (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrime)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPrivateKey (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrivateKey)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPublicKey (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPublicKey)

#### [module crypto-browserify.Hash](#apidoc.module.crypto-browserify.Hash)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Hash (algorithm, options)](#apidoc.element.crypto-browserify.Hash.Hash)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hash.</span>super_ (options)](#apidoc.element.crypto-browserify.Hash.super_)

#### [module crypto-browserify.Hash.prototype](#apidoc.module.crypto-browserify.Hash.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Hash.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Hash.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>digest (outputEncoding)](#apidoc.element.crypto-browserify.Hash.prototype.digest)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.Hash.prototype.update)

#### [module crypto-browserify.Hmac](#apidoc.module.crypto-browserify.Hmac)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>Hmac (hmac, key, options)](#apidoc.element.crypto-browserify.Hmac.Hmac)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hmac.</span>super_ (options)](#apidoc.element.crypto-browserify.Hmac.super_)

#### [module crypto-browserify.Hmac.prototype](#apidoc.module.crypto-browserify.Hmac.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Hmac.prototype._flush)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Hmac.prototype._transform)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>digest (outputEncoding)](#apidoc.element.crypto-browserify.Hmac.prototype.digest)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.Hmac.prototype.update)

#### [module crypto-browserify.createDiffieHellman](#apidoc.module.crypto-browserify.createDiffieHellman)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.createDiffieHellman.createDiffieHellman)

#### [module crypto-browserify.createDiffieHellman.prototype](#apidoc.module.crypto-browserify.createDiffieHellman.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.computeSecret)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.generateKeys)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getGenerator)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrime)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrivateKey)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPublicKey)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>setPrivateKey (key, encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPrivateKey)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>setPublicKey (key, encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPublicKey)

#### [module crypto-browserify.createSign](#apidoc.module.crypto-browserify.createSign)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createSign (algorithm, options)](#apidoc.element.crypto-browserify.createSign.createSign)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createSign.</span>super_ (options)](#apidoc.element.crypto-browserify.createSign.super_)

#### [module crypto-browserify.createSign.prototype](#apidoc.module.crypto-browserify.createSign.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.crypto-browserify.createSign.prototype._write)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>sign (options, encoding)](#apidoc.element.crypto-browserify.createSign.prototype.sign)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.createSign.prototype.update)

#### [module crypto-browserify.createVerify](#apidoc.module.crypto-browserify.createVerify)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.</span>createVerify (algorithm, options)](#apidoc.element.crypto-browserify.createVerify.createVerify)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createVerify.</span>super_ (options)](#apidoc.element.crypto-browserify.createVerify.super_)

#### [module crypto-browserify.createVerify.prototype](#apidoc.module.crypto-browserify.createVerify.prototype)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.crypto-browserify.createVerify.prototype._write)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.createVerify.prototype.update)
1.  [function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>verify (object, signature, sigEncoding)](#apidoc.element.crypto-browserify.createVerify.prototype.verify)



# <a name="apidoc.module.crypto-browserify"></a>[module crypto-browserify](#apidoc.module.crypto-browserify)

#### <a name="apidoc.element.crypto-browserify.Cipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher (cipher, password, options)](#apidoc.element.crypto-browserify.Cipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher.super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Cipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipher (cipher, password, options)](#apidoc.element.crypto-browserify.Decipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Decipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellman"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.DiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.DiffieHellmanGroup)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hash"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Hash (algorithm, options)](#apidoc.element.crypto-browserify.Hash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hmac"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Hmac (hmac, key, options)](#apidoc.element.crypto-browserify.Hmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Sign"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Sign (algorithm, options)](#apidoc.element.crypto-browserify.Sign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Verify"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Verify (algorithm, options)](#apidoc.element.crypto-browserify.Verify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createCipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createCipher (cipher, password, options)](#apidoc.element.crypto-browserify.createCipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createCipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createCipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.createCipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createCredentials"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createCredentials ()](#apidoc.element.crypto-browserify.createCredentials)
- description and source-code
```javascript
createCredentials = function () {
  throw new Error([
    'sorry, ' + name + ' is not implemented yet',
    'we accept pull requests',
    'https://github.com/crypto-browserify/crypto-browserify'
  ].join('\n'))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDecipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createDecipher (cipher, password, options)](#apidoc.element.crypto-browserify.createDecipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDecipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createDecipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.createDecipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.createDiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellmanGroup"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.createDiffieHellmanGroup)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createECDH"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createECDH (curve)](#apidoc.element.crypto-browserify.createECDH)
- description and source-code
```javascript
function createECDH(curve) {
  return new ECDH(curve);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createHash"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createHash (algorithm, options)](#apidoc.element.crypto-browserify.createHash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createHmac"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createHmac (hmac, key, options)](#apidoc.element.crypto-browserify.createHmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createSign"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createSign (algorithm, options)](#apidoc.element.crypto-browserify.createSign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createVerify"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createVerify (algorithm, options)](#apidoc.element.crypto-browserify.createVerify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.getCiphers"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>getCiphers ()](#apidoc.element.crypto-browserify.getCiphers)
- description and source-code
```javascript
() => {
  if (result === undefined)
    result = fn();
  return result.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.getDiffieHellman"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>getDiffieHellman (name)](#apidoc.element.crypto-browserify.getDiffieHellman)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.getHashes"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>getHashes ()](#apidoc.element.crypto-browserify.getHashes)
- description and source-code
```javascript
getHashes = function () {
  return hashes
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.listCiphers"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>listCiphers ()](#apidoc.element.crypto-browserify.listCiphers)
- description and source-code
```javascript
() => {
  if (result === undefined)
    result = fn();
  return result.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.pbkdf2"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>pbkdf2 (password, salt, iterations, keylen, digest, callback)](#apidoc.element.crypto-browserify.pbkdf2)
- description and source-code
```javascript
pbkdf2 = function (password, salt, iterations, keylen, digest, callback) {
  if (typeof digest === 'function') {
    callback = digest;
    digest = undefined;
    pbkdf2DeprecationWarning();
  }

  if (typeof callback !== 'function')
    throw new Error('No callback provided to pbkdf2');

  return pbkdf2(password, salt, iterations, keylen, digest, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.pbkdf2Sync"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>pbkdf2Sync (password, salt, iterations, keylen, digest)](#apidoc.element.crypto-browserify.pbkdf2Sync)
- description and source-code
```javascript
pbkdf2Sync = function (password, salt, iterations, keylen, digest) {
  if (typeof digest === 'undefined') {
    digest = undefined;
    pbkdf2DeprecationWarning();
  }
  return pbkdf2(password, salt, iterations, keylen, digest);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.privateDecrypt"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>privateDecrypt (options, buffer)](#apidoc.element.crypto-browserify.privateDecrypt)
- description and source-code
```javascript
privateDecrypt = function (options, buffer) {
  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var padding = options.padding || defaultPadding;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.privateEncrypt"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>privateEncrypt (options, buffer)](#apidoc.element.crypto-browserify.privateEncrypt)
- description and source-code
```javascript
privateEncrypt = function (options, buffer) {
  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var padding = options.padding || defaultPadding;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.prng"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>prng ()](#apidoc.element.crypto-browserify.prng)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.pseudoRandomBytes"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>pseudoRandomBytes ()](#apidoc.element.crypto-browserify.pseudoRandomBytes)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.publicDecrypt"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>publicDecrypt (options, buffer)](#apidoc.element.crypto-browserify.publicDecrypt)
- description and source-code
```javascript
publicDecrypt = function (options, buffer) {
  var key = options.key || options;
  var padding = options.padding || defaultPadding;
  var passphrase = options.passphrase || null;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.publicEncrypt"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>publicEncrypt (options, buffer)](#apidoc.element.crypto-browserify.publicEncrypt)
- description and source-code
```javascript
publicEncrypt = function (options, buffer) {
  var key = options.key || options;
  var padding = options.padding || defaultPadding;
  var passphrase = options.passphrase || null;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.randomBytes"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>randomBytes ()](#apidoc.element.crypto-browserify.randomBytes)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.rng"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>rng ()](#apidoc.element.crypto-browserify.rng)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Cipher"></a>[module crypto-browserify.Cipher](#apidoc.module.crypto-browserify.Cipher)

#### <a name="apidoc.element.crypto-browserify.Cipher.Cipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipher (cipher, password, options)](#apidoc.element.crypto-browserify.Cipher.Cipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Cipher.prototype"></a>[module crypto-browserify.Cipher.prototype](#apidoc.module.crypto-browserify.Cipher.prototype)

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Cipher.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Cipher.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.final"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Cipher.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Cipher.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Cipher.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Cipher.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Cipher.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipher.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Cipher.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Cipher.super_"></a>[module crypto-browserify.Cipher.super_](#apidoc.module.crypto-browserify.Cipher.super_)

#### <a name="apidoc.element.crypto-browserify.Cipher.super_.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipher.super_.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function')
      this._transform = options.transform;

    if (typeof options.flush === 'function')
      this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function() {
    if (typeof this._flush === 'function')
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Cipheriv"></a>[module crypto-browserify.Cipheriv](#apidoc.module.crypto-browserify.Cipheriv)

#### <a name="apidoc.element.crypto-browserify.Cipheriv.Cipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Cipheriv.Cipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.</span>super_ (options)](#apidoc.element.crypto-browserify.Cipheriv.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Cipheriv.prototype"></a>[module crypto-browserify.Cipheriv.prototype](#apidoc.module.crypto-browserify.Cipheriv.prototype)

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Cipheriv.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Cipheriv.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.final"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Cipheriv.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Cipheriv.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Cipheriv.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Cipheriv.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Cipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Cipheriv.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Decipher"></a>[module crypto-browserify.Decipher](#apidoc.module.crypto-browserify.Decipher)

#### <a name="apidoc.element.crypto-browserify.Decipher.Decipher"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipher (cipher, password, options)](#apidoc.element.crypto-browserify.Decipher.Decipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.</span>super_ (options)](#apidoc.element.crypto-browserify.Decipher.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Decipher.prototype"></a>[module crypto-browserify.Decipher.prototype](#apidoc.module.crypto-browserify.Decipher.prototype)

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Decipher.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Decipher.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.final"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.finaltol"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>finaltol (outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.finaltol)
- description and source-code
```javascript
finaltol = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Decipher.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Decipher.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Decipher.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Decipher.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipher.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Decipher.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Decipheriv"></a>[module crypto-browserify.Decipheriv](#apidoc.module.crypto-browserify.Decipheriv)

#### <a name="apidoc.element.crypto-browserify.Decipheriv.Decipheriv"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.crypto-browserify.Decipheriv.Decipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.</span>super_ (options)](#apidoc.element.crypto-browserify.Decipheriv.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Decipheriv.prototype"></a>[module crypto-browserify.Decipheriv.prototype](#apidoc.module.crypto-browserify.Decipheriv.prototype)

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Decipheriv.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Decipheriv.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.final"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.finaltol"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>finaltol (outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.finaltol)
- description and source-code
```javascript
finaltol = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>getAuthTag ()](#apidoc.element.crypto-browserify.Decipheriv.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.crypto-browserify.Decipheriv.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Decipheriv.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Decipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.crypto-browserify.Decipheriv.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.DiffieHellmanGroup"></a>[module crypto-browserify.DiffieHellmanGroup](#apidoc.module.crypto-browserify.DiffieHellmanGroup)

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.DiffieHellmanGroup"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>DiffieHellmanGroup (name)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.DiffieHellmanGroup)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.DiffieHellmanGroup.prototype"></a>[module crypto-browserify.DiffieHellmanGroup.prototype](#apidoc.module.crypto-browserify.DiffieHellmanGroup.prototype)

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.computeSecret"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.computeSecret)
- description and source-code
```javascript
function dhComputeSecret(key, inEnc, outEnc) {
  inEnc = inEnc || exports.DEFAULT_ENCODING;
  outEnc = outEnc || exports.DEFAULT_ENCODING;
  var ret = this._handle.computeSecret(toBuf(key, inEnc));
  if (outEnc && outEnc !== 'buffer')
    ret = ret.toString(outEnc);
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.generateKeys"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>generateKeys (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.generateKeys)
- description and source-code
```javascript
function dhGenerateKeys(encoding) {
  var keys = this._handle.generateKeys();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    keys = keys.toString(encoding);
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getGenerator"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getGenerator (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getGenerator)
- description and source-code
```javascript
function dhGetGenerator(encoding) {
  var generator = this._handle.getGenerator();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    generator = generator.toString(encoding);
  return generator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrime"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPrime (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrime)
- description and source-code
```javascript
function dhGetPrime(encoding) {
  var prime = this._handle.getPrime();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    prime = prime.toString(encoding);
  return prime;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrivateKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPrivateKey (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPrivateKey)
- description and source-code
```javascript
function dhGetPrivateKey(encoding) {
  var key = this._handle.getPrivateKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPublicKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.DiffieHellmanGroup.prototype.</span>getPublicKey (encoding)](#apidoc.element.crypto-browserify.DiffieHellmanGroup.prototype.getPublicKey)
- description and source-code
```javascript
function dhGetPublicKey(encoding) {
  var key = this._handle.getPublicKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Hash"></a>[module crypto-browserify.Hash](#apidoc.module.crypto-browserify.Hash)

#### <a name="apidoc.element.crypto-browserify.Hash.Hash"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Hash (algorithm, options)](#apidoc.element.crypto-browserify.Hash.Hash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hash.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hash.</span>super_ (options)](#apidoc.element.crypto-browserify.Hash.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Hash.prototype"></a>[module crypto-browserify.Hash.prototype](#apidoc.module.crypto-browserify.Hash.prototype)

#### <a name="apidoc.element.crypto-browserify.Hash.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Hash.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  this.push(this._handle.digest());
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hash.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Hash.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hash.prototype.digest"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>digest (outputEncoding)](#apidoc.element.crypto-browserify.Hash.prototype.digest)
- description and source-code
```javascript
digest = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  return this._handle.digest(outputEncoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hash.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hash.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.Hash.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Hmac"></a>[module crypto-browserify.Hmac](#apidoc.module.crypto-browserify.Hmac)

#### <a name="apidoc.element.crypto-browserify.Hmac.Hmac"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>Hmac (hmac, key, options)](#apidoc.element.crypto-browserify.Hmac.Hmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hmac.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hmac.</span>super_ (options)](#apidoc.element.crypto-browserify.Hmac.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.Hmac.prototype"></a>[module crypto-browserify.Hmac.prototype](#apidoc.module.crypto-browserify.Hmac.prototype)

#### <a name="apidoc.element.crypto-browserify.Hmac.prototype._flush"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>_flush (callback)](#apidoc.element.crypto-browserify.Hmac.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  this.push(this._handle.digest());
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hmac.prototype._transform"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.crypto-browserify.Hmac.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hmac.prototype.digest"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>digest (outputEncoding)](#apidoc.element.crypto-browserify.Hmac.prototype.digest)
- description and source-code
```javascript
digest = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  return this._handle.digest(outputEncoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.Hmac.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.Hmac.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.Hmac.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createDiffieHellman"></a>[module crypto-browserify.createDiffieHellman](#apidoc.module.crypto-browserify.createDiffieHellman)

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.createDiffieHellman"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.crypto-browserify.createDiffieHellman.createDiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createDiffieHellman.prototype"></a>[module crypto-browserify.createDiffieHellman.prototype](#apidoc.module.crypto-browserify.createDiffieHellman.prototype)

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.computeSecret"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.computeSecret)
- description and source-code
```javascript
function dhComputeSecret(key, inEnc, outEnc) {
  inEnc = inEnc || exports.DEFAULT_ENCODING;
  outEnc = outEnc || exports.DEFAULT_ENCODING;
  var ret = this._handle.computeSecret(toBuf(key, inEnc));
  if (outEnc && outEnc !== 'buffer')
    ret = ret.toString(outEnc);
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.generateKeys"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.generateKeys)
- description and source-code
```javascript
function dhGenerateKeys(encoding) {
  var keys = this._handle.generateKeys();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    keys = keys.toString(encoding);
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.getGenerator"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getGenerator)
- description and source-code
```javascript
function dhGetGenerator(encoding) {
  var generator = this._handle.getGenerator();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    generator = generator.toString(encoding);
  return generator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrime"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrime)
- description and source-code
```javascript
function dhGetPrime(encoding) {
  var prime = this._handle.getPrime();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    prime = prime.toString(encoding);
  return prime;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrivateKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPrivateKey)
- description and source-code
```javascript
function dhGetPrivateKey(encoding) {
  var key = this._handle.getPrivateKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPublicKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.getPublicKey)
- description and source-code
```javascript
function dhGetPublicKey(encoding) {
  var key = this._handle.getPublicKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPrivateKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>setPrivateKey (key, encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPrivateKey)
- description and source-code
```javascript
setPrivateKey = function (key, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.setPrivateKey(toBuf(key, encoding));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPublicKey"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createDiffieHellman.prototype.</span>setPublicKey (key, encoding)](#apidoc.element.crypto-browserify.createDiffieHellman.prototype.setPublicKey)
- description and source-code
```javascript
setPublicKey = function (key, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.setPublicKey(toBuf(key, encoding));
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createSign"></a>[module crypto-browserify.createSign](#apidoc.module.crypto-browserify.createSign)

#### <a name="apidoc.element.crypto-browserify.createSign.createSign"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createSign (algorithm, options)](#apidoc.element.crypto-browserify.createSign.createSign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createSign.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createSign.</span>super_ (options)](#apidoc.element.crypto-browserify.createSign.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createSign.prototype"></a>[module crypto-browserify.createSign.prototype](#apidoc.module.crypto-browserify.createSign.prototype)

#### <a name="apidoc.element.crypto-browserify.createSign.prototype._write"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.crypto-browserify.createSign.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createSign.prototype.sign"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>sign (options, encoding)](#apidoc.element.crypto-browserify.createSign.prototype.sign)
- description and source-code
```javascript
sign = function (options, encoding) {
  if (!options)
    throw new Error('No key provided to sign');

  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var ret = this._handle.sign(toBuf(key), null, passphrase);

  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    ret = ret.toString(encoding);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createSign.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createSign.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.createSign.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createVerify"></a>[module crypto-browserify.createVerify](#apidoc.module.crypto-browserify.createVerify)

#### <a name="apidoc.element.crypto-browserify.createVerify.createVerify"></a>[function <span class="apidocSignatureSpan">crypto-browserify.</span>createVerify (algorithm, options)](#apidoc.element.crypto-browserify.createVerify.createVerify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createVerify.super_"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createVerify.</span>super_ (options)](#apidoc.element.crypto-browserify.createVerify.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-browserify.createVerify.prototype"></a>[module crypto-browserify.createVerify.prototype](#apidoc.module.crypto-browserify.createVerify.prototype)

#### <a name="apidoc.element.crypto-browserify.createVerify.prototype._write"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.crypto-browserify.createVerify.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createVerify.prototype.update"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>update (data, encoding)](#apidoc.element.crypto-browserify.createVerify.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-browserify.createVerify.prototype.verify"></a>[function <span class="apidocSignatureSpan">crypto-browserify.createVerify.prototype.</span>verify (object, signature, sigEncoding)](#apidoc.element.crypto-browserify.createVerify.prototype.verify)
- description and source-code
```javascript
verify = function (object, signature, sigEncoding) {
  sigEncoding = sigEncoding || exports.DEFAULT_ENCODING;
  return this._handle.verify(toBuf(object), toBuf(signature, sigEncoding));
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
