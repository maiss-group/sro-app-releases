# Schulrecht Online — Linux release artefacts

Release binaries for the Linux build of the **Schulrecht Online** app by
Verlag J. Maiss GmbH. This repository holds **no source code**: it exists only
so published artefacts have a stable, publicly reachable URL.

## Why it exists

Flathub does not compile closed-source applications. Its manifest instead points
at a prebuilt tarball and pins that file's `sha256`, so the artefact must be
fetchable by Flathub's buildbot and by every machine installing the app. The
application source lives in a private repository; only the built artefact is
published here.

## What is published

Each release carries, for x86_64:

- `schulrecht-online-<version>-x86_64.tar.gz` — the runnable bundle plus its
  desktop entry, AppStream metainfo and icon tree
- `schulrecht-online-<version>-x86_64.tar.gz.sha256`

Artefacts are produced by CI from the application repository, never by hand.

## Published files are never replaced

Flathub pins a `sha256`. A published file that changes breaks every Flathub
build that referenced it. Releases here are **append-only**: to correct a
release, publish a new version.

## Installing

Install the app from **Flathub** or the **Snap Store** rather than from here.
The tarballs are packaging inputs, not a supported distribution channel: they
are unsigned, carry no installer, and receive no automatic updates.

## Support

<https://www.schulrecht-online.de>
