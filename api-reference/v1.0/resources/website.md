---
title: 网站资源类型
description: 表示网站。
ms.localizationpriority: medium
author: AAmatino
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: f63aba19d6f3e0e942ad35f445b43ed7b1bff1e3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899664"
---
# <a name="website-resource-type"></a>网站资源类型

命名空间：microsoft.graph

表示网站。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|类型|websiteType| 可能的值包括 `other`、`home`、`work`、`blog`、`profile`。|
|address|string|网站的 URL。|
|displayName|string|网站的显示名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

