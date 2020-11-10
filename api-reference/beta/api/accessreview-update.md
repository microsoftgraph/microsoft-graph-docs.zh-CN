---
title: 更新 accessReview
description: 在 "Azure AD 访问评论" 功能中，更新现有 accessReview 对象以更改其一个或多个属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1229729f2d3d149bf06d5a6308fa659ed56dcca7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952605"
---
# <a name="update-accessreview"></a>更新 accessReview

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [访问评论](../resources/accessreviews-root.md) " 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象以更改其一个或多个属性。

此 API 不用于更改审阅的审阅者或决策。  若要更改审阅者，请使用 [addReviewer](accessreview-addreviewer.md) 或 [removeReviewer](accessreview-removereviewer.md) api。  若要停止已启动的一次性审核，或提前审核已启动的定期检查实例，请提前使用 [stop](accessreview-stop.md) API。 若要将决策应用于目标组或应用访问权限，请使用 [应用](accessreview-apply.md) API。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview、AccessReview 和所有 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的参数的 JSON 表示形式。

下表显示了在更新 accessReview 时可提供的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | 访问审阅名称。  |
| `startDateTime`           |`DateTimeOffset`                                                | 计划开始评审时的日期时间。  这必须是将来的日期。   |
| `endDateTime`             |`DateTimeOffset`                                                | 计划结束评审时的日期/时间。 此时间必须至少为一个晚于开始日期的一天。   |
| `description`             |`String`                                                        | 要向审阅者显示的说明。 |



## <a name="response"></a>响应
如果成功，此方法 `204, Accepted` 在响应正文中返回响应代码和 [accessReview](../resources/accessreview.md) 对象。

## <a name="example"></a>示例

此示例将更新一次性 (不会定期) 访问审核。

##### <a name="request"></a>请求
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的新属性的 JSON 表示形式。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
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
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
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
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


