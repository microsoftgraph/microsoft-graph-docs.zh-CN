---
title: 'driveItem: preview'
description: 此操作允许您获取项目的短生存期可嵌入 url, 以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572701"
---
# <a name="driveitem-preview"></a>driveItem: preview

此操作允许您获取项目的短生存期可嵌入 url, 以呈现临时预览。

如果要获取持续生存期的可嵌入链接, 请改用[createLink][] API。

> **注意:****预览**操作当前仅适用于 SharePoint 和 OneDrive for business。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | 文件. 读取、文件读写、全部、读写全部。
| 委派（个人 Microsoft 帐户） | Read, 文件. readwrite, 全部文件。
| 应用程序                            | 不支持。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>请求正文

请求正文定义您的应用程序所请求的可嵌入 URL 的属性。
请求应为具有以下属性的 JSON 对象。

|   名称      |  类型         | 说明
|:------------|:--------------|:-----------------------------------------------
| page        | string/number | 可选。 要从其开始的文档的页码 (如果适用)。 为在文件类型 (如 ZIP) 周围的将来用例指定为字符串。
| zoom        | number        | 可选。 要从其开始的缩放级别 (如果适用)。

## <a name="response"></a>响应

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

响应将是一个包含以下属性的 JSON 对象:

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适合使用 HTTP GET (iframe 等) 进行嵌入的 URL
| postUrl        | string | 适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL
| postParameters | string | 如果使用 postUrl, 则发布要包括的参数

根据指定选项的 embed 支持的当前状态, 可能会返回 getUrl、postUrl 或 both。

postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 postUrl 执行 POST, 应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>页面/缩放

"页面" 和 "缩放" 选项可能不适用于所有预览版应用程序, 但如果预览应用支持它, 则会应用。
