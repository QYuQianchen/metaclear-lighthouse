# Metaclear-Lighthouse

(Code forked from `sigp/lighthouse`)

This code is used in the research work on the metadata privacy of MEV Relay.

- Collects attestations
- Collects public key and multiaddress pairs
- Add prometheus metrics

## Build
```bash
export metaclear_lighthouse_img=$(git rev-parse --short HEAD)
docker build -f Dockerfile -t "hoprnet/metaclear-lighthouse:$metaclear_lighthouse_img" .

# Load the local image to minikube
minikube image load "hoprnet/metaclear-lighthouse:$metaclear_lighthouse_img"
echo $metaclear_lighthouse_img
```
