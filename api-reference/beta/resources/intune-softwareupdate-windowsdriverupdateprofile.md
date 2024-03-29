---
title: windowsDriverUpdateProfile 资源类型
description: Windows 驱动程序更新配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f5001b471fb635a5b4d21c8bd1c2c6ead6442606
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629755"
---
# <a name="windowsdriverupdateprofile-resource-type"></a>windowsDriverUpdateProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 驱动程序更新配置文件

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDriverUpdateProfiles](../api/intune-softwareupdate-windowsdriverupdateprofile-list.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 集合|列出 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 对象的属性和关系。|
|[获取 windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-get.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|读取 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 对象的属性和关系。|
|[创建 windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-create.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|创建新的 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 对象。|
|[删除 windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-delete.md)|无|删除 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)。|
|[更新 windowsDriverUpdateProfile](../api/intune-softwareupdate-windowsdriverupdateprofile-update.md)|[windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)|更新 [windowsDriverUpdateProfile 对象](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 的属性。|
|[分配操作](../api/intune-softwareupdate-windowsdriverupdateprofile-assign.md)|无|尚未记录|
|[executeAction 操作](../api/intune-softwareupdate-windowsdriverupdateprofile-executeaction.md)|[bulkDriverActionResult](../resources/intune-softwareupdate-bulkdriveractionresult.md)|尚未记录|
|[syncInventory 操作](../api/intune-softwareupdate-windowsdriverupdateprofile-syncinventory.md)|无|同步 WindowsDriverUpdateProfile 的驱动程序清单。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略Intune ID。|
|displayName|String|配置文件显示名称的配置文件。|
|说明|String|由用户指定的配置文件的说明。|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|驱动程序更新配置文件审批类型。 例如，手动或自动审批。 可取值为：`manual`、`automatic`。|
|deviceReporting|Int32|此配置文件的报告设备数|
|newUpdates|Int32|可用于此配置文件的新驱动程序更新数。|
|deploymentDeferralInDays|Int32|部署延迟设置（以天表示）仅在 ApprovalType 设置为自动审批时适用。|
|createdDateTime|DateTimeOffset|创建配置文件的日期时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改配置文件的日期时间。|
|roleScopeTagIds|String 集合|此驱动程序更新实体的范围标记列表。|
|inventorySyncStatus|[windowsDriverUpdateProfileInventorySyncStatus](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstatus.md)|此配置文件的驱动程序清单同步状态。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[windowsDriverUpdateProfileAssignment](../resources/intune-softwareupdate-windowsdriverupdateprofileassignment.md) 集合|配置文件的组分配列表。|
|driverInventories|[windowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) 集合|此配置文件的驱动程序清单。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "approvalType": "String",
  "deviceReporting": 1024,
  "newUpdates": 1024,
  "deploymentDeferralInDays": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "inventorySyncStatus": {
    "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
    "lastSuccessfulSyncDateTime": "String (timestamp)",
    "driverInventorySyncState": "String"
  }
}
```




