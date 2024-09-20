# CreateProjectDefinitions

## Example Usage

```typescript
import { CreateProjectDefinitions } from "@vercel/sdk/models/operations/createproject.js";

let value: CreateProjectDefinitions = {
  host: "vercel.com",
  path: "/api/crons/sync-something?hello=world",
  schedule: "0 0 * * *",
};
```

## Fields

| Field                                           | Type                                            | Required                                        | Description                                     | Example                                         |
| ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| `host`                                          | *string*                                        | :heavy_check_mark:                              | The hostname that should be used.               | vercel.com                                      |
| `path`                                          | *string*                                        | :heavy_check_mark:                              | The path that should be called for the cronjob. | /api/crons/sync-something?hello=world           |
| `schedule`                                      | *string*                                        | :heavy_check_mark:                              | The cron expression.                            | 0 0 * * *                                       |