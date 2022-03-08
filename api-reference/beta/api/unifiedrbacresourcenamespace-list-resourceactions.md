---
title: 列出 resourceActions
description: 获取 unifiedRbacResourceAction 对象及其属性的列表。
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 31e1893bbd57d8971fbe7b4f29001d204c164151
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338233"
---
# <a name="list-resourceactions"></a>列出 resourceActions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [unifiedRbacResourceAction 对象](../resources/unifiedrbacresourceaction.md) 及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/resourceNamespaces/{unifiedRbacResourceNamespaceId}/resourceActions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 、 `$filter`、 `$select`和 `$top``$skipToken` OData 查询参数来帮助自定义响应。 此方法支持 (`$filter`) `eq` **、说明**、**id** 和 **名称属性的自定义** 属性。  此方法返回 100 **resourceActions** 的默认页面大小，并支持 `$top` 和 `$skipToken` 分页。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-microsoftdirectory-actions"></a>示例 1：获取 microsoft.directory 操作

以下示例获取标识符为 的资源命名空间的操作 `microsoft.directory`。

此方法最多返回 100 个操作。 如果更多操作，可以使用 获取 `@odata.nextLink` 下一组操作。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrbacresourceaction_directory"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrbacresourceaction-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrbacresourceaction-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrbacresourceaction-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrbacresourceaction-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrbacresourceaction-directory-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrbacresourceaction-directory-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了可读性，此处显示的答复对象已缩短。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRbacResourceAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/resourceNamespaces('microsoft.directory')/resourceActions",
    "@odata.nextLink": "https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions?$skiptoken=bWljcm9z...",
    "value": [
        {
            "actionVerb": null,
            "description": "Create and delete access reviews, and read and update all properties of access reviews in Azure AD",
            "id": "microsoft.directory-accessReviews-allProperties-allTasks",
            "name": "microsoft.directory/accessReviews/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": "GET",
            "description": "Read all properties of access reviews",
            "id": "microsoft.directory-accessReviews-allProperties-read-get",
            "name": "microsoft.directory/accessReviews/allProperties/read",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Manage access reviews of application role assignments in Azure AD",
            "id": "microsoft.directory-accessReviews-definitions.applications-allProperties-allTasks",
            "name": "microsoft.directory/accessReviews/definitions.applications/allProperties/allTasks",
            "resourceScopeId": null
        }
    ]
}
```

### <a name="example-2-get-microsoftinsights-actions"></a>示例 2：获取 microsoft.insights 操作

以下示例获取标识符为 的资源命名空间的操作 `microsoft.insights`。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrbacresourceaction_insights"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.insights/resourceActions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrbacresourceaction-insights-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrbacresourceaction-insights-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrbacresourceaction-insights-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrbacresourceaction-insights-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrbacresourceaction-insights-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrbacresourceaction-insights-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRbacResourceAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/resourceNamespaces('microsoft.insights')/resourceActions",
    "value": [
        {
            "actionVerb": null,
            "description": "Manage all aspects of Insights app",
            "id": "microsoft.insights-allEntities-allProperties-allTasks",
            "name": "microsoft.insights/allEntities/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Read all aspects of Viva Insights",
            "id": "microsoft.insights-allEntities-allProperties-read",
            "name": "microsoft.insights/allEntities/allProperties/read",
            "resourceScopeId": null
        },
        {
            "actionVerb": "PATCH",
            "description": "Deploy and manage programs in Insights app",
            "id": "microsoft.insights-programs-allProperties-update-patch",
            "name": "microsoft.insights/programs/allProperties/update",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Run and manage queries in Viva Insights",
            "id": "microsoft.insights-queries-allProperties-allTasks",
            "name": "microsoft.insights/queries/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": "GET",
            "description": "View reports and dashboard in Insights app",
            "id": "microsoft.insights-reports-allProperties-read-get",
            "name": "microsoft.insights/reports/allProperties/read",
            "resourceScopeId": null
        }
    ]
}
```
