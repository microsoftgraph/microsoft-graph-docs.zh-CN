---
title: List appliesTo
description: 列出分配给应用程序管理策略的资源。
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9bf0ac0198c50a02550a53de18ba544f1752895d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258984"
---
# <a name="list-appliesto"></a>List appliesTo

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出分配了 [appManagementPolicy 策略对象的应用程序](../resources/appManagementPolicy.md) 和服务主体对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                             |
| :------------------------------------- | :--------------------------------------------------------- |
| 委派（工作或学校帐户）     | Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration |
| 委派（个人 Microsoft 帐户） | 不支持。                                             |
| 应用程序                            | Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /policies/appManagementPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 `$select` 、 `$filter` 和 `$top` OData 查询参数来帮助自定义响应。 可以应用于 `$filter` 支持 [的应用程序或](../resources/application.md) [servicePrincipal](../resources/serviceprincipal.md) 对象的属性 `$filter` 。 例如，以下查询检索分配了策略的应用程序或服务主体的 **appId** 和 **displayName。**

``` http

https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo?$select=appId,displayName
```

若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [appManagementPolicy](../resources/appManagementPolicy.md) 对象集合。

## <a name="example-1-get-applications-and-service-principal-objects-applied-to-an-app-management-policy"></a>示例 1：获取应用于应用管理策略的应用程序和服务主体对象

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicyAppliesTo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appmanagementpolicyappliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appmanagementpolicyappliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appmanagementpolicyappliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appmanagementpolicyappliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "0d77e011-2fc6-438f-8b93-decb4f926929",
      "appId": "8f527de6-05c9-4032-bca9-b2b56ab2358a",
      "displayName": "TestApp1",
      "createdDateTime": "2018-01-24T05:55:37Z"
    }
  ]
}
```

## <a name="example-2-get-specific-properties-of-applications-and-service-principal-objects-applied-to-an-app-management-policy-using-select-query-option"></a>示例 2：使用查询选项获取应用程序和服务主体对象的特定属性$select应用管理策略

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicyAppliesTo_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo?$select=id,appId,displayName,createdDateTime
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appmanagementpolicyappliesto-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appmanagementpolicyappliesto-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appmanagementpolicyappliesto-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appmanagementpolicyappliesto-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是返回 应用策略的应用程序和服务主体的 、 和 的响应 `id` `appId` `displayName` `createdDateTime` 示例。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects(id,appId,displayName,createdDateTime)",
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "0d77e011-2fc6-438f-8b93-decb4f926929",
      "appId": "8f527de6-05c9-4032-bca9-b2b56ab2358a",
      "displayName": "TestApp1",
      "createdDateTime": "2018-01-24T05:55:37Z"
    },
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "0e1fa067-dcc1-4d85-9b4c-e69145dd3efb",
      "appId": "255912cb-e31d-4dee-bee4-3fa5d774d6b9",
      "displayName": "TestApp2",
      "createdDateTime": "2018-01-24T05:55:37Z"
    }
  ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "list resources for appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
