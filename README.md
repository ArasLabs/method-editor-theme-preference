# Method Editor Theme Preference

This package adds a field to the User Preferences to allow users to select their preferred Method Editor Theme.

## Project Details

#### Built Using:
Aras 11.0 SP11

#### History:
Release | Notes
--------|--------
[v1.2](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1.2) | Upgraded to 11.0 SP11
[v1](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1) | Initial Release

#### Versions Tested:
Release | Aras
--------|-------
[v1.2](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1.2) | 11.0 SP11
[v1](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1) | 11.0 SP9-SP10 

#### Browsers Tested:
Internet Explorer 11, Firefox 45 ESR, Chrome

> [v1.2](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1.2) should be used only with 11.0 SP11 as it contains additional themes that were not present in earlier versions. Though [v1](https://github.com/ArasLabs/method-editor-theme-preference/releases/tag/v1) was built using 11.0 SP10, this version of the project should function in older releases of Aras Innovator 11.0.

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SP9+ preferred)
2. Aras Package Import tool
3. RunClientMethod import package

### Install Steps

#### Code tree Installation
These code tree changes only contain a custom icon for the toolbar. If you wish to use your own icon, you may replace the .svg file in the `\Innovator\` folder with your own.

1. Backup your code tree and store the archive in a safe place
2. Navigate to your local `..\RefreshFromDatabase\` folder
3. Copy the `\Innovator\` folder 
4. Paste this at the root of your install directory
+ By default this is `C:\Program Files\Aras\Innovator\`

#### Database Installation
1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\method-editor-theme-preference\Import\imports.mf` file in the Manifest File field.
6. Select **aras.labs.MethodEditorThemePreference** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

#### 

You are now ready to login to Aras and try out the Method Editor Theme user preference.

## Usage

1. Log in to Aras as admin.
2. Navigate to Administration->Preferences
3. Open the Preference for Innovator Admin
4. In the General Settings tab, input a value in the Method Editor Theme dropbox
+ If no theme is specified, the theme will default to textmate
5. Save the Preference
6. Open any Method to see the theme change!


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Original Aras community project written by Christopher Gillis at Aras Corp.

Documented and published by Christopher Gillis for Aras Labs. @cgillis-aras

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE) for license rights and limitations.