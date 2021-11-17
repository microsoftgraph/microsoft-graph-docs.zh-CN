---
title: 列出 teamsApp
description: '列出应用程序目录中Microsoft Teams应用程序。 '
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d4a4115bec5803b4cd0b34437cff6f49774bb45c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991062"
---
# <a name="list-teamsapp"></a>列出 teamsApp

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出[应用程序](../resources/teamsapp.md)目录中Microsoft Teams应用程序。
这包括来自租户Microsoft Teams的应用程序，以及租户应用程序目录 (组织的应用程序目录中) 。 若要仅从组织的应用程序目录中获取应用程序，请 `organization` 指定为请求中的 **distributionMethod。**

> [!NOTE]
> teamsApp 资源的 由服务器生成，与 Teams `id`  `id` 清单中指定的 不同。 开发人员 `id` 作为应用清单的一Teams提供的 标记在 `externalId` **teamsApp** 资源中。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:------------------------------------|
| 委派（工作或学校帐户）     | AppCatalog.Submit、AppCatalog.Read.All、AppCatalog.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

> **注意**：标记为 ** 的权限已弃用，不应使用。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

Using 将返回有关应用状态（如 publishingState）的更多信息，这些状态反映应用提交评价状态，并返回应用是否已获得批准、被拒绝或仍在审核 `$expand=AppDefinitions` 中。  

> **注意：** 可以筛选 [teamsApp](../resources/teamsapp.md) 对象的任何字段以缩短结果列表。 可以使用下列任一筛选操作：等于、不等于、和、或、不。

## <a name="request-headers"></a>请求头

| 标头        | 值                     |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamsApp](../resources/teamsapp.md) 对象列表。

## <a name="examples"></a>示例

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a>示例 1：列出特定于租户的所有应用程序

以下示例列出了特定于租户的所有应用程序。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapps-filter-distributionmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapps-filter-distributionmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapps-filter-distributionmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapps-filter-distributionmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapps-filter-distributionmethod-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




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

### <a name="example-2-list-applications-with-a-given-id"></a>示例 2：列出具有给定 ID 的应用程序

以下示例列出具有给定 ID 的应用程序。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-filter-id-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a>示例 3：根据应用程序清单 ID Teams应用程序

以下示例列出了与在应用程序清单中指定的"id"Teams匹配的应用程序。 在此示例中，Teams 应用的清单 ID 为“cf1ba4c7-f94e-4d80-ba90-5594b641a8ee”。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-filter-externalid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

### <a name="example-4-list-applications-with-a-given-id-and-return-the-submission-review-state"></a>示例 4：列出具有给定 ID 的应用程序，并返回提交审阅状态

以下示例列出具有给定 ID 的应用程序，并展开 **appDefinitions** 以返回 **publishingState，** 反映应用的提交审阅状态。 `Submitted` 表示评价挂起，表示应用已由管理员批准，并且表示应用 `published` `rejected` 已遭管理员拒绝。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_with_filter_expand_appdefinitions"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-with-filter-expand-appdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-with-filter-expand-appdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-with-filter-expand-appdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-with-filter-expand-appdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-with-filter-expand-appdefinitions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_with_filter_expand_appdefinitions",
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

### <a name="example-5-list-the-details-of-only-those-apps-in-the-catalog-that-contain-a-bot"></a>示例 5：仅列出目录中包含自动程序的应用的详细信息

