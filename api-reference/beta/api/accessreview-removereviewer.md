---
title: 删除 accessReview 审阅者
description: '在 Azure AD 访问评论功能中，更新要删除的用户审阅者作为现有 accessReview 对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 84bf3d973820067e0d4561e9647f688c025d957f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956687"
---
# <a name="remove-accessreview-reviewer"></a>删除 accessReview 审阅者

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新要删除的用户审阅者作为现有[accessReview](../resources/accessreview.md)对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 


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
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
应提供没有请求正文。


## <a name="response"></a>响应
如果成功，则此方法将返回 200 系列响应代码。

## <a name="example"></a>示例

这是更新一次性 （不) 访问回顾删除不必要的审阅者的示例。


##### <a name="request"></a>请求
在请求 URL 中，提供 accessReview 对象的 id，然后用户对象的 id。

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
