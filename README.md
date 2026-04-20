# Anyrow Go SDK

[![MIT License](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)

Go client library for the [Anyrow](https://anyrow.ai) API.

## Installation

```bash
go get github.com/anyrow/sdk-go@latest
```

## Quick start

```go
package main

import (
	"context"
	"fmt"

	sdk "github.com/anyrow/sdk-go"
)

func main() {
	client := sdk.New(sdk.Config{
		BaseURL: "https://api.anyrow.ai",
		Headers: map[string]string{
			"Authorization": "Bearer YOUR_API_KEY",
		},
	})

	_ = client
	fmt.Println("connected")
}
```

## Resources

- [OpenAPI spec](https://anyrow.ai/openapi.json)
- [TypeScript SDK](https://github.com/anyrow/sdk-typescript)
- [Python SDK](https://github.com/anyrow/sdk-python)
- [Rust SDK](https://github.com/anyrow/sdk-rust)
- [CLI](https://github.com/anyrow/cli)

## License

MIT — see [LICENSE](./LICENSE).
