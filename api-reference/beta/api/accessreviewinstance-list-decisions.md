---
title: 列出决策
description: 从 decisions 导航属性获取 accessReviewInstanceDecisionItem 资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 138d53b3d0c497601b0bdfe50512ca71ddfd68d9
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161814"
---
# <a name="list-decisions"></a>列出决策
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [特定 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 [AccessReviewInstance](../resources/accessreviewinstance.md)。 返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括所有嵌套属性。

>[!NOTE]
>此 API 的默认页面大小为 100 accessReviewInstance 对象。 若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.Read.All、AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.Read.All、AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` 、 `$filter` `$orderBy` 、 、 `$skip` 和 `$top` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-retrieve-all-decisions-for-an-instance-of-an-access-review"></a>示例 1：检索访问评审实例的所有决策

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "userDisplayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "displayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            }
        },
        {
            "id": "4bde8d40-9224-4aa3-936b-08d73e1baf47",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/11feb738-0039-4a6c-a045-dcb91a47969a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "userDisplayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "displayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            }
        }
    ]
}
```


### <a name="example-2-retrieve-all-decision-items-for-which-youre-a-reviewer-and-expand-the-definitions"></a>示例 2：检索作为审阅者的所有决策项并展开定义

#### <a name="request"></a>请求
以下示例显示一个请求，请求检索调用用户是审阅者的所有实例和定义的所有决策。

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')?$expand=instance($expand=definition)
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewInstanceDecisionItems",
    "@odata.count": 10,
    "value": [
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "b4cbd87c-0ee2-4647-a7e3-41b580ea6fed",
                "displayName": "Priviliged Role Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe",
                    "userPrincipalName": "johndoe@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "2e8e717b-a857-49f0-918a-013cf0415456",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe 1",
                    "userPrincipalName": "johndoe1@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "20a97808-56dd-490a-97a9-73bf2344cce7",
                "displayName": "Hello world",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        }
    ]
}
```
