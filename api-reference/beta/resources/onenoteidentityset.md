---
title: oneNoteIdentitySet 资源类型
description: '**即将提供的支持**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642469"
---
# <a name="onenoteidentityset-resource-type"></a>oneNoteIdentitySet 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**即将提供的支持**

OneNoteIdentitySet 类型是键的[OneNoteIdentity](onenoteidentity.md)对象的集合。
它用于表示一套与各种事件关联的_笔记本_、_节_或_页_上，如_创建_或_上次修改者_的标识。 
 
当前，它包含单个键_**用户**_。  在将来，可能添加键如设备或应用程序更改的项。

将在将来，与[IdentitySet](identityset.md)合并此类型

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|表示用户 OneNoteIdentity 资源。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
