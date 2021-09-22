# job-microservice-build
A sequence of actions that setups a dotnet environment, builds your dotnet application, runs the tests, generates build assets and migrations scripts.

## Usage

### Usage example
```yaml
    steps:
      - name: Build
        uses: EasyDesk/job-microservice-build@v1
        with:
          dotnet-version: <dotnet-version> # Like 5.x
          main-project: <project-name> # Without the .csproj
          unit-tests-project: <project-name> # Without the .csproj
          output-dir: <path-to-dir>
          sql-file-name: <path-to-file>.sql
          warnings-as-errors: true
```
