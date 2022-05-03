---
title: patchContentCommand 资源类型
description: 在 PATCH 请求中对OneNote页所做的更改。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: jewan-microsoft
ms.openlocfilehash: 11155779f5765e098a566589b522f9e987d6a68d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176777"
---
# <a name="patchcontentcommand-resource-type"></a>patchContentCommand 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 PATCH 请求中对OneNote页所做的更改。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式，该表示形式在 [PATCH 页面/{id}](../api/page-update.md) 请求的正文中发送。

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
|内容|String|要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。 如果内容包含二进制数据，则必须使用 `multipart/form-data` 包含“命令”部分的内容类型发送请求。 |
|position|String|要添加所提供的内容的位置，与目标元素有关。 可能的值为： `after` (默认) 或 `before`。|
|target|String|要更新的元素。 必须是`#<data-id>`元素的或生成`{id}`的，或者`body``title`是关键字。|

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


