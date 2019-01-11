---
title: 更新 accessReview
description: 在 Azure AD 访问评论功能中，更新现有 accessReview 对象更改一个或多个其属性。
localization_priority: Normal
ms.openlocfilehash: 65420b3682eb9d9f72d95beea624eb84429628ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833745"
---
# <a name="update-accessreview"></a>更新 accessReview

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新现有[accessReview](../resources/accessreview.md)对象更改一个或多个其属性。

此 API 不是要更改的审阅者或评审的决策。  若要更改审阅者，请使用[addReviewer](accessreview-addreviewer.md)或[removeReviewer](accessreview-removereviewer.md) Api。  停止已启动一次性审阅中或已启动的定期查看实例、 早期，使用[停止](accessreview-stop.md)API 和决策于目标组或应用程序访问权限，使用[应用](accessreview-apply.md)API。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必填。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供[accessReview](../resources/accessreview.md)对象的参数的 JSON 表示形式。

下表显示可更新 accessReview 时提供的属性。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | 访问审阅名称。  |
| `startDateTime`           |`DateTimeOffset`                                                | 审阅安排在启动时 DateTime。  这必须是在将来的日期。   |
| `endDateTime`             |`DateTimeOffset`                                                | 审阅安排结束时 DateTime。 这必须是至少一个日期晚于开始日期。   |
| `description`             |`String`                                                        | 说明，向审阅者显示。 |



## <a name="response"></a>响应
如果成功，此方法返回`204, Accepted`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。

## <a name="example"></a>示例

这是一次性的 （不) 访问审阅更新的示例。

##### <a name="request"></a>请求
在请求正文中，提供[accessReview](../resources/accessreview.md)对象的新属性的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
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
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
