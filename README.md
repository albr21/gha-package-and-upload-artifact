# gha-package-and-upload-artifact

GitHub Action used as a workaround for GHES multi-file artifact slowdown - Packages files into a single archive before uploading via actions/upload-artifact.

## Usage

```yaml
steps:
  - name: Package and Upload Artifact
    uses: albr21/gha-package-and-upload-artifact@1.0.0
    with:
      path: path/to/folder
      artifact-name: my-artifact
      package-name: my-package
```

Enable output variable:

| Name | Description |
| --- | --- |
| `artifact-id` | The id of the uploaded artifact on GitHub |
| `package-name` | The name of the created package |

## Contributing

Check out the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
