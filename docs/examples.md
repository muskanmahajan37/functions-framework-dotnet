# Examples

The [examples](../examples) directory contains source code to
demonstrate various features of the Functions Framework. This page
provides commentary and explanation of those examples.

The examples are configured to refer to the projects in the
[src](../src) directory rather than the NuGet packages for simple
experimentation when building new features, but any function using
released functionality can be made standalone simply by converting
the project reference into a package reference and removing the
imports for MSBuild files from the Invoker project.

Some examples include multiple classes in a single source file. This
is purely to make the examples easier to follow when browsing on
GitHub.

## SimpleHttpFunction

The [SimpleHttpFunction](../examples/Google.Cloud.Functions.Examples.SimpleHttpFunction)
function is the result of creating a new HTTP function via the
template using the following command line:

```sh
dotnet new gcf-http
```

## SimpleEventFunction

The [SimpleEventFunction](../examples/Google.Cloud.Functions.Examples.SimpleEventFunction)
function is the result of creating a new Cloud Event function via the
template using the following command line:

```sh
dotnet new gcf-event
```

## VbHttpFunction

The [VbHttpFunction](../examples/Google.Cloud.Functions.Examples.VbHttpFunction)
function is the result of creating a new HTTP function via the
template using the following command line:

```sh
dotnet new gcf-http -lang vb
```

## VbEventFunction

The [VbEventFunction](../examples/Google.Cloud.Functions.Examples.VbEventFunction)
function is the result of creating a new Cloud Event function via the
template using the following command line:

```sh
dotnet new gcf-event -lang vb
```

## FSharpHttpFunction

The [FSharpHttpFunction](../examples/Google.Cloud.Functions.Examples.FSharpHttpFunction)
function is the result of creating a new HTTP function via the
template using the following command line:

```sh
dotnet new gcf-http -lang f#
```

## FSharpEventFunction

The [FSharpEventFunction](../examples/Google.Cloud.Functions.Examples.FSharpEventFunction)
function is the result of creating a new Cloud Event function via the
template using the following command line:

```sh
dotnet new gcf-event -lang f#
```

## SimpleDependencyInjection

The [SimpleDependencyInjection](../examples/Google.Cloud.Functions.Examples.SimpleDependencyInjection)
example demonstrates out-of-the-box dependency injection without
any additional configuration.

See the [dependency injection documentation](dependency-injection.md) for more details.

## AdvancedDependencyInjection

The [AdvancedDependencyInjection](../examples/Google.Cloud.Functions.Examples.AdvancedDependencyInjection)
example demonstrates dependency injection with extra configuration
provided via a startup class, including scoped and singleton
dependencies.

See the [dependency injection documentation](dependency-injection.md) for more details.

## TimeZoneConverter

The [TimeZoneConverter](../examples/Google.Cloud.Functions.Examples.TimeZoneConverter)
example provides a function with more business logic than most simple examples. It uses
the [Noda Time](https://nodatime.org) library to perform time zone conversions based
on the [IANA time zone database](https://www.iana.org/time-zones).

See the [README.md file](../examples/Google.Cloud.Functions.Examples.TimeZoneConverter/README.md)
for more details.

## Integration Tests

The [IntegrationTests](../examples/Google.Cloud.Functions.Examples.IntegrationTests)
directory contains integration tests for the example functions.
These can also be used as examples of how functions can be tested.
See the [testing documentation](testing.md) for more details.