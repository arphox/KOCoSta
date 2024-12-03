# 'using' directive placement

Always place `using` directives outside the namespace.

## Motivation

Placing it inside or outside both can have smaller advantages and disadvantages, depending on who you ask. Here, consistency is more important than the actual choice.

I chose _outside namespace_ because I like that one more and is more widely used, e.g. in the source code of .NET runtime and Roslyn.

## Automation

editorconfig:
```
################################################################################
# 'using' directive placement
# ID = 2e10dd93856c44aab3e89c4c1c9da0e9
################################################################################
# IDE0065: 'using' directive placement
csharp_using_directive_placement = outside_namespace:warning
dotnet_diagnostic.IDE0065.severity = warning

# SA1200: UsingDirectivesMustBePlacedCorrectly
# Turned off, because checked by IDE0065
dotnet_diagnostic.SA1200.severity = none
################################################################################
```

Also, IDEs can refactor your whole solution in one step to use it.
