---
title: 更新 accessReview
description: 在Azure AD查看功能中，更新现有 accessReview 对象以更改其一个或多个属性。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 112d341d2be082d04041dcee50a66ba85af37ebc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987998"
---
# <a name="update-accessreview"></a>更新 accessReview

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在Azure AD[查看](../resources/accessreviews-root.md)功能中，更新现有[accessReview](../resources/accessreview.md)对象以更改其一个或多个属性。

此 API 不用于更改审阅者或审阅决策。  若要更改审阅者，请使用 [addReviewer](accessreview-addreviewer.md) 或 [removeReviewer](accessreview-removereviewer.md) API。  若要停止已启动的一次性审阅或已启动的定期审阅实例，请尽早使用 [停止](accessreview-stop.md) API。 若要将决策应用于目标组或应用访问权限，请使用 [应用](accessreview-apply.md) API。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All |
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

下表显示更新 accessReview 时提供的属性。

| 属性      | 类型           | 说明                                                                                                |
|:--------------|:---------------|:-----------------------------------------------------------------------------------------------------------|
| displayName   | String         | 访问评审名称。                                                                                    |
| startDateTime | DateTimeOffset | 计划启动审阅的 DateTime。  这必须是将来的日期。                 |
| endDateTime   | DateTimeOffset | 计划结束审阅的 DateTime。 这必须至少比开始日期晚一天。 |
| 说明   | String         | 向审阅者显示的说明。                                                                 |



## <a name="response"></a>响应
如果成功，此方法在响应 `204 Accepted` 正文中返回 响应代码和 [accessReview](../resources/accessreview.md) 对象。

## <a name="example"></a>示例

这是一个更新一次访问 (访问) 的示例。

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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreview-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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


