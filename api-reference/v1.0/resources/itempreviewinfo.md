---
author: kevinlam
title: itemPreviewInfo 资源类型
ms.localizationpriority: medium
description: 包含有关如何嵌入 driveItem 预览版的信息。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: d89f7ae60df58cb34891879fbc85c4e33cc9f8d7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899580"
---
# <a name="itempreviewinfo-resource-type"></a>itemPreviewInfo 资源类型

命名空间：microsoft.graph

包含有关如何嵌入 [driveItem](driveitem.md) 预览版的信息。

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
| getUrl         | string | 适用于使用 HTTP GET (iframe 等嵌入的 URL，) 
| postUrl        | string | 适用于使用 HTTP POST (表单文章、JS 等嵌入的 URL ) 
| postParameters | string | 使用 postUrl 时要包含的 POST 参数

getUrl、postUrl 或两者都可以返回，具体取决于指定选项的当前支持状态。

postParameters 是格式化为 `application/x-www-form-urlencoded`的字符串，如果对 postUrl 执行 POST，则应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

URL 和参数的格式应被视为不透明。

