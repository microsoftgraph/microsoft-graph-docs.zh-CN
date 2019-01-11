---
title: 添加 accessReview 审阅者
description: '在 Azure AD 访问评论功能中，更新要作为审阅者添加另一个用户现有 accessReview 对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 '
localization_priority: Normal
ms.openlocfilehash: ab339a6538fc41d7e538c51251302c5e589367f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838764"
---
# <a name="add-accessreview-reviewer"></a>添加 accessReview 审阅者

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新要作为审阅者添加另一个用户现有[accessReview](../resources/accessreview.md)对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 


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
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必填。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供用户将成为审阅者的 ID 的 JSON 表示形式。

下表显示可更新 accessReview 时提供的属性。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | 用户 id。  |


## <a name="response"></a>响应
如果成功，此方法返回`201, Created`响应代码。

## <a name="example"></a>示例

这是一次性的 （不) 访问审阅更新与其他审阅者的示例。

##### <a name="request"></a>请求
在请求正文中，提供的用户对象的 id 的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
