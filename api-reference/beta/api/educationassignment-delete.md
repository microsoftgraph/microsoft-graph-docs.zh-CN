---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有课堂中的教师才能删除工作分配。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 10a66116b9fb3443cce72641fd8ffb7f63d6fee0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750036"
---
# <a name="delete-educationassignment"></a>删除 educationAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除现有工作分配。 只有课堂中的教师才能删除工作分配。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）             |
| :------------------------------------- | :------------------------------------------------------ |
| 委派（工作或学校帐户）     | EduAssignments、ReadWriteBasic、EduAssignments |
| 委派（个人 Microsoft 帐户） | 不支持。                                          |
| 应用程序                            | 不支持。                                          |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a>请求标头

| 标头        | 值                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a>响应
下面是一个响应示例。 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

#### <a name="sdk-sample-code"></a>SDK 示例代码

# <a name="ctabcs"></a>[C#](#tab/cs)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
