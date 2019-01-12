---
title: educationOneNoteResource 资源类型
description: 'EducationResource 一个子类。 这表示在 OneNote 页面的位置。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b10bef551cdc2dd29a8a20c69d2c4657ee66af4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927917"
---
# <a name="educationonenoteresource-resource-type"></a>educationOneNoteResource 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[EducationResource](educationresource.md)一个子类。 这表示在 OneNote 页面的位置。  

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|pageUrl|字符串|在 OneNote 中页的 Microsoft Graph URL。|
|sectionName|字符串|分配应复制到或已复制到的部分名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
