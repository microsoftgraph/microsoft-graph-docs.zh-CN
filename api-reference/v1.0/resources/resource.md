---
title: oneNoteResource 资源类型
description: 'OneNote页上的图像或其他文件资源。 '
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: e304bdcee171350ade75b6253d12e3abfac77856
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034885"
---
# <a name="onenoteresource-resource-type"></a>oneNoteResource 资源类型

命名空间：microsoft.graph

OneNote页上的图像或其他文件资源。

可以获取资源的二进制数据，但不支持获取资源对象或资源集合的 JSON 表示形式。

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

通过将 GET 请求发送到资源的终结点来获取特定资源的 `content` 二进制数据：

```
GET ../onenote/resources/{id}/content
```

使用以下请求获取页面的 HTML 内容时，将返回文件的资源 URI：

```
GET ../onenote/pages/{id}/content
```

在页面 HTML 中， `img` 标记包含属性中原始映像资源的 `data-fullres-src` 终结点和属性中的 `src` 优化映像：
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

表示 `object` PDF、DOCX 和 PNG) 等文件的标记 (包含属性中文件资源的 `data` 终结点：

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

