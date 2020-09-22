---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f2be439f1b286a8d916fe80a7b4fcb4f6d60071
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016819"
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


