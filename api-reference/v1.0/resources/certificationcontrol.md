---
title: certificationControl 资源类型
description: 此资源包含与安全分数控制相关联的合规性认证数据。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629311"
---
#  <a name="certificationcontrol-resource-type"></a>certificationControl 资源类型

包含与安全得分控制相关联的合规性认证数据。

## <a name="properties"></a>属性

|属性 |类型 |说明 |
|:--|:--|:--|
|name|字符串|证书控制名称 |
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
