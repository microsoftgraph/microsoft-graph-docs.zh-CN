---
title: 列出 teamsApp
description: '列出 Microsoft 团队应用程序目录中的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3c9a01ce67893cdf335f38c7351a4174a251b495
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607545"
---
# <a name="list-teamsapp"></a>列出 teamsApp

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 Microsoft 团队应用程序目录中的 [应用程序](../resources/teamsapp.md) 。
这包括 Microsoft 团队存储中的应用程序，以及组织的应用程序目录 (租户应用程序目录) 中的应用程序。 若要仅从组织的应用程序目录中获取应用程序，请 `organization` 在请求中将 **distributionMethod** 指定为 ""。

> [!NOTE]
> `id` **TeamsApp** 资源的是由服务器生成的，并且与 `id` 团队应用程序清单中指定的资源不同。 `id`作为团队应用程序清单的一部分的开发人员提供的标记为 `externalId` **teamsApp** 资源中的。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:------------------------------------|
| 委派（工作或学校帐户）     | AppCatalog、AppCatalog、所有的、所有读写的。 all |
| 委派（个人 Microsoft 帐户） | 不支持                       |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

使用 `$expand=AppDefinitions` 将返回有关应用的状态的详细信息（如 **publishingState**），它反映应用程序提交的审阅状态，并返回应用程序是否已被批准、被拒绝或仍处于审阅状态。 

> **注意：** 您可以对 [teamsApp](../resources/teamsapp.md) 对象的任何字段进行筛选，以缩短结果列表。 您可以使用以下任何筛选器操作：等于、不等于、和、或，而不是。

## <a name="request-headers"></a>请求标头

| 标头        | 值                     |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsApp](../resources/teamsapp.md) 对象的列表。

## <a name="examples"></a>示例

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a>示例1：列出特定于租户的所有应用程序

下面的示例列出了特定于您的租户的所有应用程序。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```



<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>示例2：列出具有给定 ID 的应用程序

下面的示例列出了具有给定 ID 的应用程序。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_filter_id",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a>示例3：基于团队应用程序清单 ID 查找应用程序。

下面的示例列出与团队应用程序清单中指定的 "id" 匹配的应用程序。 在此示例中，团队应用程序的清单 ID 为 "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee"。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_filter_externalid",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
  }
```

### <a name="example-4-list-applications-with-a-given-id-and-return-the-submission-review-state"></a>示例4：列出具有给定 ID 的应用程序，并返回提交检查状态

下面的示例列出了具有给定 ID 的应用程序，并展开 **appDefinitions** 以返回 **publishingState**，这将反映应用程序的提交审阅状态。 `Submitted` 表示正在等待审阅， `published` 表示该应用程序已由管理员批准，并且该 `rejected` 应用程序被管理员拒绝。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_expand_appdefinitions"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_expand_appdefinitions",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
        {
          "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",
          "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",
          "azureADAppId": null,
          "displayName": "Test App",
          "version": "1.0.1",
          "requiredResourceSpecificApplicationPermissions": [],
          "publishingState": "published"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

- [列出团队中安装的应用程序](team-list-installedapps.md)
- [列出聊天中安装的应用程序](chat-list-installedapps.md)
- [列出在用户的个人范围内安装的应用程序](userteamwork-list-installedapps.md)




