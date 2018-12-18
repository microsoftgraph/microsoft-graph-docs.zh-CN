---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: tfitzmac
ms.openlocfilehash: fbad84edffaeb3abdff0c00fdd55c1451d23a721
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327956"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

给定设备的设备符合性策略设置状态。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|setting|String|报告的设置|
|settingName|String|报告的本地化/用户友好设置名称|
|instanceDisplayName|String|报告的设置实例的名称。|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|设置合规性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|errorCode|Int64|设置的错误代码|
|errorDescription|String|错误说明|
|userId|String|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|String|UserPrincipalName。|
|sources|[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合|参与策略|
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





