---
title: " certificationControl 资源类型"
description: 此资源包含合规性与关联的证书数据安全分数控件。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810386"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl 资源类型

包含合规性与关联的证书数据安全分数控件。

|属性 |类型 |说明 |
|:--|:--|:--|
|name | string | 证书控件名称 |
|url | string | Microsoft 服务的 URL 信任门户 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
