---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5751ea8a389315e46efe1ead5149bf7e6cd7596
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731573"
---
# <a name="ipv4range-resource-type"></a>iPv4Range 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

IPv4 范围定义。


继承自 [ipRange](../resources/intune-mam-iprange.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lowerAddress|String|较低地址。|
|upperAddress|String|上地址。|

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





