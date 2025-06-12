# axios-digest-auth

[![npm](https://img.shields.io/badge/npm-0.9.0-yellow)](https://www.npmjs.com/package/@ibrahimcavdar/axios-digest-auth)
[![docs](https://img.shields.io/badge/documentation-0.8.0-blue)](https://axios-digest-auth.mhoc.co)

A library which implements HTTP digest authentication in a manner which should be familiar to any
project which also uses Axios.

> **Note:** This is a forked version of the original [@mhoc/axios-digest-auth](https://github.com/mhoc/axios-digest-auth) repository that fixes the CSRF vulnerability issue present in the main repo.

## Installation

```bash
npm i @ibrahimcavdar/axios-digest-auth
```

## Usage

```typescript
import AxiosDigestAuth from "@ibrahimcavdar/axios-digest-auth";

const digestAuth = new AxiosDigestAuth({
  username: "your-username",
  password: "your-password",
});

// Make requests with digest authentication
const response = await digestAuth.request({
  url: "https://example.com/api/data",
  method: "GET",
});
```

Check out [the documentation site](https://axios-digest-auth.mhoc.co) for more information
on usage.

## Features

- Automatic HTTP Digest Authentication
- Compatible with Axios request configuration
- TypeScript support

## License

MIT
