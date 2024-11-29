# File-scoped namespaces

Always use file-scoped namespaces.

## Motivation

For free, takes away an indentation level which reduces complexity.

## Automation

editorconfig:
```
################################################################################
# File-scoped namespaces
# ID = 031ad72c773047b8be67d6e8ed8eccb9
################################################################################
# Namespace declaration preferences (IDE0160 and IDE0161)
csharp_style_namespace_declarations = file_scoped:warning

# IDE0160: Use block-scoped namespace
dotnet_diagnostic.IDE0160.severity = none

# IDE0161: Use file-scoped namespace
dotnet_diagnostic.IDE0161.severity = warning
################################################################################
```

Also, IDEs can refactor your whole solution in one step to use it.
