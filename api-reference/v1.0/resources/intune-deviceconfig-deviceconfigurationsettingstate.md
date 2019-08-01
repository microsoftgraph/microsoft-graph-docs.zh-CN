---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50ed17421b88f2cb6137458ff853bfa92796c2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031666"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>deviceConfigurationSettingState 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的设备配置设置状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|setting|String|报告的设置|
|settingName|String|报告的本地化/用户友好设置名称|
|instanceDisplayName|String|报告的设置实例的名称。|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|设置的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|errorCode|Int64|设置的错误代码|
|errorDescription|String|错误说明|
|userId|String|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|字符串|UserPrincipalName。|
|源|[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合|参与策略|
|currentValue|String|设备上设置的当前值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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
```



