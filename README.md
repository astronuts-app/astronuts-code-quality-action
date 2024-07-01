# Astronuts Code Quality Action

This action runs Astronuts code quality scans.

### Inputs

These are some of the supported input parameters of the action.

- `sourceLanguage` - **_(Optional)_** the programming language of the source code to be analyzed.
- `rootDir` - _(Optional)_ The root directory of source code. If unspecified, its auto-detected.
- `buildSystem` - _(Optional)_ The build system. If not specified, the action tries to auto-detect one. For a list of supported build systems, see documentation.
- `failOnError` - _(Optional)_ If set to true, the build will fail if the code quality analysis fails. Build will pass silently otherwise.

### Supported Languages
- `java`
- `typescript`
- `javascript`
- `python`

### Supported Build Tools
- `gradle`
- `maven`
- `npm`
- `pip`

Note* : There is no need to specify build systems and languages explicitly used in the project as we use our
auto-detection system to detect that.
<br></br>
**We now support monorepos with multiple build systems and languages.

## Example usage

```yaml
uses: actions/astronuts-code-quality-action@v4
```

