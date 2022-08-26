                         

New Features and Enhancements in V9 Service Pack 2
==================================================

In this release, the following features have been introduced to provide an enhanced Volt MX Iris experience.

 

*   [Component Updates](#component-updates)
*   [Responsive Web Enhancements](#responsive-web-enhancements)
*   [Android Enhancements](#android-enhancements)
*   [ARRenderer Widget Enhancements](#arrenderer-widget-enhancements)
*   [Video Widget Enhancement - Closed Captions Support](#video-widget-enhancement-closed-captions-support)
*   [](#calendar-widget-enhancements)[Calendar Widget Enhancements](#Calendar)
*   [Dynamic Configuration of Skin Properties](#dynamic-configuration-of-skin-properties)
*   [Haptic Feedback Support - watchOS](#haptic-feedback-support-watchos)
*   [Tab Order Enhancement](#tab-order-enhancement)

Component Updates
-----------------

### Reorder Properties and Groups

In the V9 Service Pack 2 release, Volt MX Iris introduces the **Reorder Properties** option that enables developers to re-order or re-arrange the properties or groups of a Component (with Contract).

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#reorder-properties-or-groups).

### Generate getters and setters of a custom property

In the V9 Service Pack 2 release, Volt MX Iris introduces support to automatically generate the getters and setters of a custom property. When you create or modify a custom property through the **Manage Properties** dialog box, the getters and setters of the property are automatically added to the **initGettersSetters** function in the controller file of the component.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#getters).

Responsive Web Enhancements
---------------------------

### Custom CSS Splash Screen

In the V9 Service Pack 2 release, Volt MX Iris introduces support to implement CSS and HTML capabilities in the splash screen for Responsive web apps, by using Custom CSS and Custom HTML code. Prior to the V9 Service Pack 2 release, you could only use images to implement the splash screen for Responsive Web apps.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/Splash_Screen_Properties.md#configure-a-splash-screen-by-using-custom-css.html).

### Protected Mode CI Build

In the V9 Service Pack 2 release, Volt MX Iris introduces support to build web applications in the Protected mode by using the CI (Continuous Integration) build feature.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/SecureyourWebApplication.md#SecureCIbuild).

Android Enhancements
--------------------

### In-App Update APIs

On devices that use target SDK API version 21 (and later), the Google Play Core library allows in-app updates. By using the In-App Update APIs, developers can notify the user (while the user is using the app) that an app update is available for download.

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the following in-app update APIs

*   [voltmx.application.checkForAppUpdate](../../../Iris/iris_api_dev_guide/content/voltmx.application_in-app_updates_functions.md#checkForAppUpdate)
*   [voltmx.application.completeAppUpdate](../../../Iris/iris_api_dev_guide/content/voltmx.application_in-app_updates_functions.md#completeAppUpdate)
*   [voltmx.application.registerAppUpdateListener](../../../Iris/iris_api_dev_guide/content/voltmx.application_in-app_updates_functions.md#registerAppUpdateListener)
*   [voltmx.application.requestForAppUpdate](../../../Iris/iris_api_dev_guide/content/voltmx.application_in-app_updates_functions.md#requestForAppUpdate)
*   [voltmx.application.unRegisterAppUpdateListener](../../../Iris/iris_api_dev_guide/content/voltmx.application_in-app_updates_functions.md#unRegisterAppUpdateListener)

### In-App Review APIs

From the Android 5.0 (API level 21) release, the Google Play Core library supports the in-app review feature that provides users with an option to provide a review for the app (while the user is using the app).  
In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [voltmx.application.requestReviewFlow](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions_requestreview.md#requestReviewFlow) API that provides information required to launch the in-app review flow for an app.  
In addition, the [voltmx.application.requestReview](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions_requestreview.md#requestReview) API has been enhanced to accept **config** as an input parameter.

### Battery Optimization APIs

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the following Battery Optimization APIs:

*   [voltmx.application.isIgnoringBatteryOptimizations](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#isIgnoringBatteryOptimizations)
*   [voltmx.application.launchBatteryOptimizationSettings](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#launchBatteryOptimizationSettings)
*   [voltmx.application.requestIgnoreBatteryOptimizations](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#requestIgnoreBatteryOptimizations)

### Disable Auto-Reset Permissions

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [voltmx.application.launchAutoRevokeSettings](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions_runtimepermissionsapi.md#launchAutoRevokeSettings) API that helps users navigate to the application permissions page in the system settings. In the permissions page, the user can configure the system's ability to modify the app permissions.

### Install Source Details

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [voltmx.application.getInstallerSourceInfo](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#getInstallerSourceInfo) API that returns the package name from which the application was installed. The package name helps in identifying the market that the application was downloaded from.

### Cryptography API Enhancement - Base 64 String Support

In the V9 Service Pack 2 release, the [voltmx.crypto.createHash](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#createHash), and [voltmx.crypto.createHMacHash](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#voltmx.cry2) have been enhanced to accept an additional input parameter, [options](../../../Iris/iris_api_dev_guide/content/voltmx.crypto_functions.md#options). The **options** parameter is a data dictionary that contains the **returnBase64String** key.

ARRenderer Widget Enhancements
------------------------------

### Save and Retrieve Real World position

In the V9 Service Pack 2 release, Volt MX Iris introduces support to save the real-world position or planes, and then add a 3D object to that area. In addition, developers can also retrieve the same object when they scan the same plane.

To support this feature, the following properties and methods have been added to the ARRenderer widget:

*   [canSaveExperienceCallback](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Properties.md#canSaveExperienceCallback) property
*   [enableCloudAnchors](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Properties.md#enableCloudAnchors) Property
*   [clearExperience](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#clearExperience) Method
*   [hostCloudAnchor](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#hostCloudAnchor) Method
*   [loadExperience](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#loadExperience) Method
*   [resolveCloudAnchor](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#resolveCloudAnchor) Method
*   [saveExperience](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#saveExperience) Method

### Real-time Image Recognition and Overlays

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [StartARImageDetection](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#StartARImageDetection) and [stopARImageDetection](../../../Iris/iris_widget_prog_guide/Content/ARRenderer_Methods.md#stopARImageDetection) methods for the ARRenderer widget. Using these methods, developers can scan an image and overlay another image or a video on top of the scanned image.

VIDEO WIDGET ENHANCEMENT - CLOSED CAPTIONS SUPPORT
--------------------------------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support to display Closed Captions in the Video widget. Developers can add captions tracks and enable the captions.

To support this feature, the following properties and methods are added to the Video widget:

*   [enableCaptions](../../../Iris/iris_widget_prog_guide/Content/Video_Basic_Properties.md#enableCaptions) property
*   [tracks](../../../Iris/iris_widget_prog_guide/Content/Video_Basic_Properties.md#tracks) property
*   [setTracks](../../../Iris/iris_widget_prog_guide/Content/Video_Method.md#setTracks) method

Calendar Widget Enhancements
----------------------------

### Enable or Disable Dates

In the V9 Service Pack 2 release, Volt MX Iris introduces the [enableOrDisableDates](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#enableOrDisableDates) property for the Calendar widget. Using the **enableOrDisableDates** property, developers can configure the list of dates for the Calendar widget to display.

### Repeat Events in Intervals

In the V9 Service Pack 2 release, the [voltmx.phone.addCalendarEvent](../../../Iris/iris_api_dev_guide/content/voltmx.phone_functions.md#phone.ad) API is enhanced to accept [Interval](../../../Iris/iris_api_dev_guide/content/voltmx.phone_functions.md#Interval) as an input parameter. By using the **Interval** parameter, developers can configure an event on the calendar to repeat on a biweekly, quarterly, or semi-annual basis.

Dynamic Configuration of Skin Properties
----------------------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces the [voltmx.theme.setSkinsProperties](../../../Iris/iris_api_dev_guide/content/voltmx.theme_functions.md#setSkinsProperties) API. By using this API, developers can configure the Skin properties for a widget at run time. In addition, support for the following properties is added for a few widgets (such as Button, Calendar, Camera , CheckBoxGroup, Label, FlexContainer ,ListBox, RadioButtonGroup, RichText, TextBox2, TextArea2, and PickerView widgets):

*   focusStateSkin
*   pressedStateSkin (available on the Android platform)
*   disabledStateSkin (available on the Android platform)
*   hoverSkinState (available on the Responsive Web platform)

Haptic Feedback Support - watchOS
---------------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the following events that can be used to provide haptic feedback on the watchOS:

*   [didAppear](../../../Iris/iris_user_guide/Content/Watch.md#didAppear)
*   [interfaceDidScrollToTop](../../../Iris/iris_user_guide/Content/Watch.md#interfaceDidScrollToTop)
*   [interfaceOffsetDidScrollToBottom](../../../Iris/iris_user_guide/Content/Watch.md#interfaceOffsetDidScrollToBottom)
*   [interfaceOffsetDidScrollToTop](../../../Iris/iris_user_guide/Content/Watch.md#interfaceOffsetDidScrollToTop)

Tab Order Enhancement
---------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support to provide 0 or -1 as a value for the tab order. Prior to the V9 Service Pack 2 release, developers could only set values that were greater than zero.

For more information about this feature, click [here](../../../Iris/app_design_dev/Content/Accessibility_Iris.md#taborder2).
