---
title: managedDeviceMobileAppConfigurationState 资源类型
description: 给定设备的托管设备移动应用配置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3faa3547af9337483f0ded1306e7a64321d345a6
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636069"
---
# <a name="manageddevicemobileappconfigurationstate-resource-type"></a>managedDeviceMobileAppConfigurationState 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的托管设备移动应用配置状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceMobileAppConfigurationStates](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-list.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)集合|列出[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)对象的属性和关系。|
|[获取 managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-get.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|读取[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)对象的属性和关系。|
|[创建 managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-create.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|创建新的[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)对象。|
|[删除 managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-delete.md)|无|删除[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)。|
|[更新 managedDeviceMobileAppConfigurationState](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-update.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|更新[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|settingStates|[managedDeviceMobileAppConfigurationSettingState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationSettingState.md)集合|**TODO：添加说明。**|
|displayName|String|此 policyBase 的策略名称|
|version|Int32|策略版本|
|platformType|[policyPlatformType](../resources/intune-shared-policyPlatformType.md)|应用该策略的平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。|
|state|[complianceStatus](../resources/intune-shared-complianceStatus.md)|策略的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|settingCount|Int32|策略保留的设置计数|
|userId|String|用户唯一标识符，必须为 Guid|
|userPrincipalName|字符串|用户主体名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024,
  "userId": "String",
  "userPrincipalName": "String"
}
```

