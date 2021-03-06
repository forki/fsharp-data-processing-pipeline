[![Build status](https://ci.appveyor.com/api/projects/status/1skn6mpe3x91ipfs/branch/master?svg=true)](https://ci.appveyor.com/project/marcio-azevedo/fsharp-data-processing-pipeline/branch/master)
[![NuGet Version](https://img.shields.io/nuget/v/FSharp.DataProcessingPipelines.Core.svg?style=flat)](https://www.nuget.org/packages/FSharp.DataProcessingPipelines.Core/)
[![NuGet Version](https://img.shields.io/nuget/v/FSharp.DataProcessingPipelines.RabbitMQ.svg?style=flat)](https://www.nuget.org/packages/FSharp.DataProcessingPipelines.RabbitMQ/)

# Easily build data processing pipelines in F# #
Provides an extensible solution for creating Data Processing Pipelines in F#.

----------

This solution offers the basic infrastructure to build data processing pipelines in F# (or C# due to it's interoperability with F#).

The implementation is based on the [Pipes and Filters Pattern](https://msdn.microsoft.com/en-us/library/dn568100.aspx). The goal is to provide the basic Infrastructure as well as some External Interfaces implementations to allow an easy and fast setup of a typical Data Processing Pipeline, following Pipes and Filters pattern.

The typical scenario for establishing communication between Pipes and Filters is by providing integration with Queues, so if you have a scenario like this:

![](/docs/files/img/pipes-filters01.png)

You can implement an External Integration with a typical Messaging Queue System and you get a Pub/Sub system (Event-oriented):

![](/docs/files/img/pipes-filters02.png)

The project [FSharp.DataProcessingPipelines.Core](/src/FSharp.DataProcessingPipelines.Core/) provides the basic definition of the Core Entities like Messages, Pipes, Filters and Runners.

### [Currently supported integrations](../../wiki/2.-Supported-Integrations/) ###

For more details about how to use / extend this see the [Wiki](../../wiki/). If you find any issues, please report in [Issues](../../issues/).

**This is a open source project from and for the community so feel free to contribute (don't forget to send your contact) - just pick a task in [Trello Project](https://trello.com/b/JlE1RNwN/f-data-processing-pipeline)!**

**Note**: The solution structure is based on the [prototypical .NET solution (file system layout and tooling), recommended by the F# Foundation.](https://github.com/fsprojects/ProjectScaffold/).
