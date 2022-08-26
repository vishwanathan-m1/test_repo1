                         

New Features and Enhancements in V9 SP2 M1
==========================================

In this release, the following features have been introduced to provide an enhanced Volt MX Iris experience.

 

*   [Create and Use Form Templates](#create-and-use-form-templates)
*   [Component Updates](#component-updates)
*   [Data and Services Panel Enhancements](#data-and-services-panel-enhancements)
*   [Test Automation Enhancements](#test-automation-enhancements)
*   [Android Enhancements](#android-enhancements)
*   [Support for Widget Extensions](#support-for-widget-extensions)
*   [Sign In With Apple](#sign-in-with-apple)
*   [Calendar Enhancements for Responsive Web](#calendar-enhancements-for-responsive-web)
*   [ListBox Widget Enhancements](#listbox-widget-enhancements)
*   [zIndex Support for Map Methods](#zindex-support-for-map-methods)
*   [Text Widget Enhancement - Support for textCopyable property](#text-widget-enhancement)

 

Create and Use Form Templates
-----------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces a feature that provides an easy way to reuse a form as a template across the project. Using Form Templates, you can display the same UI pattern across multiple forms, platforms, and projects. To use Form Templates, you must first create a form with the required UI elements and add it to a Collection Library. You can then drag-and-drop the template from the collection library onto a form or import the template into your project.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/FormTemplates.md).

Component Updates
-----------------

### Component Versioning Enhancement

In the V9 Service Pack 2 release, Volt MX Iris introduces support to view the version number and store multiple versions of a component underthe **My Libraries** section. Components from the libraries can be directly added to a form or to the Project Components.

For more information on viewing and storing multiple versions of a component, click [here](../../../Iris/iris_user_guide/Content/C_UsingComponents.md#Mversion).

For more information on adding multiple versions of collections from Templates, click [here](../../../Iris/iris_user_guide/Content/C_UsingComponents.md#Addcomponent).

### Update Existing Components

In the V9 Service Pack 2 release, Volt MX Iris introduces support to update an existing component to a desired higher version. You can view all the higher versions of a component in the Update Component dialog box, and then select the version that you want to update to.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_UsingComponents.md#update-a-component-instance).

### Define Conditional and Dependent Properties for Components with Contract

In the V9 Service Pack 2 release, Volt MX Iris introduces the conditional rendering of properties feature allows you to define conditions and dependencies between properties for a component with contract. For example, using this feature, you can update the visibility of a dependent property based on the value of another property.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#Conditions).

### Tooltip for Properties of a Component

In the V9 Service Pack 2 release, Volt MX Iris introduces the Tooltip feature for the custom properties of a Component with contract. Developers can provide detailed information about the functionality of the property that appears when a developer using the component hovers over the property in the component.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#Tooltip).

### Support for JSON as a Property Type for Components with Contract

In the V9 Service Pack 2 release, Volt MX Iris introduces support to provide JSON as a Property Type for custom properties in the Manage Properties section for components with contract.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#JSON).

### i18N as a Pass-through Property for Components with Contract

From Volt MX Iris V9 Service Pack 2, you can add i18N properties as a Pass-through property for Components with contract. This helps users support Internationalization more easily in the components with contract. You can add the property from the Manage Properties section of the Components or add the property directly from the Properties panel.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_CreatingComponent.md#i18N).

### Support to Add Components Within a Segment

In the V9 Service Pack 2 release, Volt MX Iris introduces support to add components (with contract) within a Segment Template.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/C_UsingComponents.md#Adding).

### Expose Component Event as a Pass-through Event in a Component with Contract

With the V9 Service Pack 2 release, Iris enables the capability to expose an event in a component with contract as a pass-through event. The pass-through event at the instance can then be used to modify the existing functionality in the event or to extend the functionality of the event.

Data and Services Panel Enhancements
------------------------------------

*   ### Support to Add Custom Verbs to a Form
    
    From Volt MX Iris V9 Service Pack 2, you can drag and drop a Custom Verb from the Data and Services panel onto a form. Custom Verbs along with the fields and attributes of the custom verbs appear in the Data and Services panel. When you add a Custom Verb to a form, Volt MX Iris generates a popup that allows you to select templates for both the Request and Response UI generation.
    
    For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/DataPanel.md#custom-verbs-in-data-and-services-panel).
    
*   ### Support to Add Child Objects to a Form
    
    From Volt MX Iris V9 Service Pack 2, you can drag and drop Child Objects from the Data and Services panel onto a form. When you add a Child Object to a form, Volt MX Iris generates a custom UI for the Child Object and sends the metadata to the Volt MX Foundry Console.
    
    For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/DataPanel.md#add-child-objects-to-a-form).
    
*   CRUD Forms will now automatically ignore the Child Objects when you select a form from the Data and Services panel at the service level. For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/DataPanel.md#Crudnote).

Test Automation Enhancements
----------------------------

### Configure Timeout for a TestCase

Prior to the V9 Service Pack 2 release, there was no option to configure the timeout for individual test cases, and a default timeout of 5 seconds was applied to all test cases. In the V9 Service Pack 2 release, Volt MX Iris has introduced the Timeout feature in the Testcase Recorder window that allows you to configure the timeout value for each test case. This feature enables developers to identify the timeout value for each test case and then configure the timeout value.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/TestAutomation.md#timeout).

### View Screenshots of Failed Expectations

From Volt MX Iris V9 Service Pack 2, you can view the details of all the failed expectations of Jasmine Test Automation in the Results window of the Automator. The Results window displays a list of all the failed expectations along with the name of the test case, line in code, column number, test message, stack trace, and the screenshot of the failure.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/TestAutomation.md#screenshot).

### Add Assertions in Test Case Recordings

The Test Recorder in Volt MX Iris now supports all the assertion types provided by Jasmine Test Automation.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/TestAutomation.md#Assertion).

### Automatically Add WaitFor for a New Test Case

From Volt MX Iris V9 Service Pack 2, when a user performs an action to Navigate to a new form, the Test Case Recorder automatically adds the waitFor statement during the recording to ensure that the test execution considers the wait time for the form load.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/TestAutomation.md#waitforauto).

Android Enhancements
--------------------

### Support for Android Target SDK 30

Support for the Android R (API level 30) Target SDK has been added in Volt MX Iris.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/AndroidR_Behavioral_Changes.md).

### Support for 5G Network APIs

As the Android Framework has provided support for 5G network connection, Volt MX Iris has introduced support for the following 5G Network APIs

*   [voltmx.net.set5GNetworkListener](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md#set5GNetworkListener)
*   [voltmx.net.unregister5GNetworkListener](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md#unregister5GNetworkListener)
*   [voltmx.net.hasCapablity](../../../Iris/iris_api_dev_guide/content/voltmx.net_functions.md#hasCapability)

### Background Location Access

Apps that run on Android 11 (API level 30, or later) devices must already have access to foreground location before requesting for background location access. If the user denies permission for background location access, you can provide an educational UI to the user by using the [voltmx.application.getBackgroundPermissionOptionLabel](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions_runtimepermissionsapi.md#getBackgroundPermissionOptionLabel) API. The API provides the text for the option that educates the user to grant background access permission.

### GeoLocation API Enhancements

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [voltmx.location.checkLocationSettings](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#checkLocationSettings) API that allows you to check whether the current location settings meet the desired accuracy settings. In addition, support for the [accuracyMode](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#accuracyMode), [requestModifyLocationSettings](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#requestModifyLocationSettings), and [improveBGLocationUpdateFrequency](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#improveBGLocationUpdateFrequency) parameters have been added in the positionoptions parameter of the [voltmx.location.getCurrentPosition](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#getCurrentPosition) and the [voltmx.location.watchPosition](../../../Iris/iris_api_dev_guide/content/voltmx.location_functions.md#watchPosition) APIs.

### Package Visibility Updates

Android 11 introduces restrictions on how apps query and interact with other apps installed on a device. Apps must use the `<queries>` element to define other packages that the app can interact with. In addition, you must add the `<queries>` element in the Android Manifest Entries to view a filtered list of email applications while using the [filterEmailAppsOnly](../../../Iris/iris_api_dev_guide/content/voltmx.phone_functions.md#filterEmailAppsOnly) parameter of the [voltmx.phone.openEmail](../../../Iris/iris_api_dev_guide/content/voltmx.phone_functions.md#phone.op2) API. Further, when you build an app in **Protected Mode**, you must add the `donotAddQueryAllPackages = true` entry in the **androidbuild.properties** file to disable the automatic addition of the QUERY\_ALL\_PACKAGES permission in the Android Manifest file.

For more information on this feature, click [here](../../../Iris/iris_user_guide/Content/Native_App_Properties.md#PackageVisibility).

### Support for SafetyNet APIs

Support for the following set of SafetyNet APIs has been added as part of the Volt MX Iris V9 ServicePack 2 release:

*   Attestation API
    
    *   [voltmx.safetynet.attest](../../../Iris/iris_api_dev_guide/content/safetynetapi.md#attest)
*   Verify Apps API
    
    *   [voltmx.safetynet.isVerifyAppsEnabled](../../../Iris/iris_api_dev_guide/content/safetynetapi.md#isVerifyAppsEnabled)
    *   [voltmx.safetynet.enableVerifyApps](../../../Iris/iris_api_dev_guide/content/safetynetapi.md#enableVerifyApps)
    *   [voltmx.safetynet.listHarmfulApps](../../../Iris/iris_api_dev_guide/content/safetynetapi.md#listHarmfulApps)

For more information on this feature, click [here](../../../Iris/iris_api_dev_guide/content/safetynetapi.md).

### Auto-Reset Permissions

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [voltmx.application.isAutoRevokeWhitelisted](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions_runtimepermissionsapi.md#isAutoRevokeWhitelisted) API that helps users determine whether an application is exempt from having its permissions be automatically revoked when the app is unused for an extended period of time.

### Authenticate using Device Credentials

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the **constants.LOCAL\_AUTHENTICATION\_MODE\_DEVICE\_CREDENTIALS** as an Authentication Mode constant has been added in the [voltmx.localAuthentication.getStatusForAuthenticationMode](../../../Iris/iris_api_dev_guide/content/voltmx.localauthentication_functions.md#getStatusForAuthenticationMode) API. This constant determines whether the device has either PIN, PATTERN, or PASSWORD configured as the authentication mode.

Support for Widget Extensions
-----------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support to customize existing Flare Volt MX widgets by using the [voltmx.ui.defineExtendedWidge](../../../Iris/iris_api_dev_guide/content/voltmx.ui_functions.md#ExtendedWidget)t API to create a new widget with additional functionality. Once you create the custom widget, you can use it as a regular widget across your project.

Sign In With Apple
------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support for the [SigninWithApple widget](../../../Iris/iris_widget_prog_guide/Content/SigninWithApple.md) that enables application users to sign in to apps and websites by using their Apple ID. Use the voltmx.ui.signInWithApple to create the SigninWithApple widget. You can then use the [voltmx.signInWithApple.evaluateCredentialStateforUserID](../../../Iris/iris_api_dev_guide/content/voltmx.signinwithapple_functions.md#evaluateCredentialStateforUserID) to get the current state of an opaque user ID that was specified previously.

For more information on this feature, click [here](../../../Iris/iris_api_dev_guide/content/signinwithapple_api.md).

Calendar Enhancements for Responsive Web
----------------------------------------

Prior to the Volt MX Iris V9 Service Pack 2 release, you had to click the Calendar icon, and then click the month or year from a grid view, and then confirm the selections. From Volt MX Iris V9 Service Pack 2, the Calendar widget has been enhanced with a new look that lets you select the month and year from drop-down lists. Additionally, support for the following attributes has been added in the viewConfig property of the Calendar widget:

*   [gridCellHoverSkin](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#gridCellHoverSkin)
*   [gridMonthYearHoverSkin](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#gridMonthYearHoverSkin)
*   [gridMonthYearSelectedSkin](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#gridMonthYearSelectedSkin)
*   [monthYearDone](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#monthYearDone)
*   [monthYearCancel](../../../Iris/iris_widget_prog_guide/Content/Calendar_Properties.md#monthYearCancel)

 

In addition, the [calendarMonthYearSelectionDropdownView](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#DropdownView) parameter has been added in the [voltmx.application.setApplicationBehaviors](../../../Iris/iris_api_dev_guide/content/voltmx.application_functions.md#voltmx.app5) API. This parameter allows you to enable or disable the new look of Calendar widget.

ListBox Widget Enhancements
---------------------------

Enhancements have been made to the ListBox widget on the Desktop Web channel to provide the same capabilities as a ListBox widget on the Mobile Native channel. In the V9 Service Pack 2 release, Volt MX Iris introduces support for the following properties to enable the addition of Skins to the ListBox items on the Desktop Web channel:

*   [disabledKeys](../../../Iris/iris_widget_prog_guide/Content/ListBox_Basic_Properties.md#disabledKeys)
*   [itemDisabledSkin](../../../Iris/iris_widget_prog_guide/Content/ListBox_Basic_Properties.md#itemDisabledSkin)
*   [itemHoverSkin](../../../Iris/iris_widget_prog_guide/Content/ListBox_Basic_Properties.md#itemHoverSkin)
*   [itemNormalSkin](../../../Iris/iris_widget_prog_guide/Content/ListBox_Basic_Properties.md#itemNormalSkin)

zIndex Support for Map Methods
------------------------------

In the V9 Service Pack 2 release, Volt MX Iris introduces support to provide the zIndex for the pins and shapes added to maps. While using the Map widget, you can add the zIndex parameter to the following methods:

*   [addPin](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexaddPin)
*   [addPins](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexaddPins)
*   [addPolygon](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexaddPolygon)
*   [addPolyline](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexaddPolyline)
*   [addCircle](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexaddCircle)
*   [updatePin](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexupdatePin)
*   [updatePins](../../../Iris/iris_widget_prog_guide/Content/Map_Methods.md#zIndexupdatePins)

Text Widget Enhancement
-----------------------

*   ### Support for textCopyable property
    
    In the V9 Service Pack 2 release, Volt MX Iris introduces support for the **textCopyable** property for the [TextBox](../../../Iris/iris_widget_prog_guide/Content/TextBox_Properties.md#textCopyable1) and [TextArea](../../../Iris/iris_widget_prog_guide/Content/TextArea_Properties.md#textCopyable) widgets. By using this property, you can enable or disable the cut, copy and paste actions on the text entered in the TextBox and TextArea widgets.
    
*   The Desktop Web platform now supports the following properties of the TextBox and TextArea widgets:
    *   [autoCapitalize](../../../Iris/iris_widget_prog_guide/Content/TextArea_Properties.md#autoCapitalize) Property
    *   [restrictCharactersSet](../../../Iris/iris_widget_prog_guide/Content/TextArea_Properties.md#restrictCharactersSet) Property
    *   [textInputMode](../../../Iris/iris_widget_prog_guide/Content/TextArea_Properties.md#textInputmode) Property
