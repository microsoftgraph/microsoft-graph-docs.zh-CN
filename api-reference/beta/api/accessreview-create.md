---
title: 创建 accessReview
description: 在 "Azure AD access 评论" 功能中, 创建一个新的 accessReview 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab1711a370d766631611d9cd5f96635760f98f48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946054"
---
# <a name="create-accessreview"></a>创建 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 创建一个新的[accessReview](../resources/accessreview.md)对象。

在发出此请求之前, 呼叫者必须先[检索业务流模板列表](businessflowtemplate-list.md), 才能将值`businessFlowTemplateId`包含在请求中。

发出此请求后, 调用方应[创建一个 programControl](programcontrol-create.md), 以将访问审核链接到某个程序。  

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

调用方还应具有 ProgramControl 权限, 以便在创建访问审核之后, 调用方可以创建[ProgramControl](../resources/programcontrol.md)。
此外, 登录用户还必须位于允许他们创建访问审阅的目录角色中。  有关更多详细信息, 请参阅[access 评审](../resources/accessreviews-root.md)的角色和权限要求。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。

下表显示创建 accessReview 时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | 访问审阅名称。  |
| `startDateTime`           |`DateTimeOffset`                                                | 计划开始评审时的日期时间。  这必须是将来的日期。   |
| `endDateTime`             |`DateTimeOffset`                                                | 计划结束评审时的日期/时间。 此时间必须至少为一个晚于开始日期的一天。   |
| `description`             |`String`                                                        | 要向审阅者显示的说明。 |
| `businessFlowTemplateId`  |`String`                                                        | 从[businessFlowTemplate](../resources/businessflowtemplate.md)获取的业务流模板标识符。  |
| `reviewerType`            |`String`                                                        | 审阅者的关系类型: 审阅的对象的访问权限、 `self` `delegated`、或。 `entityOwners` | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | 为其创建访问审核的对象, 例如组的成员身份或向应用程序分配的用户。 | 


如果要提供的 reviewerType 具有值`delegated`, 则调用方还必须包括该`reviewers`属性, 其中包含审阅人的[userIdentity](../resources/useridentity.md)的集合。

如果您的应用程序在没有登录用户的情况下调用此 API, 则呼叫者还必须包含**createdBy**属性, 其值是将被标识为审阅的创建者的用户的[userIdentity](../resources/useridentity.md) 。

此外, 呼叫者还可以包括设置、创建定期审阅系列或从默认的审阅行为更改。 特别是, 若要创建定期检查, 呼叫者必须在 " `accessReviewRecurrenceSettings`访问审核设置" 中包含 "",


## <a name="response"></a>响应
如果成功, 此方法在响应`201, Created`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。

## <a name="example"></a>示例

下面的示例演示了如何创建一次性 (非定期) 访问审核, 并将两个用户显式指定为审阅者。

##### <a name="request"></a>请求
在请求正文中, 提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
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
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
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
