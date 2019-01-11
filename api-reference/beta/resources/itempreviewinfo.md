---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857342"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**ItemPreviewInfo**资源包含有关如何将嵌入的[DriveItem](driveitem.md)预览信息。

## <a name="json-representation"></a>JSON 表示形式

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>属性

| 名称           | 类型   | Description
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
