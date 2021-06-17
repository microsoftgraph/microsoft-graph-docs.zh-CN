---
author: JeremyKelley
description: 可以使用 createLink 操作通过共享链接共享 DriveItem。
title: driveItem： createLink
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b471e95a07a0f7ec8c375d098b3875b8951e893e
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971084"
---
# <a name="driveitem-createlink"></a>driveItem： createLink

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以使用 **createLink** 操作通过共享链接共享 [driveItem。](../resources/driveitem.md)

如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。

DriveItem 资源从其上级继承共享权限。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

请求正文定义应用程序正在请求的共享链接的属性。
请求应为具有以下属性的 JSON 对象。

|   属性                 |  类型  |                                 说明                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|type|字符串|可选。要创建的共享链接的类型。   |
|scope|String|可选。 要创建的链接的范围。 匿名、组织或用户。|
|expirationDateTime|DateTimeOffset|可选。 DateTime 格式为 yyyy-MM-ddTHH：mm：ssZ 的 String 表示权限的过期时间。|
|密码|String|可选。创建者设置的共享链接的密码。|
|recipients|[driveRecipient](../resources/driverecipient.md) 集合|可选。 将接收共享链接访问权限的收件人的集合。|

### <a name="link-types"></a>链接类型

**type** 参数允许使用以下值：

| 类型值 | 说明                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| view           | 创建到 **driveItem** 的只读链接。                                                                        |
| review         | 创建 **driveItem 的审阅链接**。 此选项仅适用于 OneDrive for Business 和 SharePoint。                   |
| edit           | 创建到 **driveItem** 的读写链接。                                                                       |
| 嵌入          | 创建 **driveItem** 的可嵌入链接。                                                                      |
| blocksDownload | 创建阻止下载到 **driveItem** 的只读链接。 此选项仅适用于 OneDrive for Business 和 SharePoint。  |
| createOnly     | 创建 **driveItem** 的仅上载链接。 此选项仅适用于 OneDrive for Business 和 SharePoint 中的文件夹。             |
| addressBar     | 为新建的文件创建浏览器地址栏中显示的默认链接。 仅适用于 OneDrive for Business 和 SharePoint。 组织管理员配置此链接类型是否受支持，以及此链接类型支持哪些功能。 |
| adminDefault   | 创建到 **driveItem** 的默认链接，该链接由组织的管理员确定。 仅适用于 OneDrive for Business 和 SharePoint。 该策略由管理员为组织强制执行 |

### <a name="scope-types"></a>范围类型

**scope** 参数允许使用以下值。

| 值          | 说明
|:---------------|:------------------------------------------------------------
| anonymous    | 拥有该链接的任何人都可以访问，无需登录。 这可能包括组织外部的人员。 管理员可能会禁用匿名链接支持。
| 组织 | 登录到组织（租户）的任何人都可以使用该链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。
| users        | 收件人集合中的特定人员可以使用链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享权限。

如果为 `201 Created` **driveItem** 创建了新的共享链接，或者返回了现有链接， `200 OK` 则响应将为 。

## <a name="examples"></a>示例

### <a name="example-1-create-an-anonymous-sharing-link"></a>示例 1：创建匿名共享链接
以下示例请求为用户的 OneDrive 中的 {itemId} 指定的 **driveItem** 创建共享OneDrive。
共享链接配置为只读并且可由具有该链接的任何用户使用。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
  "hasPassword": true
}
```

### <a name="example-2-creating-company-sharable-links"></a>示例 2：创建公司可共享链接

OneDrive for Business 和 SharePoint 都支持公司可共享的链接。
此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。
若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

### <a name="example-3-creating-embeddable-links"></a>示例 3：创建可嵌入链接

使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。

>**注意：** 仅 OneDrive 个人版支持嵌入链接。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>注解

* 若要根据组织的默认策略和呼叫者对 **driveItem** 的权限创建链接，请省略 scope 和 type 参数
* 使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。
* 链接在 **driveItem** 的共享权限中可见，并且可以通过 **driveItem** 的所有者删除。
* 链接始终指向 **driveItem** 的当前版本，除非仅将 **driveItem** (SharePoint签出) 。

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for a driveItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->