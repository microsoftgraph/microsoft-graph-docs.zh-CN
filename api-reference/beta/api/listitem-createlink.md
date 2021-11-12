---
title: listItem： createLink
description: 创建链接以共享 listItem
author: learafa
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e12ceccbf8ea29893d185ba8564e831bbe850b5c
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60941342"
---
# <a name="listitem-createlink"></a>listItem： createLink

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 [listItem 创建共享链接](../resources/listitem.md)。

如果调用应用程序不存在指定的链接类型 **，createLink** 操作将创建新的共享链接。
如果应用已存在指定类型的共享链接，此操作将返回现有共享链接。

**listItem** 资源从项目所在的 [列表中](../resources/list.md) 继承共享权限。

## <a name="permissions"></a>权限
若要调用此 API，需要以下权限之一。 若要了解更多信息，包括如何选择权限，请参阅 [权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|   属性             |  类型  |           Description                        |
| :----------------------| :----- | :--------------------------------------------|
|type|String|要创建的共享链接的类型。 可选。 |
|scope|String|要创建的链接的范围。 、 `anonymous` `organization` 或 `users` 。 可选。 |
|expirationDateTime|DateTimeOffset|DateTime 格式为 yyyy-MM-ddTHH：mm：ssZ 的字符串指示权限的过期时间。 可选。 |
|密码|String|创建者设置的共享链接的密码。 可选。 |
|recipients|[driveRecipient](../resources/driverecipient.md) 集合|将接收共享链接访问权限的收件人的集合。 可选。 |

### <a name="link-types"></a>链接类型

**type** 参数允许使用以下值：

| 类型值 | 说明                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| view           | 创建到项目的只读链接。                                                                        |
| review         | 创建指向该项目的审阅链接。 此选项仅适用于 OneDrive for Business 和 SharePoint。                   |
| edit           | 创建指向该项目的读写链接。                                                                       |
| 嵌入          | 创建到项目的可嵌入链接。                                                                      |
| blocksDownload | 创建阻止下载到项目的只读链接。 此选项仅适用于 OneDrive for Business 和 SharePoint。  |
| createOnly     | 创建项的仅上载链接。 此选项仅适用于 OneDrive for Business 和 SharePoint 中的文件夹。             |
| addressBar     | 为新建的文件创建浏览器地址栏中显示的默认链接。 仅适用于 OneDrive for Business 和 SharePoint。 组织管理员配置此链接类型是否受支持，以及此链接类型支持哪些功能。 |
| adminDefault   | 创建指向项目的默认链接，该链接由组织的管理员确定。 仅适用于 OneDrive for Business 和 SharePoint。 该策略由管理员为组织强制执行 |

### <a name="scope-types"></a>范围类型

**scope** 参数允许使用以下值。

| 值          | Description
|:---------------|:------------------------------------------------------------
| anonymous    | 拥有该链接的任何人都可以访问，无需登录。 这可能包括组织外部的人员。 管理员可能会禁用匿名链接支持。
| 组织 | 登录到组织（租户）的任何人都可以使用该链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。
| users        | 收件人集合中的特定人员可以使用链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。

## <a name="response"></a>响应

如果成功，此方法在表示请求的[](../resources/permission.md)共享权限的响应正文中返回单个权限资源。

如果为 listItem 创建了新的共享链接，或者 `201 Created` `200 OK` 返回了现有链接，则响应将为 。

## <a name="examples"></a>示例

### <a name="example-1-create-an-anonymous-sharing-link"></a>示例 1：创建匿名共享链接
以下示例请求为 {itemId} 在指定的 {listId} 列表中指定的 listItem 创建共享链接。
共享链接配置为只读并且可由具有该链接的任何用户使用。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

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
[!INCLUDE [sample-code](../includes/snippets/csharp/listitem-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/listitem-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/listitem-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/listitem-createlink-java-snippets.md)]
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
``` http
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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/listitem-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/listitem-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/listitem-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/listitem-createlink-java-snippets.md)]
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
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

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

* 若要基于组织的默认策略和呼叫者对 listItem 的权限创建链接，请省略 scope 和 type 参数
* 使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。
* 链接在 listItem 的共享权限中可见，并且可以通过 listItem 的所有者删除。
* 链接始终指向 listItem 的当前版本，除非 listItem 已签出 (SharePoint列表) 。

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
