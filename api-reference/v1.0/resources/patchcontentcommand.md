---
title: patchContentCommand 资源类型
description: PATCH 请求中要对 OneNote 页面进行的更改。
ms.openlocfilehash: bfbdceeda0294540f701f9fa458030834e7d7850
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008670"
---
# <a name="patchcontentcommand-resource-type"></a>patchContentCommand 资源类型

PATCH 请求中要对 OneNote 页面进行的更改。

## <a name="json-representation"></a>JSON 表示形式

其是 [PATCH pages/{id}`](../api/page-update.md) 请求的正文中发送的资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|action|onenotePatchActionType|要在目标元素上执行的操作。 可能的值为： `replace`， `append`， `delete`， `insert`，或`prepend`。|
|content|String|要添加到页面的格式标准的 HTML 字符串或任意图片或二进制文件数据。如果内容包含二进制数据，则必须使用包含“Commands”部分的 `multipart/form-data` 内容类型发送请求。 |
|position|onenotePatchInsertPosition|要添加所提供内容的位置，与目标元素相对。 可能的值为： `after` （默认值） 或`before`。|
|target|字符串|要更新的元素。必须为 `#<data-id>` 或元素生成的 `<id>`，或 `body` 或 `title` 关键词。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
