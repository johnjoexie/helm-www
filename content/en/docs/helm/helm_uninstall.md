---
title: "Helm Uninstall"
---

## helm uninstall

uninstall a release

### Synopsis


This command takes a release name and uninstalls the release.

It removes all of the resources associated with the last release of the chart
as well as the release history, freeing it up for future use.

Use the '--dry-run' flag to see which releases will be uninstalled without actually
uninstalling them.


```
helm uninstall RELEASE_NAME [...] [flags]
```

### Options

```
      --description string   add a custom description
      --dry-run              simulate a uninstall
  -h, --help                 help for uninstall
      --keep-history         remove all associated resources and mark the release as deleted, but retain the release history
      --no-hooks             prevent hooks from running during uninstallation
      --timeout duration     time to wait for any individual Kubernetes operation (like Jobs for hooks) (default 5m0s)
```

### Options inherited from parent commands

```
      --add-dir-header                   If true, adds the file directory to the header
      --alsologtostderr                  log to standard error as well as files
      --debug                            enable verbose output
      --kube-apiserver string            the address and the port for the Kubernetes API server
      --kube-context string              name of the kubeconfig context to use
      --kube-token string                bearer token used for authentication
      --kubeconfig string                path to the kubeconfig file
      --log-backtrace-at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log-dir string                   If non-empty, write log files in this directory
      --log-file string                  If non-empty, use this log file
      --log-file-max-size uint           Defines the maximum size a log file can grow to. Unit is megabytes. If the value is 0, the maximum file size is unlimited. (default 1800)
      --logtostderr                      log to standard error instead of files (default true)
  -n, --namespace string                 namespace scope for this request
      --registry-config string           path to the registry config file (default "~/.config/helm/registry.json")
      --repository-cache string          path to the file containing cached repository indexes (default "~/.cache/helm/repository")
      --repository-config string         path to the file containing repository names and URLs (default "~/.config/helm/repositories.yaml")
      --skip-headers                     If true, avoid header prefixes in the log messages
      --skip-log-headers                 If true, avoid headers when opening log files
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          number for the log level verbosity
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO

* [helm](../helm)	 - The Helm package manager for Kubernetes.

###### Auto generated by spf13/cobra on 11-May-2020
