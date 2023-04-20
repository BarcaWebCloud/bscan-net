## bscan-net v0.1.0

<br>

A .NET library for scan any computational device and atmospheric environment.

#### Requeriments:

- [SDK do .NET](https://www.microsoft.com/net/download)

<br>

### Building library

Build the library with the command below:

```
dotnet pack
```

<br>


In case you want to create a new class library type the following command

```
dotnet new classlib
```

For more information, see `dotnet new`.


### Published

<br>

Publish the *.nupkg* file to [nuget.org](https://nuget.org/) using the `dotnet nuget push` command with an **API key** that you obtain from [nuget.org](https://nuget.org/).

<br>

> #### Observation
>
> - [Nuget.org](https://nuget.org/) checks all uploaded **packages** for viruses and rejects **packages** if it finds *viruses*. [Nuget.org](https://nuget.org/) also scans all existing listed **packages** periodically.
> - Packages published on [nuget.org](https://nuget.org/) are publicly visible to other *developers* unless you unlist them. To host packages privately, see Host your own NuGet feeds.
>
>

<br>

### Get your API key

<br>

1. Log in to your [nuget.org](https://www.nuget.org/) account or [create an account](https://learn.microsoft.com/pt-br/nuget/nuget-org/individual-accounts#add-a-new-individual-account) if you don't already have one.

2. Select the **username** in the upper-right corner, then select **API Keys**.

3. Select Create and provide a name for your **key**.

4. Under **Select Scopes**, select **Push**.

5. In Select **Glob Default** Packages, enter: `*.`
 
6. Select **Create**.

7. Select **Copy** to copy the new **key**.

<br>

![Alt text](https://learn.microsoft.com/pt-br/nuget/quickstart/media/qs-create-api-key.png "api-key-nuget")

<br>

> #### Important
>
> - Always keep your **API key** secret. The **API key** is like a password that allows anyone to manage `packages` on your behalf. Delete or regenerate your **API key** if it is accidentally revealed.
>

<br>

### Publish with `dotnet nuget push`

<br>

In the folder containing the *.nupkg* file, run the following command. Specify your *.nupkg file name and replace the key value with your **API key**.

```
dotnet nuget push BScan.0.1.0.Test.1.0.0.nupkg --api-key qz2jga8pl3dvn2akksyquwcs9ygggg4exypy3bhxy6w6x6 --source https://api.nuget.org/v3/index.json
```
