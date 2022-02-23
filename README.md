## ESM Loader work around
[https://github.com/phoenixframework/phoenix/issues/4662]  There is a problem that phoenix.js is shipped in a phoenix.esm.js and phoenix.cjs.js formats. When using Next.js with esmExternals: true
the system tries to load the cjs instead of the esm.

The solution is to just change the file name from phoenix.esm.js -> phoenix.mjs.  

Because it modifies the package.json this can't be done in a local project patch. So I'm just snap shotting 1.6.6 and making the change - with the hope that this will setting down in the future


## Copyright and License

Copyright (c) 2014, Chris McCord.

Phoenix source code is licensed under the [MIT License](LICENSE.md).
