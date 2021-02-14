---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: itemPreviewInfo 资源包含有关如何嵌入 driveItem 预览的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240568"
---
# <a name="itempreviewinfo-resource-type"></a>itemPreviewInfo 资源类型

命名空间：microsoft.graph

**itemPreviewInfo** 资源包含有关如何嵌入 [driveItem](driveitem.md)预览的信息。

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
| getUrl         | string | 适合使用 HTTP GET (iframe 等嵌入的 URL) 
| postUrl        | string | 适合使用 HTTP POST 和表单 (JS 等嵌入的 URL) 
| postParameters | string | 使用 postUrl 时要包含的 POST 参数

可能会返回 getUrl、postUrl 或两者，具体取决于指定选项的当前支持状态。

postParameters 是格式设置为的字符串，如果对 postUrl 执行 `application/x-www-form-urlencoded` POST，应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

URL 和参数的格式应视为不透明。

