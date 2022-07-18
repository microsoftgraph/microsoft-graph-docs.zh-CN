---
title: 列出 directoryAudits
description: 介绍 Microsoft 图形 API (beta 版本) ) 的 directoryAudit 资源 (实体的列表方法。
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: dd8fe4c8923dac46cd9e9d7854d64015a5319390
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437402"
---
# <a name="list-directoryaudits"></a>列出 directoryAudits

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 Azure Active Directory 生成的审核日志列表。 这包括 Azure AD 中各种服务生成的审核日志，包括用户、应用、设备和组管理、特权标识管理 (PIM) 、访问评审、使用条款、标识保护、密码管理 (SSPR 和管理员密码重置) ，以及自助服务组管理。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AuditLog.Read.All 和 Directory.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | AuditLog.Read.All 和 Directory.Read.All | 

> [!IMPORTANT]
> 此 API 存在 [已知问题](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) ，当前需要同意 **AuditLog.Read.All** 和 **Directory.Read.All** 权限。

此外，应用还必须向 Azure AD [正确注册](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 OData 查询参数，以帮助自定义响应。 有关如何使用此参数的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

|参数     |说明                            |示例|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|筛选结果（行）。 |`/auditLogs/directoryAudits?$filter=activityDateTime le 2018-01-24`<br>`/auditLogs/directoryAudits?$filter=targetResources/any(x: startswith(x/displayName, 'def'))` |
|[$top](/graph/query-parameters#top-parameter)|设置结果的页面大小。|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|从跨多页的结果集中检索下一页结果。|`/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a>$filter参数支持的属性

|属性        |支持的运算符|
|:----------------|:------|
|activityDisplayName| eq、startswith|
|activityDateTime| eq、ge、le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq、startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/displayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq、startswith|

## <a name="request-headers"></a>请求头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryAudit](../resources/directoryaudit.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryaudits-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryaudits-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
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
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
