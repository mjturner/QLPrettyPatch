QLPrettyPatch
=============

QLPrettyPatch is a QuickLook generator for patch files.

Once installed, you can select patch file attachments in an email or patch files in Finder, hit `spacebar` and get a colorized/prettified representation of the patch.

From the Terminal, you can also run `qlmanage -p /path/to/my.patch` to open the patch in a QuickLook preview pane.

![Example patch file QuickLook preview](https://github.com/atnan/QLPrettyPatch/raw/master/Screenshot.png)

### Installation

There are two options for installation:

1. To install a pre-built copy, head to the [Releases page](https://github.com/atnan/QLPrettyPatch/releases) and download the latest `QLPrettyPatch.qlgenerator.zip` file. Unzip the archive, and copy `QLPrettyPatch.qlgenerator` to `~/Library/QuickLook/`.
2. To build your own copy, clone the project, open `QLPrettyPatch.xcproj` in Xcode and build the `Install` target. The build product will automatically be copied to `~/Library/QuickLook/QLPrettyPatch.qlgeneator`.

### Credits

QLPrettyPatch uses the incredibly useful [PrettyPatch formatter](http://svn.webkit.org/repository/webkit/trunk/Websites/bugs.webkit.org/PrettyPatch/), which is used by the patch review system on [bugs.webkit.org](https://bugs.webkit.org).

### Related Tools

If you find yourself sending emails with patch attachments and want to include a prettified version of the patch in the email body, you should take a look at my [atnan/purdypatch](https://github.com/atnan/purdypatch) command line tool. It uses the same underlying formatter as this QuickLook generator.
