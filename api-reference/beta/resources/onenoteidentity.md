---
title: oneNoteIdentity 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0a7df80dd3dcd4f4b93edb4e708e65de3f74d775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966445"
---
# <a name="onenoteidentity-resource-type"></a>oneNoteIdentity 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**支持即将推出**

OneNoteIdentity 类型表示_用户_的标识。

将来, 此类型将与[标识](identity.md)合并


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|此身份的显示名称。|
|id|string|身份的唯一标识符。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
