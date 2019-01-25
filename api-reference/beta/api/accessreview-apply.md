---
title: 应用 accessReview
description: '在 Azure AD 中访问评论功能、 apply 完成 accessReview 的决策。  目标对象可以是一次性访问回顾或定期访问评审的实例。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512211"
---
# <a name="apply-accessreview"></a>应用 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能应用完成[accessReview](../resources/accessreview.md)的决策。  目标对象可以是一次性访问回顾或定期访问评审的实例。  


访问审阅完毕后，或者因为它到达的结束日期或管理员手动停止，将自动应用未配置供审阅，您可以调用应用，以应用所做的更改。 应用，发生此事件，直到要删除的访问权限的决定不显示对源资源，用户例如保留其组成员身份。 通过调用应用，由更新的组或应用程序实现的审阅结果。 如果用户的访问被拒绝在审阅中，当管理员调用此 API，Azure AD 中删除其成员身份或应用程序的工作分配。 

访问查看已完成，并自动应用之后进行配置，然后查看的状态将从已完成通过中间状态更改和最后将更改为状态应用。 您应该会看到拒绝的用户，如果要删除资源中的任何组成员身份或应用程序的工作分配，请过几分钟。

配置的自动应用审阅，或选择应用不会影响的本地目录中的组或动态组。 如果您想要更改组的内部部署，下载结果并将这些更改应用于该目录中的组的表示形式。


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
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者令牌 必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="see-also"></a>另请参阅

- [如何完成访问审阅](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
