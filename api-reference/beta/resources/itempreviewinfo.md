---
author: kevinlam
description: ItemPreviewInfo 资源包含有关如何嵌入 DriveItem 预览的信息。
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9e4f3b390fe21284791b6c40d19d4de71ec3548b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723344"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemPreviewInfo** 资源包含有关如何嵌入 [DriveItem 预览的信息](driveitem.md)。

## <a name="json-representation"></a>JSON 表示形式

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>属性

| 属性       | 类型   | 说明                                                      |
| :------------- | :----- | :--------------------------------------------------------------- |
| getUrl         | string | 适合使用 HTTP GET (iframe 等嵌入的 URL )         |
| postUrl        | string | 适合使用 HTTP POST 和表单帖子 (JS 等进行嵌入的 URL )  |
| postParameters | string | 使用 postUrl 时要包含的 POST 参数                      |

可能会返回 getUrl、postUrl 或两者，具体取决于指定选项的当前支持状态。

postParameters 是 `application/x-www-form-urlencoded`格式设置为 的字符串，如果对 postUrl 执行 POST，应相应地设置内容类型。 例如：

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

URL 和参数的格式应视为不透明。
