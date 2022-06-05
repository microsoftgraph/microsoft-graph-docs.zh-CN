---
title: certificationControl 资源类型
description: 此资源包含与安全分数控制关联的符合性认证数据。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 62a3fe7f2fc85a63108f2702a1612e7f6a771298
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899020"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl 资源类型

命名空间：microsoft.graph

包含与安全分数控制关联的合规性认证数据。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|name|字符串|认证控制名称 |
|url|String|Microsoft 服务信任门户的 URL |

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
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

