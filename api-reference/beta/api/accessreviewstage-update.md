---
title: 更新 accessReviewStage
description: 更新 accessReviewStage 对象的属性。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3441d93ab31270915fb1139e30c65e67ab28a197
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816135"
---
# <a name="update-accessreviewstage"></a>更新 accessReviewStage
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [accessReviewStage 对象](../resources/accessreviewstage.md) 的属性。 只能 **更新审阅****者和 fallbackReviewers** 属性。 只能将审阅者添加到 **fallbackReviewers** 属性，但无法删除现有的 **fallbackReviewers**。

若要更新 **accessReviewStage**， **其状态** 必须为 `NotStarted`、 `Initializing`或 `InProgress`。

> [!NOTE]
> 
> 更新 **accessReviewStage** 将仅更新该阶段。 父 **accessReviewInstance** 和任何将来的 **accessReviewStage** 对象不会更改。 若要进行适用于所有未来实例和阶段的更新，请更新父 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|reviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此访问评审范围集合用于定义审阅者是谁。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-scope-concept)。 可选。 可更新。|
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。 可选。 可更新。|



## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [accessReviewStage](../resources/accessreviewstage.md) 对象。

尝试删除现有的 **fallbackReviewers** 将返回 响应 `409 Conflict` 代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_accessreviewstage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5dcfcc88-da88-4252-8629-a0807b4b076d/instances/720b8ee0-cee4-42ac-b164-894c48703acc/stages/7d244ab1-4ab1-7d24-b14a-247db14a247d
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "reviewers": [
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ],
  "fallbackReviewers": [
      {
          "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
          "queryType": "MicrosoftGraph"
      },
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ]
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewStage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "id": "7d244ab1-4ab1-7d24-b14a-247db14a247d",
  "startDateTime": "2021-12-14T11:15:43.207Z",
  "endDateTime": "2021-12-15T11:15:43.207Z",
  "status": "InProgress",
  "reviewers": [
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ],
  "fallbackReviewers": [
      {
          "query": "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
          "queryType": "MicrosoftGraph"
      },
      {
          "query": "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
          "queryType": "MicrosoftGraph"
      }
  ]
}
```

