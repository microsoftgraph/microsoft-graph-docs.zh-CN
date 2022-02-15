---
title: accessReviewStage： filterByCurrentUser
description: 返回给定审阅者的所有 accessReviewStage 对象。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f224acfdd86ca07a211a1389125524d90b7b8a07
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816144"
---
# <a name="accessreviewstage-filterbycurrentuser"></a>accessReviewStage： filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

返回给定 [accessReviewInstance](../resources/accessreviewinstance.md) 上的所有 [accessReviewStage](../resources/accessReviewStage.md) 对象，其中调用用户是一个或多个 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的审阅者。

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
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/filterByCurrentUser(on='reviewer')
```

## <a name="function-parameters"></a>函数参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|accessReviewStageFilterByCurrentUserOptions|根据调用用户筛选结果。 允许的值为 `reviewer`。 这将返回 accessReviewInstance 上调用用户为审阅者的所有 accessReviewStage 对象。 必需项。|

此函数还支持 、 `$select`、 `$filter``$orderBy`和 `$skip` `$top` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [accessReviewStage](../resources/accessreviewstage.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accessreviewstage_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/86889534-b102-4226-bfce-0c2aeee845df/stages/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewStage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewStage)",
    "@odata.count": 2,
    "value": [
        {
            "id": "9ac05ca6-396a-469c-8a8b-bcb98fceb2dd",
            "startDateTime": "2018-08-03T21:02:30.667Z",
            "endDateTime": "2018-08-13T21:17:30.513Z",
            "status": "Completed",
            "reviewers": [
                {
                    "query": "/groups/46d30af1-e626-4928-83f5-e9bfa400289e/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq
                    'USA'",
                    "type": "MicrosoftGraph"
                }
            ]
        },
        {
            "id": "03266a48-8731-4cfc-8a60-b2fa6648a14c",
            "startDateTime": "2018-08-14T21:02:30.667Z",
            "endDateTime": "2018-09-03T21:17:30.513Z",
            "status": "InProgress",
            "reviewers": [
                {
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions",
                    "query": "./manager",
                }
            ]
        }
    ]
}
```

