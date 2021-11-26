https://golangci-lint.run/usage/install/

# Go 1.16+
go install github.com/golangci/golangci-lint/cmd/golangci-lint@v1.43.0

# Go version < 1.16
go get -u github.com/golangci/golangci-lint/cmd/golangci-lint@v1.43.0

golangci-lint --version

golangci-lint run
