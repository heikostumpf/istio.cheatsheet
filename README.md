# istio.cheatsheet

## Analyze
Analyze the istio configuration for a given namespace
````
istioctl analyze -n <namespace>
````

## Logging
Enable debug logging on Envoy proxies. The command can be applied to any pod running an envoy proxy or being an envoy proxy itself (e.g. ingress-gateway)
````
istioctl proxy-config log {ingress-pod}.istio-system --level debug
````