以下示例仅列出目录中包含自动程序的应用。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_with_bots"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$expand=appDefinitions($expand=bot)&$filter=appDefinitions/any(a:a/bot ne null)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-with-bots-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-with-bots-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-with-bots-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-with-bots-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-with-bots-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_with_bots",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps(appDefinitions(bot()))",
    "value": [
        {
            "id": "8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6",
            "externalId": "3CAB7543-216D-47C6-986C-6247670F4663",
            "displayName": "Ducks-3",
            "distributionMethod": "organization",
            "appDefinitions@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6')/appDefinitions(bot())",
            "appDefinitions": [
                {
                    "@odata.etag": "ImNOTW1CR2V1VzgwczlEblVidU00UHc9PSI=",
                    "id": "OGExZWQ3YTMtNWM3OC00NmIyLTg1MDQtZjlkYTAwYTFkMWE2IyMxLjAuOSMjUmVqZWN0ZWQ=",
                    "teamsAppId": "8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6",
                    "azureADAppId": null,
                    "displayName": "Ducks-3",
                    "version": "1.0.9",
                    "requiredResourceSpecificApplicationPermissions": [],
                    "publishingState": "rejected",
                    "shortdescription": "quaerat quasi magnam. slight change. 5",
                    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
                    "lastModifiedDateTime": "2020-11-23T21:36:00.9437445Z",
                    "createdBy": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "70292a90-d2a7-432c-857e-55db6d8f5cd0",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    },
                    "bot@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6')/appDefinitions('OGExZWQ3YTMtNWM3OC00NmIyLTg1MDQtZjlkYTAwYTFkMWE2IyMxLjAuOSMjUmVqZWN0ZWQ%3D')/bot/$entity",
                    "bot": {
                        "id": "bb9f67a4-893b-48d7-ab17-40ed466c0f16"
                    }
                }
            ]
        },
        {
            "id": "30909dee-f7dd-4f89-8b3b-55de2e32489c",
            "externalId": "0ebd3f4d-ca91-495b-a227-a17d298e22cc",
            "displayName": "Self-Install-App-E2E-Tests",
            "distributionMethod": "organization",
            "appDefinitions@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('30909dee-f7dd-4f89-8b3b-55de2e32489c')/appDefinitions(bot())",
            "appDefinitions": [
                {
                    "@odata.etag": "IkwzVDlMOTBSSEdTMFducHUyYkpjVmc9PSI=",
                    "id": "MzA5MDlkZWUtZjdkZC00Zjg5LThiM2ItNTVkZTJlMzI0ODljIyM2LjAuMCMjU3VibWl0dGVk",
                    "teamsAppId": "30909dee-f7dd-4f89-8b3b-55de2e32489c",
                    "azureADAppId": "d75abc57-8255-4309-9c29-a3c689e20341",
                    "displayName": "Self-Install-App-E2E-Tests",
                    "version": "6.0.0",
                    "requiredResourceSpecificApplicationPermissions": [],
                    "publishingState": "submitted",
                    "shortdescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                    "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                    "lastModifiedDateTime": "2020-08-25T18:40:13.035341Z",
                    "createdBy": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "c071a180-a220-43a1-adaf-e8db95c4a7d6",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    },
                    "bot@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('30909dee-f7dd-4f89-8b3b-55de2e32489c')/appDefinitions('MzA5MDlkZWUtZjdkZC00Zjg5LThiM2ItNTVkZTJlMzI0ODljIyM2LjAuMCMjU3VibWl0dGVk')/bot/$entity",
                    "bot": {
                        "id": "da7d471b-de7d-4152-8556-1cdf7a564f6c"
                    }
                }
            ]
        }
    ]
}
```

### <a name="example-6-list-the-details-of-apps-filtered-by-app-installation-scope"></a>示例 6：列出按应用安装范围筛选的应用的详细信息

以下示例仅列出可在用户个人范围内安装的应用。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_in_personal_scope"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$expand=appDefinitions($select=id,displayName,allowedInstallationScopes)&$filter=appDefinitions/any(a:a/allowedInstallationScopes has 'personal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-in-personal-scope-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-in-personal-scope-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-in-personal-scope-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-in-personal-scope-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-in-personal-scope-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_in_personal_scope",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps(appDefinitions(id,displayName,allowedInstallationScopes))",
    "value": [
        {
            "id": "5a542e1c-5f8c-4793-8b0c-6082464b2378",
            "externalId": "4b3ec336-b998-4623-9e25-d4182fb82159",
            "displayName": "Carriage",
            "distributionMethod": "organization",
            "appDefinitions@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a542e1c-5f8c-4793-8b0c-6082464b2378')/appDefinitions(id,displayName,allowedInstallationScopes)",
            "appDefinitions": [
                {
                    "id": "MWE1NDJlMWMtNWY4Yy00NzkzLThiMGMtNjA4MjQ2NGIyMzc4IyMxLjAuMCMjUHVibGlzaGVk",
                    "displayName": "Carriage",
                    "allowedInstallationScopes": "personal"
                }
            ]
        }
    ]
}
```


## <a name="see-also"></a>另请参阅

- [列出在团队中安装的应用](team-list-installedapps.md)
- [列出聊天中安装的应用](chat-list-installedapps.md)
- [列出在用户的个人范围内安装的应用](userteamwork-list-installedapps.md)




