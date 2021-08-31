---
title: vppTokenLicenseSummary 资源类型
description: 令牌中给定应用的许可证摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 916891d0bd87796007805850cb54bc04cb9dad6d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789889"
---
# <a name="vpptokenlicensesummary-resource-type"></a>vppTokenLicenseSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

令牌中给定应用的许可证摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|vppTokenId|String|VPP 令牌的标识符。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|organizationName|String|与 Apple Volume Purchase Program 令牌关联的组织。|
|availableLicenseCount|Int32|可用 VPP 许可证的数量。|
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



