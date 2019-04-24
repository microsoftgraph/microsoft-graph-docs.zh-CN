---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585235"
---
# <a name="itempreviewinfo-resource-type"></a>itemPreviewInfo 资源类型

**itemPreviewInfo**资源包含有关如何嵌入[driveItem](driveitem.md)的预览的信息。

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
| getUrl         | 字符串 | 适合使用 HTTP GET (iframe 等) 进行嵌入的 URL
| postUrl        | 字符串 | 适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL
| postParameters | 字符串 | 如果使用 postUrl, 则发布要包括的参数

根据指定选项的当前支持状态, 可能会返回 getUrl、postUrl 或 both。

postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 postUrl 执行 POST, 应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

url 和参数的格式应被认为是不透明的。
