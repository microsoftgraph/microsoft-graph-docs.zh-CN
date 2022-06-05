---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制关联的符合性认证数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: dd18b83f6f370caabe3d6518f7d9e2d92241f1d3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900203"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性认证数据。

|属性 |类型 |说明 |
|:--|:--|:--|
|name | string | 认证控制名称 |
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


