---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31301b045d69302e90bec38901c9236abab77418
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030058"
---
# <a name="ipv4range-resource-type"></a>iPv4Range 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

IPv4 范围定义。


继承自 [ipRange](../resources/intune-shared-iprange.md)

## <a name="properties"></a>属性
|属性|类型|描述|
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



