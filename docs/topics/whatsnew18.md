[//]: # (title: What's new in Kotlin 1.8.0)

<microformat>
   <p>The IDE support for Kotlin 1.8.0 is available for IntelliJ IDEA TBD.</p>
</microformat>

_[Release date: %kotlinReleaseDate%](eap.md#build-details)_

The Kotlin 1.8.0 release is out! Here are some highlights from this release:

* The old backend for Kotlin/JVM has been removed
* We now support Xcode 14
* We ensured compatibility with Gradle 7.3
* We introduced new experimental functions for JVM: recursively copy or delete directory content

## Kotlin/JVM

## Kotlin/Native

## Kotlin/JS

## Kotlin Multiplatform

## Gradle

## Compiler

## Standard library

Kotlin 1.8.0 offers new [extension functions](extensions.md#extension-functions) for the `java.nio.file.Path` class, which allows you to recursively copy or delete directory content:

* `copyToRecursively()`
* `deleteRecursively()`

> The new extension functions for `java.nio.file.Path` are [Experimental](components-stability.md).
> They may be changed at any time. Opt-in is required (see details below), and you should use them only for evaluation purposes.
>
{type="warning"}

As is usual for an experimental API, the new extensions require an opt-in: `@OptIn(kotlin.io.path.ExperimentalPathApi::class)`
or `@kotlin.io.path.ExperimentalPathApi`. Alternatively, you can use compiler option: `-opt-in=kotlin.io.path.ExperimentalPathApi`.

## Documentation updates

Since the previous release, the Kotlin documentation has received some notable changes: TBD

## Install Kotlin 1.8.0

[IntelliJ IDEA](https://www.jetbrains.com/idea/download/) TBD automatically suggest updating the Kotlin plugin to 1.8.0.

> For Android Studio TBD the Kotlin plugin 1.8.0 will be delivered
> with upcoming Android Studios updates.
>
{type="note"}

The new command-line compiler is available for download on the [GitHub release page](https://github.com/JetBrains/kotlin/releases/tag/v1.8.0).

### Compatibility guide for Kotlin 1.8.0

Kotlin 1.8.0 is a [feature release](kotlin-evolution.md#feature-releases-and-incremental-releases) and can, therefore, bring changes that are incompatible with your code written for earlier versions of the language.

Find the detailed list of such changes in the [Compatibility guide for Kotlin 1.8.0]().