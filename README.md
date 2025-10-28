# PAC-CLI-CheatSheet

Handy guide to the most common commands a Power Apps developer may need


## Authentication Commands

```powershell
# Create a new authentication profile
pac auth create --environment "YourEnvironmentName"

# List all authentication profiles
pac auth list

# Select a different authentication profile
pac auth select --index 2
```

## Canvas Power Apps Developer Essentials

Canvas app developers can leverage PAC CLI to automate various aspects of their development workflow:

```powershell
# List all canvas apps in the current environment
pac canvas list

# Download a canvas app as .msapp file
pac canvas download --id "app-id" --path "./MyApp.msapp"

# Generate a canvas app from a custom connector
pac canvas create --msapp MyGeneratedApp.msapp --connector-display-name "My Custom Connector"
```

## Source Control Operations

```powershell
# Extract an .msapp file into source files
pac canvas unpack --msapp MyApp.msapp --sources ./src

# Pack source files into an .msapp file
pac canvas pack --sources ./src --msapp MyApp.msapp

# Validate the source files
pac canvas validate --sources ./src
```

## Power Fx REPL: Read-Eval-Print-Loop

```
# Run Power Fx expressions
pac power-fx run
```