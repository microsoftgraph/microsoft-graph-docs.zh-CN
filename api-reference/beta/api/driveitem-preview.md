---
title: driveItem： preview
description: 此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: 074bc4c0da2362c6be9958be3ffec8dd4027b690
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808821"
---
# <a name="driveitem-preview"></a>driveItem： preview

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。

如果要获取持续生存期的可嵌入链接，请改用 [createLink][] API。

> **注意：****预览**操作当前仅适用于 SharePoint 和 OneDrive for business。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | 文件. 读取、文件读写、全部、读写全部。
| 委派（个人 Microsoft 帐户） | Read，文件. ReadWrite，全部文件。
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
| 格式      | string        | 可选。 要使用的预览应用。 `onedrive` 或 `office`）。 如果为 null，则将自动选择合适的查看器。
| chromeless  | 布尔       | 可选。 如果 `true` (默认) ，则嵌入的视图将不包含任何控件。
| allowEdit   | 布尔       | 可选。 如果 `true` 是，则可以从嵌入的 UI 编辑该文件。
| page        | string/number | 可选。 要从其开始的文档的页码（如果适用）。 为在文件类型（如 ZIP）周围的将来用例指定为字符串。
| zoom        | number        | 可选。 要从其开始的缩放级别（如果适用）。

## <a name="response"></a>响应

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

响应将是一个包含以下属性的 JSON 对象：

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适用于使用 HTTP GET (iframe 等嵌入的 URL ) 
| postUrl        | string | 适合使用 HTTP POST (表单 post、JS 等进行嵌入的 URL ) 
| postParameters | string | 如果使用 postUrl，则发布要包括的参数

根据指定选项的 embed 支持的当前状态，可能会返回 getUrl、postUrl 或 both。

postParameters 是格式为的字符串 `application/x-www-form-urlencoded` ，如果向 postUrl 执行 POST，应相应地设置内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>查看者

**查看器**参数允许使用以下值。

| 类型值 | 说明
|:-----------|:----------------------------------------------------------------
|  (null)      | 选择用于呈现文件的适当的应用程序。 在大多数情况下，这将使用 `onedrive` 预览器，但可能因文件类型而异。
| `onedrive` | 使用 OneDrive 预览器应用程序呈现文件。
| `office`   | 使用 Office 的 web 版本呈现文件。 仅对 Office 文档有效。

### <a name="chrome-vs-chromeless"></a>Chrome vs chromeless

如果 `chromeless` 为 true，预览将是文件的简略呈现。
否则，可能会显示其他工具栏/按钮以与文档/视图进行交互。

### <a name="viewedit"></a>查看/编辑

如果 `allowEdit` 为 true，则文档可以通过嵌入预览的用户交互进行修改。
此功能可能不适用于所有预览版应用或文件类型。

### <a name="pagezoom"></a>页面/缩放

"" 和 "" `page` `zoom` 选项可能不适用于所有预览版应用，但如果预览应用支持它，则将应用 "" 和 "" 选项。
