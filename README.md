# clog

- Multi-level coloring logger.
- Print coloring information
    - Prefix word
    - File name
    - Line
    - Function name 

## Installation

- Simply run
    ```shell
    $ go get github.com/GoblinBear/clog
    ```

## Library

- `clog.Info()`：Print greed prefix word `[INFO]`
- `clog.Debug()`：Print yellow prefix word `[DEBUG]`
- `clog.Error()`：Print red prefix word `[ERROR]`

## Example

```go
package main

import (
    "github.com/GoblinBear/clog"
)

func main() {
    clog.Info("There is some information.")

    num := 5
    clog.Debug("Total = %d monkeys", num)
    
    clog.Error("Connect to server error.")
}
```
![](https://github.com/GoblinBear/clog/blob/master/console.png)
