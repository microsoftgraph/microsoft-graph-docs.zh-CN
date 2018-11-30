---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010064"
---
# <a name="itempreviewinfo-resource-type"></a>itemPreviewInfo 资源类型

**ItemPreviewInfo**资源包含有关如何将嵌入的[driveItem](driveitem.md)预览信息。

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
| getUrl         | string | 适用于嵌入使用 HTTP GET （iframe 等） 的 URL
| postUrl        | string | 适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）
| postParameters | string | 如果使用 postUrl 包括 POST 参数

GetUrl、 postUrl，或同时可能会返回根据支持指定的选项的当前状态。

postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

不透明应考虑的 Url 和参数的格式。
