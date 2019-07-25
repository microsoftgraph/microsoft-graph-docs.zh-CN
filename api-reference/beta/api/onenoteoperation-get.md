---
title: 获取 onenoteOperation
description: '获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d5af90f9600d62a800683da444a0470f857ffa56
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878779"
---
# <a name="get-onenoteoperation"></a>获取 onenoteOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取长时间运行的 OneNote 操作的状态。 这适用于在响应中返回**操作位置**标头的`CopyNotebook`操作, 例如`CopyToNotebook`、、 `CopyToSectionGroup`、。 `and CopyToSection`   

您可以轮询操作-位置终结点, 直到`status`属性返回`completed`或`failed`。 

如果状态为`completed`, 则`resourceLocation`属性包含资源终结点 URI。 

如果状态为`failed`, 则错误和`@api.diagnostics`属性将提供错误信息。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Notes.Create、Notes.Read、Notes.ReadWrite    |
|应用程序 | Notes.Read.All、Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
无。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| 接受 | string | `application/json` |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenoteOperation](../resources/onenoteoperation.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
