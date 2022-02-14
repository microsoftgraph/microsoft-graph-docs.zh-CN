---
title: onenoteResource 资源类型
description: '页面图像或其他文件OneNote资源。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: f7a479ec529cae209fef085da2978c3e412a844f
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804918"
---
# <a name="onenoteresource-resource-type"></a>onenoteResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

页面图像或其他文件OneNote资源。

您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}
```

通过向资源的终结点发送 GET 请求，获取特定资源的二进制 `content` 数据：

```http
GET ../onenote/resources/{id}/content
```

当您通过以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：

```http
GET ../onenote/pages/{id}/content
```

在页面 HTML 中，标记 `img` 包括 属性 `data-fullres-src` 中原始图像资源的终结点和 属性中的 `src` 优化图像：

```html
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

一 `object` 个 (表示 PDF、DOCX 和 PNG 等文件的标记) 属性中包含文件资源的 `data` 终结点：

```html
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取资源二进制数据](../api/resource-get.md) | Stream |检索文件或图像资源的二进制数据。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| 内容 | Edm.Stream||
| contentUrl | 字符串 ||

## <a name="relationships"></a>关系
无。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


