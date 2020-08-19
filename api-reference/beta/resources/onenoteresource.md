---
title: onenoteResource 资源类型
description: 'OneNote 页面上的图像或其他文件资源。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: fc4f3962e5be1eeb69598548067b61aa86c9c246
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806273"
---
# <a name="onenoteresource-resource-type"></a>onenoteResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote 页面上的图像或其他文件资源。

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
通过向资源的终结点发送 GET 请求获取特定资源的二进制数据 `content` ：

```
GET ../onenote/resources/{id}/content
```

当您使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：

```
GET ../onenote/pages/{id}/content
```

在页面 HTML 中， `img` 标记包含属性中的原始图像资源 `data-fullres-src` 和属性中优化的图像的终结点 `src` ：
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

一个 `object` 代表文件（如 PDF、.docx 和 PNG）的标记 () 在属性中包含文件资源的终结点 `data` ：

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| 内容 | Edm||
| contentUrl | String ||

## <a name="relationships"></a>关系
无。


## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取资源二进制数据](../api/resource-get.md) | Stream |检索文件或图像资源的二进制数据。|

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
