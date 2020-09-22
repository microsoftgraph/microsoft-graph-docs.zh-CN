---
author: kevinlam
description: ItemPreviewInfo 资源包含有关如何嵌入 DriveItem 的预览的信息。
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab62e2a41d257adcb8f763b77e42f0d7e515ee5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033692"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemPreviewInfo**资源包含有关如何嵌入[DriveItem](driveitem.md)的预览的信息。

## <a name="json-representation"></a>JSON 表示形式

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>属性

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适用于使用 HTTP GET (iframe 等嵌入的 URL ) 
| postUrl        | string | 适合使用 HTTP POST (表单 post、JS 等进行嵌入的 URL ) 
| postParameters | string | 如果使用 postUrl，则发布要包括的参数

根据指定选项的当前支持状态，可能会返回 getUrl、postUrl 或 both。

postParameters 是格式为的字符串 `application/x-www-form-urlencoded` ，如果向 postUrl 执行 POST，应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Url 和参数的格式应被认为是不透明的。


