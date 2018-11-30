---
title: vppTokenLicenseSummary 资源类型
description: 许可证令牌中的给定应用程序的摘要。
ms.openlocfilehash: fba888c706b21a796615bf9bc2ea79968d5ad6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043130"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

许可证令牌中的给定应用程序的摘要。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|vppTokenId|字符串|VPP 令牌的标识符。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|organizationName|String|与 Apple 卷购买程序令牌关联的组织。|
|availableLicenseCount|Int32|VPP 可用的许可证数量。|
|usedLicenseCount|Int32|使用中的 VPP 许可证数量。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```





