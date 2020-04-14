---
title: restrictedAppsViolation 资源类型
description: 每个用户的每个设备违反受限制的应用配置文件
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae4212ce13a71f33d493de61e00a321577b8d16a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444921"
---
# <a name="restrictedappsviolation-resource-type"></a>restrictedAppsViolation 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个用户的每个设备违反受限制的应用配置文件

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合|列出[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性和关系。|
|[获取 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|读取[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性和关系。|
|[创建 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。|
|[删除 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|无|删除[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。|
|[更新 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|对象的唯一标识符。 由 accountId、deviceId、policyId 和 userId 组成|
|userId|String|用户唯一标识符，必须为 Guid|
|userName|String|用户名|
|managedDeviceId|String|托管设备唯一标识符，必须为 Guid|
|deviceName|String|设备名称|
|deviceConfigurationId|String|设备配置文件唯一标识符，必须为 Guid|
|deviceConfigurationName|String|设备配置文件名称|
|platformType|[policyPlatformType](../resources/intune-shared-policyplatformtype.md)|平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|受限制的应用程序状态。 可取值为：`prohibitedApps`、`notApprovedApps`。|
|restrictedApps|[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合|违反受限制的应用程序的列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```



