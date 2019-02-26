---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c126323e0f5785752238ec64cfade2c34d5c24
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161059"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

令牌中给定应用的许可证摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|vppTokenId|String|VPP 令牌的标识符。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|organizationName|String|与 Apple volume purchase Program 令牌关联的组织。|
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




