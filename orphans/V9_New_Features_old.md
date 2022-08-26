                          

Volt MX  Foundry V9 Release Notes
============================

Console
-------

*   **Added a new Operation Security level**
    
    Select **Private** from the Operation Security level to indicate that the current operation will be accessible only by other operations or services in the same account.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/XML.md).
    
*   **Added support for the parameter prompt**
    
    As part of OIDC authorization to improve the logout flow while using the OAuth Provider.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Identity11_OAuth.md).
    
*   Added support for sending push notification to EAS.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/PushNotificationsEas.md).
    
*   Added support to create the app service document based on the **alias hostname**.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Publish_LifeCycle.md#app-service-document-object-services-metadata-and-sync-client-code).
    
*   Added support for **Enumeration Datatype**.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/ObjectsServices/enumDatatypes.md).
    
*   **Added ability to rotate appkeys**
    
    Different appkeys for web and native with ability to rotate keys.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/SeparateAppKey-Secret.md).
    
*   Added support to access custom features of Volt MX Foundry environments.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Settings_Cloud.md#users-cloud).
    
*   Simplified the object model definition - field names and types.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/ObjectsServices/Stage_2.md#creating-objects-39-definition-and-map-to-back-end-objects-manually).
    
*   Support to generate Object model by importing an MS Excel file, for Storage.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/ObjectsServices/Storage_ObjectServices.md).
    
*   Added support to download the reconfigurations made to an app before publishing.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Publish_LifeCycle.md).
    

Identity
--------

*   **Support to enable and disable integrity check**
    
    For certain identity services to enable the server for server communication.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Identity2_MS_AD.md).
    
*   **Enhanced the custom identity adapter**
    
    For supporting additional pass-through endpoints like user attributes, security attributes, and MFA.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Identity8_VoltMX_Custom.md#custom-identity-service).
    
*   **Added support for Sign-Up in Volt MX User Repository**
    
    The Sign-up option allows the user to sign-up or register to the application by using their e-mail ID.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/sign-Up_User_Flow.md).
    

Admin Console
-------------

*   **Added Throttling configuration**
    
    A new field is added in Admin Console > Runtime Configuration to configure the throttling at service operation level.
    
    For more information about this feature, click [here](../../../Foundry/vmf_integrationservice_admin_console_userguide/Content/Runtime_Configuration.md).
    
*   **Added Server Monitoring**.
    
    For more information about this feature, click [here](../../../Foundry/vmf_integrationservice_admin_console_userguide/Content/Server_Events_Monitoring.md).
    

Offline Objects
---------------

*   Added object-level support for clearing the offline data.  
    
    For more information about this feature, click [here](../../../Foundry/offline_objectsapi_reference_guide/Content/Object_clearOfflineData.md).
    

Analytics
---------

*   Added the On-Premise support for collecting metrics for child services of Integration/Orchestration services and offline objects.
    
    For more information about this feature, click [here](../../../Foundry/custom_metrics_and_reports/Content/Creating_a_Custom_Report.md).
    

Integration
-----------

*   **Improved the Service Definition UI of the RDBMS adapter**
    
    The User Interface of the RDBMS adapter's Service Definition page is improved for better user experience. The Database Driver Class and Connection URL boxes will now have pointers on how to fill these parameters.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/Relational_Database_Adapter.md).
    

App Factory
-----------

*   Jasmine testing framework has been added.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_appfactory_user_guide/Content/TestingAnAppJasmine.md).
    
*   Details to avoid deleting the `jenkins_github_ssh-certificates`, `jenkins_github_ssh-volt-mx-common`, and `jenkins_github_ssh-volt-mx-jenkins-job-DSL` SSH credentials have been provided, as they are system driven.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_appfactory_user_guide/Content/Working_with_AppFactory.md).
    

Engagement Services
-------------------

*   **Added support for App API Key**
    *   Added five new APIs: [Add](../../../Foundry/engagement_api_guide/Content/REST_API_Application/AddAppApiKey.md), [GetAppAPIKeys(s)](../../../Foundry/engagement_api_guide/Content/REST_API_Application/GetAppApiKey.md), [GetAppAPIKeyDetails](../../../Foundry/engagement_api_guide/Content/REST_API_Application/GetAppApiKeyDetails.md), [ModifyAppAPIKey](../../../Foundry/engagement_api_guide/Content/REST_API_Application/ModifyAppApiKey.md), and [DeleteAppAPIKey](../../../Foundry/engagement_api_guide/Content/REST_API_Application/DelAppApiKey.md).
    *   Added Manage App API Key support on the console.
        
        For more information about this feature, click [here](../../../Foundry/vms_console_user_guide/Content/Apps/AppAPIKey.md).  
        
*   **Enhanced the Email API** to be able to send email messages using a template ID.
    
    For more information about this feature, click [here](../../../Foundry/engagement_api_guide/Content/REST_API_Email/Email_API_With_Audience_Id___Email.md).
    
*   Added custom parameters to the Fetch Push API.
    
    For more information about this feature, click [here](../../../Foundry/engagement_api_guide/Content/Push_Message_APIs/Fetch_All_Messages_from_VoltMX_MobileFoundry_Engagement.md).
    

Installer
---------

*   **Support for New Versions of Software**
    
    Volt MX Foundry V9 installer supports new versions of several required software.
    
    *   Volt MX Foundry installer is bundled with an updated version of Tomcat 9.0.22.
    *   Support for installing Volt MX Foundry on MySQL 8.
    
    For more information about this feature, click [here](../../../Foundry/voltmx_foundry_user_guide/Content/ObjectsServices/Storage_ObjectServices.md).
    

Cloud Installer on MS Azure
---------------------------

*   Added Azure Redis Cache support for Identity Server.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/VoltMX_Foundry_on_Azure.md#configuration).
    
*   Added support for configuring auto-scalability for cluster.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/Appendices.md#aks-autoscaling).
    
*   Added support for configuring geographically redundant backup.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/VoltMX_Foundry_on_Azure.md#configuration).
    
*   Added support for Service Principle Object ID.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/VoltMX_Foundry_on_Azure.md#configuration).
    
*   Enhanced steps to use the Kubernetes Dashboard.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/Appendices.md#kubernetes-dashboard).
    
*   Added support for Pod anti-affinity.
    
    For more information about this feature, click [here](../../../Foundry/voltmxfoundry_on_azure/Content/Appendices.md#pod-anti-affinity).
