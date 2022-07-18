---
title: 获取 directoryAudit
description: 介绍 Microsoft 图形 API (beta 版本) ) 的 directoryAudit 资源 (实体的 get 方法。
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bc17537c2eafaf53855c65291296c03670d4842a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445708"
---
# <a name="get-directoryaudit"></a>获取 directoryAudit

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取特定的 Azure Active Directory 审核日志项。 这包括 Azure Active Directory 中各种服务生成的审核日志项，例如用户、应用程序、设备和组管理、特权标识管理 (PIM) 、访问评审、使用条款、标识保护、密码管理 (自助服务和管理员密码重置) 、自助服务组管理等。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AuditLog.Read.All 和 Directory.Read.All |
|委派（个人 Microsoft 帐户） | 不支持   |
|Application | AuditLog.Read.All 和 Directory.Read.All | 

> [!IMPORTANT]
> 此 API 存在 [已知问题](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) ，当前需要同意 **AuditLog.Read.All** 和 **Directory.Read.All** 权限。

此外，应用还必须向 Azure AD [正确注册](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。 有关如何使用此参数的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryAudit](../resources/directoryaudit.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudit-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryaudit-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Directory_504a302a-8f2d-418d-b7df-bf77de6ed831_M1N6X_27777783",
    "category": "UserManagement",
    "correlationId": "504a302a-8f2d-418d-b7df-bf77de6ed831",
    "result": "success",
    "resultReason": "",
    "activityDisplayName": "Update user",
    "activityDateTime": "2022-06-21T23:25:00.1458248Z",
    "loggedByService": "Core Directory",
    "operationType": "Update",
    "userAgent": null,
    "initiatedBy": {
        "app": null,
        "user": {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test Admin",
            "userPrincipalName": "tadmin@contoso.com",
            "ipAddress": "",
            "userType": "Member",
            "homeTenantId": null,
            "homeTenantName": null
        }
    },
    "targetResources": [
        {
            "id": "2c940657-1026-4386-bcfd-3176637ba01f",
            "displayName": "Test User",
            "type": "User",
            "userPrincipalName": "tuser@contoso.com",
            "groupType": null,
            "modifiedProperties": [
                {
                    "displayName": "StrongAuthenticationMethod",
                    "oldValue": "[{\"MethodType\":6,\"Default\":true},{\"MethodType\":7,\"Default\":false}]",
                    "newValue": "[{\"MethodType\":7,\"Default\":false},{\"MethodType\":6,\"Default\":true},{\"MethodType\":0,\"Default\":false},{\"MethodType\":5,\"Default\":false}]"
                },
                {
                    "displayName": "Included Updated Properties",
                    "oldValue": null,
                    "newValue": "\"StrongAuthenticationMethod\""
                },
                {
                    "displayName": "TargetId.UserType",
                    "oldValue": null,
                    "newValue": "\"Member\""
                }
            ]
        }
    ],
    "additionalDetails": [
        {
            "key": "UserType",
            "value": "Member"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
