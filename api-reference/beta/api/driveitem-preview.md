---
title: driveItem： 预览
description: 此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be96a0cd451bb3f1c75c32f235d7669ce0bd7509
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980872"
---
# <a name="driveitem-preview"></a>driveItem： 预览

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。

如果您想要获取长生存期嵌入链接，请改用[createLink][] API。

> **注意：****预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）
|:---------------------------------------|:-------------------------------------------
| 委派（工作或学校帐户）     | Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All
| 委派（个人 Microsoft 帐户） | Files.Read，Files.ReadWrite，Files.ReadWrite.All
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

在请求正文定义嵌入请求您的应用程序的 URL 的属性。
请求应为具有以下属性的 JSON 对象。

|   名称      |  类型         | 说明
|:------------|:--------------|:-----------------------------------------------
| 查看器      | string        | 可选。 预览应用程序使用。 `onedrive` 或 `office`）。 如果为空，将自动选择合适的查看器。
| 边框  | boolean       | 可选。 如果`true`（默认），嵌入视图将不包括任何控件。
| allowEdit   | boolean       | 可选。 如果`true`，该文件可以从嵌入 UI 进行编辑。
| page        | 字符串/编号 | 可选。 要启动，如果适用文档的页码。 指定为字符串的文件类型，如 ZIP 周围的将来使用情况。
| zoom        | 数字        | 可选。 如果适用，则缩放级别，从开始。

## <a name="response"></a>响应

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

响应将是一个 JSON 对象，包含以下属性：

| 名称           | 类型   | 说明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | 适用于嵌入使用 HTTP GET （iframe 等） 的 URL
| postUrl        | string | 适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）
| postParameters | string | 如果使用 postUrl 包括 POST 参数

GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。

postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。 例如：
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>查看者

**查看器**参数允许以下值。

| 类型值 | 说明
|:-----------|:----------------------------------------------------------------
| (null)     | 选择相应的应用程序用于呈现该文件。 这将在大多数情况下使用`onedrive`预览器，但可能因文件类型。
| `onedrive` | 使用 OneDrive previewer app 呈现该文件。
| `office`   | WAC (Office online) 用于呈现该文件。 唯一有效的 Office 文档。

### <a name="chrome-vs-chromeless"></a>部件版式 vs 边框

如果`chromeless`是 true，则预览将该文件裸机呈现。
否则，可能有其他工具栏/按钮显示与文档/视图进行交互。

### <a name="viewedit"></a>查看/编辑

如果`allowEdit`是 true，则可以通过嵌入的预览与用户交互修改文档。
此功能可能不可用的全部预览应用程序或文件类型。

### <a name="pagezoom"></a>页/缩放

`page`和`zoom`选项可能不是可用于所有预览应用程序，但如果预览应用程序支持将应用。
