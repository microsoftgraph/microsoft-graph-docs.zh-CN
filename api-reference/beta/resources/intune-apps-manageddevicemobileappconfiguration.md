---
title: managedDeviceMobileAppConfiguration 资源类型
description: 已注册设备移动应用配置的抽象类
ms.openlocfilehash: c829e720e8d998428e778e5b7bf20e5fe465dfd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041366"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a>managedDeviceMobileAppConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

已注册设备移动应用配置的抽象类
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedDeviceMobileAppConfigurations](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合|列出 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。|
|[Get managedDeviceMobileAppConfiguration](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|读取 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 对象的属性和关系。|
|[assign 操作](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|targetedMobileApps|String 集合|关联的应用。|
|roleScopeTagIds|String 集合|此应用程序配置实体范围标记的列表。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|description|String|管理员提供的设备配置说明。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|管理员提供的设备配置名称。|
|version|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 集合|应用配置的组分配列表。|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合|ManagedDeviceMobileAppConfigurationDeviceStatus 的列表。|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合|ManagedDeviceMobileAppConfigurationUserStatus 列表|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|应用配置设备状态摘要。|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|应用配置用户状态摘要。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





