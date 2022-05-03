---
author: kevinlam
description: ItemPreviewInfo 资源包含有关如何嵌入 DriveItem 预览版的信息。
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 49c792845205b8b42b70961185da4ca46bee2fb7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176974"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemPreviewInfo** 资源包含有关如何嵌入 [DriveItem](driveitem.md) 预览版的信息。

## <a name="json-representation"></a>JSON 表示形式

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>属性

| 属性       | 类型   | Description                                                      |
| :------------- | :----- | :--------------------------------------------------------------- |
| getUrl         | string | 适用于使用 HTTP GET (iframe 等嵌入的 URL，)         |
| postUrl        | string | 适用于使用 HTTP POST (表单文章、JS 等嵌入的 URL )  |
| postParameters | string | 使用 postUrl 时要包含的 POST 参数                      |

getUrl、postUrl 或两者都可以返回，具体取决于指定选项的当前支持状态。

postParameters 是格式化为 `application/x-www-form-urlencoded`的字符串，如果对 postUrl 执行 POST，则应相应地设置内容类型。 例如：

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

URL 和参数的格式应被视为不透明。
