                         

New Features and Enhancements in V9 Service Pack 1
==================================================

In this release, the following features have been introduced to provide an enhanced Volt MX Iris experience.

 

*   [Simple Responsive Design](#simple-responsive-design)
*   [Emulators Support for iOS and Android](#emulators-support-for-ios-and-android)
*   [Enhanced Theme feature - Support to Rebrand a Project](#enhanced-theme-feature-support-to-rebrand-a-project)
*   [Rollback to a specific version of  Volt MX Iris](#rollback-to-a-specific-version-of)
*   [Enhanced Upgrade Feature](#enhanced-upgrade-feature)
*   [Support for Component Versioning](#support-for-component-versioning)
*   [Mapping Editor Enhancement - Support to Map Breakpoint-specific Data](#mapping-editor-enhancement-support-to-map-breakpoint-specific-data)
*   [Test Automation Enhancement - Fetch and Edit a Widget Path](#test-automation-enhancement-fetch-and-edit-a-widget-path)
*   [Android Enhancements](#android-enhancements)
    *   [Enhanced Scroll Functionality](#enhanced-scroll-functionality)
    *   [Scoped Storage Access APIs](#scoped-storage-access-apis)
    *   [RawBytes Object Enhancements](#rawbytes-object-enhancements)
    *   [Date and Time KeyBoard Styles](#date-and-time-keyboard-styles)
    *   [Handle Recoverable Exception](#handle-recoverable-exception)
    *   [Location Updates Enhancements](#location-updates-enhancements)
    *   [Gradle Entry for the BottomSheet widget](#gradle-entry-for-the-bottomsheet-widget)
    *   [Enable Controller Cloning for Segment Row Template](#enable-controller-cloning-for-segment-row-template)
*   [Volt MX IQ - Enhanced Language Translation Support](#volt-mx-iq-enhanced-language-translation)
*   [Cookie Management APIs](#cookie-management-apis)
*   [Secure data input in TextBox and TextArea widgets](#secure-data-input-in-textbox-and-textarea-widgets)
*   [Accessibility Enhancement - Support for Tab Order](#accessibility-enhancement-support-for-tab-order)

 

Simple Responsive Design
------------------------

The Simple Responsive Design feature provides a quick and convenient way to create responsive apps for the Web, Mobile, and Tablet channels.  
Volt MX  Iris has introduced the Responsive Grid layout for the [FlexForm](../../../Iris/iris_widget_prog_guide/Content/FlexForm_Properties.md#flexResponsive), [FlexContainer](../../../Iris/iris_widget_prog_guide/Content/FlexContainer_Properties.md#flexResponsive), and [FlexScrollContainer](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#flexResponsive) widgets to support the Simple Responsive Design feature. A new property, [responsiveConfig](../../../Iris/iris_widget_prog_guide/Content/FlexContainer_Properties.md#responsiveConfig), has also been introduced for the FlexContainer widget that allows you to set the width of a container and the space between adjacent containers.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/Responsive_Design.md).

Emulators Support for iOS and Android
-------------------------------------

Developers can now view their apps on iOS and Android emulators. In the build screen, Volt MX Iris displays a list of configured emulators, using which you can launch and run apps in [iOS](../../../Iris/iris_user_guide/Content/SUGiPhone.md#launch-the-app-using-run-on-my-device-or-the-emulator-menu) and [Android](../../../Iris/iris_user_guide/Content/SUG_Android.md#launch-the-app-using-run-on-my-device-or-the-emulator-menu) native emulators.

Enhanced Theme feature - Support to Rebrand a Project
-----------------------------------------------------

The Theme feature is enhanced with a new rebrand capability. The **Find and Replace Skin Properties** option has been added in the Edit menu of Volt MX Iris. This feature enables you to customize the Background, Border, and Font properties of the skins present in the current theme of the project.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/FindReplaceSkin.md).

Rollback to a specific version of  Volt MX Iris
-----------------------------------------------------

Developers can now Rollback to a specific Fix Pack within a Service Pack.

For more information on this feature, click [here](../../../Iris/iris_starter_install_win/Content/Upgrade.md#rollback-to-a-previous-version-of-volt-mx-iris).

Enhanced Upgrade Feature
------------------------

The upgrade process is enhanced giving the developers more flexibility to choose the Fix Pack or Service Pack version they want to upgrade to.

For more information on this feature, click [here](../../../Iris/iris_starter_install_win/Content/Upgrade.md#update-volt-mx-iris).

Support for Component Versioning
--------------------------------

In Volt MX Iris, developers can now create and use different versions of a component in an application.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_UsingComponents.md#import-different-versions-of-an-existing-component).

Mapping Editor Enhancement - Support tO mAP Breakpoint-sPECIFIC dATA
--------------------------------------------------------------------

Using Volt MX Iris you can now map different data for different breakpoints or channels. The feature helps developers to showcase only the specific data required in a breakpoint or a channel.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/ActionsMapping.md#map-data-across-channels-and-breakpoints).

Test Automation Enhancement - Fetch and Edit a Widget Path
----------------------------------------------------------

The Test Automation feature is enhanced with new fetch and edit a widget path features. While the Test Automation is being recorded, developers can click on any widget in the application to view or edit the path of the widget.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/TestAutomation.md#fetchWidget).

Android Enhancements
--------------------

### Enhanced Scroll Functionality

To enhance the consistency of the scroll behavior across platforms, Volt MX Iris has introduced the [overScrollX](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#overScrollX) and [overScrollY](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#overScrollY) properties for the FlexScrollContainer widget on the Android platform. Further, to maintain consistent scrolling behavior, the Android platform also supports the [bounces](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#bounceAndroid), [allowHorizontalBounce](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#hbounceAndroid), and [allowVerticalBounce](../../../Iris/iris_widget_prog_guide/Content/FlexScrollContainer_Properties.md#vbounceAndroid) properties.

### Scoped Storage Access APIs

If the targetSDK version of an Android app is 29 or later, scoped storage is enabled for the app, by default. Therefore, the following Scoped Storage APIs are added to replace the Legacy Storage APIs (such as getExternalStorageDirectoryPath).

*   [voltmx.io.FileSystem.getExternalCacheDir](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#getExternalCacheDir)
*   [voltmx.io.FileSystem.getExternalCacheDirs](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#getExternalCacheDirs)
*   [voltmx.io.FileSystem.getExternalFilesDir](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#volt-mx-io-filesystem-getexternalfilesdir)
*   [voltmx.io.FileSystem.getExternalFilesDirs](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#volt-mx-io-filesystem-getexternalfilesdirs)
*   [voltmx.io.FileSystem.getNoBackupFilesDir](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#getNoBackupFilesDir)
*   [voltmx.io.FileSystem.getExternalStorageState](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#getExternalStorageState)
*   [voltmx.io.FileSystem.getFileSystemStats](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#voltmx.io.)
*   [voltmx.io.FileSystem.isExternalStorageEmulated](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#volt-mx-io-filesystem-isexternalstorageemulated)
*   [voltmx.io.FileSystem.isExternalStorageLegacy](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#isExternalStorageLegacy)
*   [voltmx.io.FileSystem.isExternalStorageRemovable](../../../Iris/iris_api_dev_guide/content/voltmx.io.filesystem_functions.md#volt-mx-io-filesystem-isexternalstorageremovable)

### RawBytes Object Enhancements

*   Support to assign RawBytes as an input to the [Cryptography APIs](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#functions) has been added on the Android platform.
*   The [voltmx.crypto.decrypt](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#decrypt) and [voltmx.crypto.asymmetricDecrypt](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#asymmetricDecrypt) APIs now support the [decryptToRawBytes](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#decryptToRawBytes) property.
*   The following APIs have been added to the RawBytes Object:
    *   [voltmx.types.RawBytes.clear](../../../Iris/iris_api_dev_guide/content/voltmx.types_objects_rawbytes.md#clear)
    *   [voltmx.types.RawBytes.getContentType](../../../Iris/iris_api_dev_guide/content/voltmx.types_objects_rawbytes.md#getContentType)

### Date and Time KeyBoard Styles

Volt MX  Iris has introduced [keyboard styles](../../../Iris/iris_widget_prog_guide/Content/TextBox_Properties.md#dateTimekeyBoard) and a [text input mode](../../../Iris/iris_widget_prog_guide/Content/TextBox_Properties.md#dateTimeTextInputMode) for the Date and Time values in the TextBox and TextArea widgets on the Android platform.

### Handle Recoverable Exception

Support for the [HandleRecoverableException](../../../Iris/iris_api_dev_guide/content/image_methods.md#handleRecoverableException) parameter has been added in the [writeToMediaGallery](../../../Iris/iris_api_dev_guide/content/image_methods.md#writeToMediaGallery) API.

### Location Updates Enhancements

Support for the [requireBackgroundAccess](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#requiredBackgroundAccess) parameter has been added in the [voltmx.location.getCurrentPosition](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#getCurrentPosition) and [voltmx.location.watchPosition](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#watchPosition) APIs.  
In addition, updates have been made to include [Android-specific Error Codes](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#Android_ErrorCodes).

### Gradle Entry for the BottomSheet widget

From AndroidSDK version 26, if an app contains a BottomSheet widget, you must add additional dependencies in the Android gradle entries. For more information on the Gradle entries that you must provide, click [here](../../../Iris/iris_widget_prog_guide/Content/BottomSheet.md#gradleEntry).

### Enable Controller Cloning for Segment Row Template

Volt MX  Iris has introduced the [enableCloneControllerForRowTemplates](../../../Iris/iris_widget_prog_guide/Content/Segment_Properties.md#enableCloneControllerForRowTemplates) property for the Segment widget. This property is only available on the Android platform. It allows developers to clone the row template controller for each row of a Segment widget.

Volt MX  IQ - Enhanced Language Translation
------------------------------------------

Volt MX  IQ's language translation feature now supports all the locales supported by Google Translate.

For more information about this feature, click [here](../../../Iris/iris_user_guide/Content/VoltMX_IQ.md).

Cookie Management APIs
----------------------

To support the WKWebView engine's usage of separate cookie storage, the [setCookies](../../../Iris/iris_widget_prog_guide/Content/Browser_Methods.md), [getCookies](../../../Iris/iris_widget_prog_guide/Content/Browser_Methods.md), [clearCookies](../../../Iris/iris_widget_prog_guide/Content/Browser_Methods.md) methods have been added for the Browser widget.

Support for the [voltmx.net.setCookies](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md#setCookies) API has been added in the iOS Framework. The API allows users to add or replace cookies in the app cookie storage. In addition, support for the [cookieFormat](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md.html#cookieFormat) parameter has been added in the [voltmx.net.getCookies](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md.html#voltmx.net8) API.

A new [shareCookiesInBrowsers](../../../Iris/iris_widget_prog_guide/Content/Browser_Methods.md) property has also been added to enable the sharing of the cookies between browsers.

Secure data input in TextBox and TextArea widgets
-------------------------------------------------

Data input for TextBox and TextArea widgets has been enhanced with additional security by using the [isSensitiveText](../../../Iris/iris_widget_prog_guide/Content/TextBox_Properties.md#isSensitiveText) property.

Accessibility Enhancement - Support For Tab Order
-------------------------------------------------

From Volt MX Iris V9 Service Pack 1, the Tab Order field has been introduced in the Accessibility Config properties of Desktop Web Forms.

For more information about this feature, click [here](../../../Iris/app_design_dev/Content/Accessibility_Iris.md#taborder).
