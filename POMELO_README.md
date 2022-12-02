# Deploy new version
To deploy a new version, build the binary for the GitHub action environment and deploy it to the reviewdog cloud bucket.

```
env GOOS=linux GOARCH=amd64 go build ./cmd/reviewdog && gsutil cp reviewdog gs://reviewdog/
```