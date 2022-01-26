---
title: 聊天的列表权限权限
description: 检索聊天的权限权限。
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56e3d816dd8736d4ef34a602de22b6295df45ecf
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225880"
---
# <a name="list-permissiongrants-of-a-chat"></a>聊天的列表权限权限

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 [聊天](../resources/chat.md) 的所有 [特定于资源的权限授予](../resources/resourcespecificpermissiongrant.md)。此列表指定有权访问 **聊天** 的 Azure AD 应用，以及每个应用具有的相应类型的特定于资源的访问权限。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                                                                                                                        |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | ResourceSificPermissionGrant.ReadFor你、TeamsAppInstallation.ReadFor如果一、TeamsAppInstallation.ReadWriteSelfForChat、TeamsAppInstallation.ReadWriteFor一并                                    |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                                                                                                                                     |
| 应用程序                            | TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, ResourceSpecificPermissionGrant.ReadForChat.All, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/permissionGrants
```

## <a name="optional-query-parameters"></a>可选的查询参数

此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。

## <a name="request-headers"></a>请求标头

| 标头           | 值                      |
| :--------------- | :------------------------- |
| Authorization    | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_list_permission_grants"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-list-permission-grants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-list-permission-grants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-list-permission-grants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-list-permission-grants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-list-permission-grants-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chat-list-permission-grants-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>响应

以下示例显示了相应的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#permissionGrants",
   "value":[
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNDaGF0U2V0dGluZ3MuUmVhZFdyaXRlLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"ChatSettings.ReadWrite.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc0FwcEluc3RhbGxhdGlvbi5SZWFkLkNoYXQjI0FwcGxpY2F0aW9u",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsAppInstallation.Read.Chat"
      },
      {
         "id":"Y2VkZGEyMWUtYTUwZS00ZDI3LWEyZjAtOTk0MTMwMGY3Y2I1IyNUZWFtc1RhYi5EZWxldGUuQ2hhdCMjQXBwbGljYXRpb24=",
         "clientAppId":"fdebf36e-8b3a-4b00-99fb-2e4d1da706d6",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"771b9da9-2260-41eb-a587-4d936e4aa08c",
         "permissionType":"Application",
         "permission":"TeamsTab.Delete.Chat"
      },
      {
         "id":"ZmNmMGMzNjQtMWY1ZS00MDVjLThiN2QtNjI2YmRmOWQyZjI1IyNDaGF0U2V0dGluZ3MuUmVhZC5DaGF0IyNBcHBsaWNhdGlvbg==",
         "clientAppId":"69024002-35ae-4574-a219-f261183580b4",
         "resourceAppId":"00000003-0000-0000-c000-000000000000",
         "clientId":"74c92190-dc0e-485a-81c6-fdffd4aadfd8",
         "permissionType":"Application",
         "permission":"ChatSettings.Read.Chat"
      }
   ]
}
```

## <a name="see-also"></a>另请参阅
- [列出团队的权限授予](team-list-permissionGrants.md)
- [组的列表权限管理](group-list-permissionGrants.md)
