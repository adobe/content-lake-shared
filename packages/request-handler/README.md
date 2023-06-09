# Content Lake Shared - Request Handler

> Supports handling HTTP and SQS requests in a lambda function.

This is one of the [Content Lake Shared](https://github.com/adobe/contentlake-shared) libraries.

## Status

[![GitHub license](https://img.shields.io/github/license/adobe/contentlake-shared.svg)](https://github.com/adobe/contentlake-shared/blob/main/LICENSE.txt)

## Usage

Install using:

```
npm install @adobe/contentlake-shared-request-handler
```

Use with:

```
import { RequestHandler } from '@adobe/contentlake-shared-request-handler';


const requestHandler = new RequestHandler()
  .withHandler(
    'some-action',
    (event, context) => someFunction(event, context),
  );

export const main = requestHandler.getMain();
```