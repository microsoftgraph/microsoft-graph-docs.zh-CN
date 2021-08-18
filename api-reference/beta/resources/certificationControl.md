---
title: " certificationControl 资源类型"
description: 此资源包含与安全分数控制关联的合规性认证数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: ae7634ed168870bd03282a9a20dc9cba536db0635d750d07d17407f85a9e8c8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164354"
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


