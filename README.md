# go-update: Automatically update Go programs from the internet

go-update allows a program to update itself by replacing its executable file
with a new version. It provides the flexibility to implement different updating user experiences
like auto-updating, or manual user-initiated updates. It also boasts
advanced features like binary patching and code signing verification.

Updating your program to a new version is as easy as:

	err, errRecover := update.New().FromUrl("http://release.example.com/2.0/myprogram")
	if err != nil {
		fmt.Printf("Update failed: %v\n", err)
	}

## Documentation and API Reference

Comprehensive API documentation and code examples are available in the code documentation available on godoc.org:

### [https://godoc.org/github.com/inconshreveable/go-update](https://godoc.org/github.com/inconshreveable/go-update)

## Features

## [equinox.io](https://equinox.io)
go-update provides the primitives for building self-updating applications, but there a number of other challenges
involved in a complete updating solution such as hosting, code signing, update channels, gradual rollout,
dynamically computing binary patches, tracking update metrics, and more.

I provide this service, a complete solution, free for open source projects, at [equinox.io](https://equinox.io).

## License
Apache
