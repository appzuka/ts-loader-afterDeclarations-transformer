# Demonstration of TypeScript custom transformer to transform d.ts files

This is a demonstration of using the getCustomTransformers ts-loader option to transform emitted d.ts files.  It is based on the CustomTransformer comparison test in ts-loader with an afterDeclarations transformer added.

The declarationsTrasformer simple replaces all identifiers with 'replaced_identifier', which is pointless but demonstrates that the transformer is running.

Some real cases of using afterDeclarations to transform d.ts files are given in the following article:

https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-1-7585d6916819

And the following repository uses this to transform imports in d.ts files:

https://github.com/longlho/ts-transform-json
