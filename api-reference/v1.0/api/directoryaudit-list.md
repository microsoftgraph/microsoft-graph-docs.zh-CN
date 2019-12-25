---
title: 列出 directoryAudits
description: 介绍了 Microsoft Graph API 中的 directoryAudit 资源（实体）的列表方法。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7733cd1a29640331ecd4ab766bc3563fa29600b7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869956"
---
# <a name="list-directoryaudits"></a>列出 directoryAudits

获取 Azure Active Directory 生成的审核日志的列表。 这包括由 Azure AD 中的各种服务生成的审核日志，包括用户、应用、设备和组管理、特权标识管理（PIM）、访问查看、使用条款、身份保护、密码管理（自助服务和管理员）密码重置）和自助服务组管理等。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | AuditLog 和所有目录。全部读取. 所有    |
| 委派（个人 Microsoft 帐户） | 不支持                               |
| 应用                            | AuditLog.Read.All                           |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryaudits
```

## <a name="optional-query-parameters"></a>可选查询参数

此方法支持以下 OData 查询参数来帮助自定义响应。 关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query_parameters)。

| 名称                                                       | 说明                                                                   | 示例                                                                     |
| :--------------------------------------------------------- | :---------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [\$筛选器](/graph/query_parameters#filter-parameter)       | 筛选结果（行）。                                                       | `/auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`         |
| [\$返回页首](/graph/query_parameters#top-parameter)             | 设置结果的页面大小。                                                | `/auditLogs/directoryAudits?$top=1`                                         |
| [\$skiptoken](/graph/query_parameters#skiptoken-parameter) | 从跨多页的结果集中检索下一页结果。 | `/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a>Filter 参数支持\$的属性

| 属性名                                               | 支持的运算符 |
| :----------------------------------------------------------- | :------------------ |
| activityDisplayName                                          | eq、startswith      |
| activityDateTime                                             | eq、ge、le          |
| loggedByService                                              | eq                  |
| initiatedBy/user/id                                          | eq                  |
| initiatedBy/user/displayName                                 | eq                  |
| initiatedBy/user/userPrincipalName                           | eq、startswith      |
| initiatedBy/app/appId                                        | eq                  |
| initiatedBy/app/appDisplayName                               | eq                  |
| targetResources/any （t： t/id eq "{value}"）                    | eq                  |
| targetResources/any （t： t/displayName eq ' {value} '）            | eq                  |
| targetResources/any （x： startswith （x/displayName，"{value}"）） | startswith          |

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[directoryAudit](../resources/directoryaudit.md)对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditlogs/directoryaudits",
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "728309ae-1a37-4937-9afe-e35d964db09b",
                "displayName": "Audry Oliver",
                "userPrincipalName": "bob@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"}],
            "groupType": "unifiedGroups"
            }, 
            {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "bob@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
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
