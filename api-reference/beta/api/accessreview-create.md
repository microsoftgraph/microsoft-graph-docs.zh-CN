---
title: 创建 accessReview
description: 在 Azure AD 访问评审功能中，创建新的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fd1f6c25dcc4013c1abc3d39dafa63723a1e3ea0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751116"
---
# <a name="create-accessreview"></a>创建 accessReview

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，创建新的 [accessReview](../resources/accessreview.md) 对象。

进行此请求之前，调用方之前必须已检索 [](businessflowtemplate-list.md)到业务流模板的列表，才能将 **businessFlowTemplateId** 的值包括在请求中。

提出此请求后，调用方应 [创建 programControl，](programcontrol-create.md)以将访问评审链接到程序。  

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.ReadWrite.Membership |

调用方还应具有 ProgramControl.ReadWrite.All 权限，以便创建访问评审后，调用方可以创建 [programControl](../resources/programcontrol.md)。
此外，登录用户还必须具有允许其创建访问评审的目录角色。  有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviews-root.md)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
| Authorization | 持有者 \{token\}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。

下表显示创建 accessReview 时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| displayName             |String                                                        | 访问评审名称。  |
| startDateTime           |DateTimeOffset                                                | 计划开始审阅的 DateTime。  这必须是将来的日期。   |
| endDateTime             |DateTimeOffset                                                | 计划结束审阅的 DateTime。 这必须至少比开始日期晚一天。   |
| 说明             |String                                                        | 向审阅者显示的说明。 |
| businessFlowTemplateId  |String                                                        | 从 [businessFlowTemplate](../resources/businessflowtemplate.md)获取的业务流程模板标识符。  |
| reviewerType            |String                                                        | 审阅者对被审阅对象的访问权的关系类型，如 、 或 `self` `delegated` `entityOwners` 。 | 
| reviewedEntity          |[identity](../resources/identity.md)                                     | 创建访问评审的对象，例如组的成员身份或用户到应用程序的分配。 | 


如果 **reviewerType** 具有值，则调用方还必须包含 `delegated` **reviewers** 属性，其中 [userIdentity](../resources/useridentity.md) 对象集合代表审阅者。

如果你的应用在没有登录用户的情况下调用此 API，则调用方还必须包含 **createdBy** 属性，其值为将被标识为评价创建者的用户的 [userIdentity。](../resources/useridentity.md)

此外，呼叫者可以包含 **设置**，以创建定期审阅系列或更改默认审阅行为。 具体而言，若要创建定期审阅，呼叫者必须在访问评审设置中包括[accessReviewRecurrenceSettings，](../resources/accessreviewrecurrencesettings.md)


## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [accessReview](../resources/accessreview.md) 对象。

## <a name="example"></a>示例

这是一个创建一次性网站，而不是 (访问) ，明确指定两个用户作为审阅者的示例。

### <a name="request"></a>请求
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


