---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7fc8ef3ecc436580c14150df472971144b5197d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356448"
---
# <a name="ipv4range-resource-type"></a>iPv4Range 资源类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

IPv4 范围定义。


继承自 [ipRange](../resources/intune-mam-iprange.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lowerAddress|String|较低的地址。|
|upperAddress|String|地址上限。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




