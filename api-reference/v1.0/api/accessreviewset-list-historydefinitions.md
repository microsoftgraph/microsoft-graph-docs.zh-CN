---
title: 列出 historyDefinitions
description: 获取 accessReviewHistoryDefinition 对象的列表。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9e2f44c8484b65e2980a70cb6041826656b8a078
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444088"
---
# <a name="list-historydefinitions"></a>列出 historyDefinitions

命名空间：microsoft.graph

检索过去 30 天内创建的 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象，包括所有嵌套属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.ReadWrite.All|

如果已登录用户不是全局管理员目录角色成员或全局读取者目录角色成员，则只会返回已登录用户创建的定义。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$top``$filter``$expand`OData 查询参数，`$skip`以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。 包括 `?$expand=instances` 将返回 [accessReviewHistoryDefinitions](../resources/accessreviewhistorydefinition.md) 对象及其关联的实例。

此 API 的默认页面大小为 100 **个 accessReviewHistoryDefinitions** 对象。 若要提高效率并避免因大型结果集而超时，请使用 `$skip` 分页和 `$top` 查询参数。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistorydefinition"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewhistorydefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "isCollection": "true"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
            "id": "67e3de15-d263-45a9-8f4f-71271b495db7",
            "displayName": "Last year's ELM assignment reviews - one time",
            "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
            "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
            "decisions": [
                "approve",
                "deny",
                "dontKnow",
                "notReviewed",
                "notNotified"
            ],
            "status": "done",
            "createdDateTime": "2021-04-14T00:22:48.9392594Z",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scopes": [
                {
                    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                    "queryType": "MicrosoftGraph",
                    "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
                    "queryRoot": null
                }
            ]
        }
    ]
}
```
