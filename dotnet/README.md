# .NET coding standards

Coding standards for everything related to .NET:
- .NET (the framework)
- C#
- ASP.NET
etc.

Also contains useful information regarding IDEs, tools, etc.

## `.editorconfig` notes
- Some `.editorconfig` configuration parts may include reference to tools you don't use (e.g. StyleCop). Feel free to remove those parts if they bother you, however it's not a problem if you leave them there for the sake of completeness (and you may start using them in the future, so you already have them configured in this regard).
- Most rules are configured as warnings. I also recommend treating warnings as errors. If this combination bothers you too much during code editing, you can set it up to only treat warnings as errors in non-DEBUG configuration. 