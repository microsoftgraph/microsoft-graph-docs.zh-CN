---
title: 网站资源类型
description: 表示网站。
ms.localizationpriority: medium
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c0daa5106f70f049d070968749e5a7d391783d59
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134211"
---
# <a name="website-resource-type"></a>网站资源类型

命名空间：microsoft.graph

表示网站。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|类型|websiteType| 可能的值包括 `other`、`home`、`work`、`blog`、`profile`。|
|address|string|网站的 URL。|
|displayName|string|显示名称的网站集。|

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

