---
title: 创建 accessReview
description: 在 Azure AD 访问评审功能中，创建新的 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d53f0335ed9b130be65611d049645aba6a7abe44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439406"
---
# <a name="create-accessreview"></a>创建 accessReview

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，创建新的 [accessReview](../resources/accessreview.md) 对象。

在提出此请求之前，调用方之前必须已[](businessflowtemplate-list.md)检索到业务流程模板的列表，才能将值 `businessFlowTemplateId` 包括在请求中。

提出此请求后，调用方应 [创建一个 programControl，](programcontrol-create.md)以将访问评审链接到程序。  

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | AccessReview.ReadWrite.Membership |

调用方还应具有 ProgramControl.ReadWrite.All 权限，以便创建访问评审后，调用方可以创建[programControl。](../resources/programcontrol.md)
此外，已登录用户还必须具有允许其创建访问评审的目录角色。  有关详细信息，请参阅访问评审的角色 [和权限要求](../resources/accessreviews-root.md)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
| Authorization | 持有者 \{token\}。 必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。

下表显示创建 accessReview 时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | 访问评审名称。  |
| `startDateTime`           |`DateTimeOffset`                                                | 计划开始审阅的日期/时间。  这必须是将来的日期。   |
| `endDateTime`             |`DateTimeOffset`                                                | 计划结束审阅的日期/时间。 这必须至少比开始日期晚一天。   |
| `description`             |`String`                                                        | 向审阅者显示的说明。 |
| `businessFlowTemplateId`  |`String`                                                        | 从 [businessFlowTemplate](../resources/businessflowtemplate.md)获取的业务流程模板标识符。  |
| `reviewerType`            |`String`                                                        | 审阅者对已审阅对象的访问权的关系类型，其中一 `self` 个 ，或 `delegated` `entityOwners` 。 | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | 创建访问评审的对象，例如组的成员身份或向应用程序分配用户。 | 


如果提供的 reviewerType 具有值，则调用方还必须包含具有 `delegated` `reviewers` 审阅者 [用户](../resources/useridentity.md) 标识集合的属性。

如果你的应用在没有登录用户的情况下调用此 API，则调用方还必须包含 **createdBy** 属性，其值为将标识为评价创建者的用户的用户标识 [](../resources/useridentity.md)。

此外，呼叫者还可以包括设置，以创建定期审阅系列或更改默认审阅行为。 具体而言，若要创建定期审阅，呼叫者必须在访问评审设置 `accessReviewRecurrenceSettings` 中包括


## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应代码 `201, Created` 和 [accessReview](../resources/accessreview.md) 对象。

## <a name="example"></a>示例

这是一个创建一次性网站（而不是定期 (访问) ，明确将两个用户指定为审阅者的示例。

### <a name="request"></a>请求
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。

<!-- {
  "blockType": "ignored",
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

### <a name="response"></a>响应
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


