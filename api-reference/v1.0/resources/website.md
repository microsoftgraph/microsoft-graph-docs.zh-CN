---
title: 网站资源类型
description: 表示网站。
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6e237756f96df9ed0592ab38cf7af04e0fb43f90323e1b63ffc9902d4a329a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196458"
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

