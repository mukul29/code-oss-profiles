# code-oss-profiles

#### A simple wrapper script written in Bash to enable specific extensions in vscode on startup. 

### Setup
Run the following commands

```
git clone https://github.com/mukul29/code-oss-profiles
cd code-oss-profiles
chmod +x code-oss-profiles
sudo cp code-oss-profiles /usr/local/bin # or any other location in PATH
mkdir -p ~/.config/code-oss-profiles
cp profiles.json ~/.config/code-oss-profiles
```

### Running code-oss-profiles

Use the `-p` flag to specify the profile name. This profile name should be in the profiles.json file and should generally not be `_common`.

Example:

```code-oss-profiles -p python```

would load the extensions specified in the `python` key from profiles.json as well as the extensions in the `_common` key.

The extensions in `_common` are always enabled when using the `-p` flag.

Specifying no flag would just result in running code-oss with all the extensions enabled.
