---
title: "mobileAppTroubleshootingAppTargetHistory resource type"
description: "History Item contained in the Mobile App Troubleshooting Event."
author: "rolyon"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# mobileAppTroubleshootingAppTargetHistory resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

History Item contained in the Mobile App Troubleshooting Event.


Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|Time when the history item occurred. Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|securityGroupId|String|AAD security group id to which it was targeted.|
|runState|[runState](../resources/intune-shared-runstate.md)|Status of the item. Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.|
|errorCode|String|Error code for the failure, empty if no failure.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



