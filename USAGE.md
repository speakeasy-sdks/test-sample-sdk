<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testsamplesdk "github.com/speakeasy-sdks/test-sample-sdk"
	"log"
)

func main() {
	s := testsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->