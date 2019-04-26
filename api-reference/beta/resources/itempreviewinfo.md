---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: c43626292cd07ad14d27202255a499b413dbae63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345505"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo 资源类型

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
| getUrl         | string | 适合使用 HTTP GET (iframe 等) 进行嵌入的 URL
| postUrl        | string | 适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL
| postParameters | string | 如果使用 postUrl, 则发布要包括的参数

根据指定选项的当前支持状态, 可能会返回 getUrl、postUrl 或 both。

postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 postUrl 执行 POST, 应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

url 和参数的格式应被认为是不透明的。
