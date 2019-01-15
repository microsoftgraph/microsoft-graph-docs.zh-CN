---
title: 创建 accessReview
description: Azure AD 中访问审阅功能，创建一个新的 accessReview 对象。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de8574566a8ca1eedb1f0f55230fb91053370ccc
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016721"
---
# <a name="create-accessreview"></a>创建 accessReview

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[accessReview](../resources/accessreview.md)对象。

此请求之前，呼叫者必须具有之前[检索业务流程模板列表中的](businessflowtemplate-list.md)，具有的值`businessFlowTemplateId`要包含在请求中。

进行此请求之后, 将呼叫者应[创建 programControl](programcontrol-create.md)，若要访问评审链接到的程序。  

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All，也应具有完成后续呼叫中以创建 programControl 方案的 ProgramControl.ReadWrite.All 和 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。

下表显示时创建 accessReview 所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | 访问审阅名称。  |
| `startDateTime`           |`DateTimeOffset`                                                | 审阅安排在启动时 DateTime。  这必须是在将来的日期。   |
| `endDateTime`             |`DateTimeOffset`                                                | 审阅安排结束时 DateTime。 这必须是至少一个日期晚于开始日期。   |
| `description`             |`String`                                                        | 说明，向审阅者显示。 |
| `businessFlowTemplateId`  |`String`                                                        | 业务流程模板标识符，从[businessFlowTemplate](../resources/businessflowtemplate.md)获得。  |
| `reviewerType`            |`String`                                                        | 审阅者已审阅对象之一的访问权限的关系类型`self`， `delegated`，或`entityOwners`。 | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | 为其访问审阅创建对象，如组的成员身份或向应用程序的用户的分配。 | 


如果要提供 reviewerType 具有值`delegated`，然后将呼叫者还必须包括`reviewers`属性，与[userIdentity](../resources/useridentity.md)审阅者的集合。

此外，呼叫者可以包括设置，以创建定期查看系列或更改默认查看行为。 具体而言，若要创建定期查看，呼叫者必须包括`accessReviewRecurrenceSettings`中访问检查设置，


## <a name="response"></a>响应
如果成功，此方法返回`201, Created`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。

## <a name="example"></a>示例

这是创建一次性 （而不是定期） 访问回顾，显式指定为审阅者的两个用户的一个示例。

##### <a name="request"></a>请求
在请求正文中，提供[accessReview](../resources/accessreview.md)对象的 JSON 表示形式。

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

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
