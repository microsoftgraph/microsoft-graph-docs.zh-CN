---
title: patchContentCommand 资源类型
description: 对修补程序请求中的 OneNote 页面进行的更改。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 798eb15955ddbbed3ced2f85d091d06c5ee1d84d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998122"
---
# <a name="patchcontentcommand-resource-type"></a>patchContentCommand 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对修补程序请求中的 OneNote 页面进行的更改。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式，它是在 [修补程序页/{id} '](../api/page-update.md) 请求的正文中发送的。

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
|action|String|要在目标元素上执行的操作。 可取值为：`replace`、`append`、`delete`、`insert` 或 `prepend`。|
|内容|String|要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。 如果内容包含二进制数据，则必须使用 `multipart/form-data` 包含 "命令" 部分的内容类型发送该请求。 |
|position|String|要添加所提供的内容的位置，与目标元素有关。 可能的值包括： `after` (默认) 或 `before` 。|
|target|String|要更新的元素。 必须是 `#<data-id>` 或生成 `{id}` 的元素，或 `body` 或 `title` 关键字。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


