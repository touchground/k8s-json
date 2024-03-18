# k8s-json
Validate input json syntax and convert it into an acceptable kubernetes string format.

Specific jsonFilePath to the locaion of your input:
```yaml
  test: 
    runs-on: ubuntu-latest
    steps:
    - id: processJson
      uses: touchground/k8s-json@main
      with:
        jsonFilePath: 'path/to/the/JSON'
```

Output above will be ${{ steps.processJson.outputs.content }}