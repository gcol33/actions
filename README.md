# actions

Composite GitHub Actions shared by my R package workflows.

## setup-pandoc

Installs pandoc through `r-lib/actions/setup-pandoc@v2`. If the download fails, it waits 90 s and retries; if that fails too, it installs pandoc from the runner's package manager (brew on macOS, apt on Linux, choco on Windows).

```yaml
- uses: gcol33/actions/setup-pandoc@v1
```

`method: package-manager` skips the release download and uses the package manager directly.
