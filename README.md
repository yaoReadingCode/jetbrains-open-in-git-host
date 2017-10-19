<h1 align="center">
  GitLink
  <br>
</h1>

<h4 align="center">
    A Jetbrains plugin that provides shortcuts to open a file or commit in Stash, GitHub, BitBucket or GitLab using the default browser or copy the link to the clipboard.
</h4>

<p align="center">
  <a href="https://travis-ci.org/ben-gibson/jetbrains-open-in-git-host">
    <img src="https://travis-ci.org/ben-gibson/jetbrains-open-in-git-host.svg?branch=master"
         alt="Gitter">
  </a>
  <a href="https://gitter.im/jetbrains-open-in-git-host/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge"><img src="https://badges.gitter.im/jetbrains-open-in-git-host/Lobby.svg"></a>
</p>
<br>

Installation
-------------------------------------------------------------------------------

This plugin is published on the
[JetBrains Plugin Repository](https://plugins.jetbrains.com/plugin/8183):

    Preferences → Plugins → Browse Repositories → Search for "GitLink"

### From Source

Clone this repository:

    $ git clone https://github.com/ben-gibson/GitLink
    $ cd GitLink

Update the permissions:

     $ chmod +x ./gradlew

Build the plugin zip file:

    $ ./gradlew buildPlugin

Install the plugin from `./build/distributions/GitLink-2.*.zip`:

    Preferences → Plugins → Install plugin from disk


Development
-------------------------------------------------------------------------------

Update the permissions:

     $ chmod +x ./gradlew

Execute an IntelliJ IDEA instance with the plugin you're developing installed:

    $ ./gradlew runIdea

Run the tests:

    $ ./gradlew test

Usage
-------------------------------------------------------------------------------

After installing the plugin set your remote host (GitHub, GitLab, BitBucket, Stash) and enabled extensions in the preferences:

      Preferences → Other Settings → GitLink
      
Make sure you have registered your projects root under the version control preferences:

      Preferences → Version Control (see unregistered roots)

Open a project file that is under Git version control in the editor:

      View → Open in Git host or
      Select in... → Open in Git host

The current branch is used unless it does not exist in the remote host in which case it defaults to using the master branch.
The resulting link can be copied to the clipboard depending on your plugin preferences.

Change log
-------------------------------------------------------------------------------

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

Contributing
-------------------------------------------------------------------------------

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

### Credits

License
-------------------------------------------------------------------------------

Please see [LICENSE](LICENSE) for details.
