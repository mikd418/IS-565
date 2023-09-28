# September Creation

For our September creation, we have added to the open source vulnerability scanner [Nuclei](https://github.com/projectdiscovery/nuclei) by [Project Discovery](https://github.com/projectdiscovery)

## Nuclei
### How it works
Nuclei works by sending requests to targets to scan for vulnerabilities based on predefined templates. For example, you can use Nuclei with a default-login template to see if a web app is using any default credentials.

### Installing Nuclei
Nuclei requires **go1.20** to install successfully. Run the following command to install the latest version -

```sh
go install -v github.com/projectdiscovery/nuclei/v2/cmd/nuclei@latest
```

<details>
  <summary>Brew</summary>

  ```sh
  brew install nuclei
  ```
</details>
<details>
  <summary>Docker</summary>

  ```sh
  docker pull projectdiscovery/nuclei:latest
  ```
</details>

### Usage
```sh
nuclei -u <target> -t <path_to_template>
```

Installing Nuclei will install all nuclei templates by default. You can specify specific templates or directories of templates to use. Nuclei will use all templates if none are specified.
