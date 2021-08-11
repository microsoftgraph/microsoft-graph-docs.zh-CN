---
title: OneNoteResource 资源类型
description: '页面图像或其他文件OneNote资源。 '
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 39945f3086c8470dcbccc9d11a242d71df2a99dfd99977f147b2fcd180d69d24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218413"
---
# <a name="onenoteresource-resource-type"></a>OneNoteResource 资源类型

命名空间：microsoft.graph

页面图像或其他文件OneNote资源。

您可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

通过向资源的终结点发送 GET 请求，获取特定资源的二进制 `content` 数据：

```
GET ../onenote/resources/{id}/content
```

当您通过以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：

```
GET ../onenote/pages/{id}/content
```

在页面 HTML 中，标记包括 属性中原始图像资源的终结点和 属性 `img` `data-fullres-src` 中的优化 `src` 图像：
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

一个 (表示 PDF、DOCX 和 PNG 等文件的标记) 属性中包含 `object` 文件资源的 `data` 终结点：

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>属性

| 属性             | 类型            | 说明
|:---------------------|:----------------|:---------------------------------
| content              | 流          | 内容流
| contentUrl           | 字符串 (url)     | 用于下载内容的 URL

## <a name="relationships"></a>关系
无。


## <a name="methods"></a>方法
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取资源二进制数据](../api/resource-get.md) | Stream |检索文件或图像资源的二进制数据。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

