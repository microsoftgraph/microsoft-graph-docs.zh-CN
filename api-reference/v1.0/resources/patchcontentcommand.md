---
title: patchContentCommand 资源类型
description: 对 PATCH 请求中的OneNote页所做的更改。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0b34271f08cc8f8e234c6a10ecd28229ddbce451ca0f54b26197bc1a9d02f56f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205252"
---
# <a name="patchcontentcommand-resource-type"></a>patchContentCommand 资源类型

命名空间：microsoft.graph

对 PATCH 请求中的OneNote页所做的更改。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式，在 [PATCH 页面/{id}](../api/page-update.md) 请求的正文中发送。

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
|action|onenotePatchActionType|要在目标元素上执行的操作。 可能的值包括 `replace` `append` ：、、、 `delete` `insert` 或 `prepend` 。|
|内容|String|要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。 如果内容包含二进制数据，则必须使用包含 `multipart/form-data` "Commands"部分的内容类型发送请求。 |
|position|onenotePatchInsertPosition|要添加所提供的内容的位置，与目标元素有关。 可能的值包括： `after` 默认 (或) `before` 。|
|target|String|要更新的元素。 必须是 `#<data-id>` 元素的 或 生成的 `<id>` ，或者是 `body` 或 `title` 关键字。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

