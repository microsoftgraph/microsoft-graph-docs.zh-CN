---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f6ecfa2ffddd362ba6c166d9dc839aedaf6f4723
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810578"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl 资源类型

命名空间：microsoft.graph

包含与安全得分控制相关联的合规性认证数据。

|属性 |类型 |说明 |
|:--|:--|:--|
|name | string | 证书控制名称 |
|url | string | Microsoft 服务信任门户的 URL |

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
