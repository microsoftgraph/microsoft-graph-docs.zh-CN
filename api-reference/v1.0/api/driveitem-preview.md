---
title: driveItem：预览
description: 此操作允许你获取项目的短期嵌入 URL，以便呈现临时预览。
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: fecbdba30948dc89e0344a90574fe932562058fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022763"
---
# <a name="driveitem-preview"></a>driveItem：预览

命名空间：microsoft.graph

此操作允许你获取项目的短期嵌入 URL，以便呈现临时预览。

如果要获取长期嵌入的链接，请改为使用 [createLink][] API。

> **注意：** 预览 **操作** 当前仅适用于 SharePoint 和 OneDrive for Business。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All
| 委派（个人 Microsoft 帐户） | 不支持。
| 应用程序                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All

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

请求正文定义应用程序正在请求的可嵌入 URL 的属性。
请求应为具有以下属性的 JSON 对象。

|   名称      |  类型         | 说明
|:------------|:--------------|:-----------------------------------------------
| page        | string/number | 可选。 要开始的文档的页码（如果适用）。 指定为字符串，用于以后使用诸如 ZIP 等文件类型的情况。
| zoom        | number        | 可选。 缩放级别开始（如果适用）。

## <a name="response"></a>响应

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

该响应将是包含以下属性的 JSON 对象：

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适合使用 HTTP GET (iframe 等嵌入的 URL ) 
| postUrl        | string | 适合使用 HTTP POST 和表单 (JS 等进行嵌入的 URL ) 
| postParameters | string | 使用 postUrl 时要包含的 POST 参数

可能会返回 getUrl、postUrl 或两者，具体取决于指定选项的嵌入支持的当前状态。

postParameters 是格式设置为 的字符串，如果对 postUrl 执行 `application/x-www-form-urlencoded` POST，应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>页面/缩放

"页面"和"缩放"选项可能并非适用于所有预览应用，但将在预览应用支持时应用。

