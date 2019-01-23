---
title: restrictedAppsViolation 资源类型
description: 与每个每个用户的设备的受限的应用程序配置文件的冲突
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424978"
---
# <a name="restrictedappsviolation-resource-type"></a>restrictedAppsViolation 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与每个每个用户的设备的受限的应用程序配置文件的冲突

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合|列出属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象之间的关系。|
|[获取 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|读取属性和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的关系。|
|[创建 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。|
|[删除 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|无|删除[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)。|
|[更新 restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的唯一标识符。 由 accountId、 deviceId、 policyId 和用户 Id|
|userId|String|用户的唯一标识符，必须为 Guid|
|userName|String|用户名|
|managedDeviceId|String|托管的设备的唯一标识符，必须为 Guid|
|deviceName|String|设备名称|
|deviceConfigurationId|String|设备配置配置文件的唯一标识符，必须为 Guid|
|deviceConfigurationName|String|设备配置配置文件名称|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。|
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




