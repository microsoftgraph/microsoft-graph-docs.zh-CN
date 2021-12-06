---
title: '列出 oAuth2PermissionGrants (委派的权限授予) '
description: 检索表示委派权限授予的 oauth2PermissionGrant 对象的列表。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 55e4e2477e2893b06044b099aab30b40fd67004d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032304"
---
# <a name="list-oauth2permissiongrants-delegated-permission-grants"></a>列出 oauth2PermissionGrants (委派的权限授予) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象的列表，这些对象代表已授予客户端应用程序代表登录用户访问 API 的委派权限。

> [!NOTE]
> 此请求对最近创建、更新或删除的委派权限授予可能具有复制延迟。 如果指定了筛选，此延迟 `clientId` 将最小化。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-oauth2permissiongrants-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#oauth2PermissionGrants",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/oauth2PermissionGrants/AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0",
            "clientId": "263a5b01-03e5-408e-8557-bab681df104c",
            "consentType": "AllPrincipals",
            "expiryTime": "2022-01-29T10:32:59.5138373Z",
            "id": "AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0",
            "principalId": null,
            "resourceId": "1804a6f8-e623-4520-8f40-ba1b0c11c42d",
            "scope": "User.Read Group.ReadWrite.All",
            "startTime": "0001-01-01T00:00:00Z"
        },
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/oauth2PermissionGrants/AVs6JuUDjkCFV7q2gd8QTOQDNpSH5-lPk9HjD3Sarjk",
            "clientId": "263a5b01-03e5-408e-8557-bab681df104c",
            "consentType": "AllPrincipals",
            "expiryTime": "2031-08-02T14:05:12.575045Z",
            "id": "AVs6JuUDjkCFV7q2gd8QTOQDNpSH5-lPk9HjD3Sarjk",
            "principalId": null,
            "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
            "scope": "Tasks.ReadWrite Files.ReadWrite.All Files.ReadWrite Contacts.ReadWrite Calendars.ReadWrite Mail.ReadWrite Directory.AccessAsUser.All Directory.ReadWrite.All Group.ReadWrite.All Group.Read.All User.ReadWrite Mail.ReadWrite.Shared Mail.Send.Shared Calendars.ReadWrite.Shared Contacts.ReadWrite.Shared Tasks.ReadWrite.Shared Sites.ReadWrite.All Files.ReadWrite.AppFolder Files.ReadWrite.Selected Notes.ReadWrite Notes.ReadWrite.All MailboxSettings.ReadWrite DeviceManagementManagedDevices.PrivilegedOperations.All DeviceManagementManagedDevices.ReadWrite.All DeviceManagementRBAC.ReadWrite.All DeviceManagementApps.ReadWrite.All DeviceManagementConfiguration.ReadWrite.All openid profile Directory.Read.All User.Read.All User.ReadWrite.All ChannelMember.ReadWrite.All DeviceManagementServiceConfiguration.ReadWrite.All",
            "startTime": "0001-01-01T00:00:00Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


