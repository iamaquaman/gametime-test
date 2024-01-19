**Python APP**

The Fibonacci sequence function works based on user input, but it has an arbitrary limit of 50 where it doesn't have the logic to handle a number above 50. It also does not contain any error handling.

**Chart**

You can run the staging chart by running:

```
helm upgrade --install --create-namespace \
  --namespace staging-fibonacci-app \
  -f charts/staging.yaml \
  staging-python-app \
  charts/
```

*CircleCI**

The CircleCI config assumes you have environment variables injected via the Console and that you have access to an EKS cluster.
