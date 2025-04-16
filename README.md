Using Node.js v20.18.3

Run the following:

```bash
$ yarn install
$ npx tsc -p jsconfig.json --noEmit
```

You will get this error:

```text
/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:122142
      throw e;
      ^

TypeError: Cannot read properties of undefined (reading 'flags')
    at getMembersOfSymbol (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:56777:19)
    at getLateBoundSymbol (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:56787:11)
    at getSymbolOfDeclaration (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:49588:43)
    at getSymbolOfNode (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:49591:34)
    at getFunctionExpressionParentSymbolOrSymbol (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:49598:198)
    at getResolvedMembersOrExportsOfSymbol (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:56742:27)
    at getExportsOfSymbol (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:49486:61)
    at resolveAnonymousTypeMembers (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:57350:19)
    at resolveStructuredTypeMembers (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:57698:11)
    at getSignaturesOfStructuredType (/Users/blazegt/test-tsc/node_modules/typescript/lib/_tsc.js:58389:24)

Node.js v20.18.3
```
