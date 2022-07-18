---
title: 更新 accessReviewStage
description: 更新 accessReviewStage 对象的属性。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e1862cb9da2bc234c3037f11c2de68557f9462cc
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697258"
---
# <a name="update-accessreviewstage"></a>更新 accessReviewStage
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [accessReviewStage](../resources/accessreviewstage.md) 对象的属性。 只能更新 **审阅者** 和 **fallbackReviewers** 属性。 只能将审阅者添加到 **fallbackReviewers** 属性，但不能删除现有的 **FallbackReviewers**。

若要更新 **accessReviewStage**，其 **状态** 必须为`NotStarted`或 `Initializing``InProgress`.

> [!NOTE]
> 
> 更新 **accessReviewStage** 将仅更新该阶段。 父 **accessReviewInstance** 和任何将来 **的 accessReviewStage** 对象不会更改。 若要进行适用于所有未来实例和阶段的更新，请更新父 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用                            | AccessReview.ReadWrite.All |

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
|评论家|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此访问评审范围集合用于定义审阅者是谁。 有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-scope-concept)。 可选。 更新。|
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。 可选。 更新。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [accessReviewStage](../resources/accessreviewstage.md) 对象。

尝试删除现有 **fallbackReviewers** 将返回 `409 Conflict` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewstage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewstage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewstage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewstage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewstage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

