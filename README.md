This is a project for detailed setup to deploy nextjs app on iis

This project includes 2 different ways to deploy to iis.
- using `iisnode`
- using `httpPlatformHandler`

# Packages

Install following packages

```bash

npm install -D fs-extra @types/fs-extra

npm install -D ts-node

```

# Build configuration
- Modify next.config.ts as follow

    ```ts
    import type { NextConfig } from "next";

    const nextConfig: NextConfig = {
    output: "standalone"
    };

    export default nextConfig;

    ```

# Required Files

- publish-iis-http-platform.ts
  run `ts-node ./publish-iis-http-platform.ts` for deploy using httpPlatformHandler

- publish-iis-iisnode.ts
  run `ts-node ./publish-iis-iisnode.ts` for deploy using iisnode

