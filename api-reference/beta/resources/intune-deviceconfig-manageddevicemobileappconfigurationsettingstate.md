---
title: managedDeviceMobileAppConfigurationSettingState 资源类型
description: 给定设备的托管设备移动应用配置设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9e74a4fb9b6739d5051e37af4c15c48ede6bda1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302836"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a>managedDeviceMobileAppConfigurationSettingState 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的托管设备移动应用配置设置状态。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|setting|String|报告的设置|
|settingName|String|报告的本地化/用户友好设置名称|
|instanceDisplayName|String|报告的设置实例的名称。|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|设置的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|errorCode|Int64|设置的错误代码|
|errorDescription|String|错误说明|
|userId|字符串|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|字符串|UserPrincipalName。|
|源|[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合|参与策略|
|currentValue|String|设备上设置的当前值|
|settingInstanceId|字符串|SettingInstanceId|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```




