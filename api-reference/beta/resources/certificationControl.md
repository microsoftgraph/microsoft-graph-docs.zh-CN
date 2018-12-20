---
title: " certificationControl 资源类型"
description: 此资源包含合规性与关联的证书数据安全分数控件。
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380943"
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
