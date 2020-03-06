---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d75c82cfdd53d1df51537980487e7f7ed780414
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530820"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的设备符合性策略设置状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|setting|字符串|报告的设置|
|settingName|字符串|报告的本地化/用户友好设置名称|
|instanceDisplayName|字符串|报告的设置实例的名称。|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|设置的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|errorCode|Int64|设置的错误代码|
|errorDescription|字符串|错误说明|
|userId|String|UserId|
|userName|字符串|UserName|
|userEmail|字符串|UserEmail|
|userPrincipalName|字符串|UserPrincipalName。|
|源|[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合|参与策略|
|currentValue|String|设备上设置的当前值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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




