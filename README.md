# Example usage

```golang
package main

import (
	"fmt"
	"os"
	"strings"

	_ "github.com/aqua777/go-dotenv"
)

func main() {
	for _, env := range os.Environ() {
		if strings.HasPrefix(env, "TEST_") {
			fmt.Println(env)
		}
	}
}
```
