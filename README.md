# kube-ninja
kube-ninja is a collection of kubectl plugins that empower you to become a Kubernetes ninja.

## Installation
To install kube-ninja, simply clone the GitHub repository and add the bin directory to your $PATH:

```bash
git clone https://github.com/thevahidal/kube-ninja.git
export PATH=$PATH:<path_to_kube-ninja>/bin
```

Once you've added the bin directory to your $PATH, you need to make the plugins executable.

To achieve that set the executable permission on the plugin files using the chmod command.

```bash
chmod +x <path_to_kube-ninja>/bin/*
# or one by one
chmod +x <path_to_kube-ninja>/bin/kubectl-find
```

## Usage
kube-ninja currently contains one plugin, find, which can help you find Kubernetes resources quickly and easily. To use the find plugin, simply run the following command:

```bash
kubectl find <resource_type> -n <namespace> <search_query>
```

For example, to find all Pods with the label "nginx", you can run:

```bash
kubectl find pods -n all nginx
```

In the future, kube-ninja will contain additional plugins that can help you perform common tasks with kubectl.

## Contributing
If you'd like to contribute to kube-ninja, please feel free to submit a pull request with your changes. We welcome contributions of all types, from bug fixes to new plugins.


## License
kube-ninja is released under the MIT License. Feel free to use, modify, and distribute this code as you see fit.
