---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20d7c24c887ca97f3a5a9890f5089b745130055e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777873"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

令牌中给定应用的许可证摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|vppTokenId|String|VPP 令牌的标识符。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|organizationName|String|与 Apple Volume Purchase Program 令牌关联的组织。|
|availableLicenseCount|Int32|可用的 VPP 许可证数。|
|usedLicenseCount|Int32|使用中的 VPP 许可证数量。|

## <a name="relationships"></a>关系
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



