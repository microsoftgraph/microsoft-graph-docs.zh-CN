---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465522"
---
# <a name="ipv4range-resource-type"></a>iPv4Range 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

IPv4 范围定义。


继承自 [ipRange](../resources/intune-mam-iprange.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lowerAddress|字符串|较低的地址。|
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



