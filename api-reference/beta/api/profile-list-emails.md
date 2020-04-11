---
title: 列出电子邮件
description: 检索 itemEmail 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b51f1f16cb55d69c043a6b76b4ea98a4684bf906
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228665"
---
# <a name="list-emails"></a>列出电子邮件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从用户的[配置文件](../resources/profile.md)中检索[itemEmail](../resources/itememail.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User. Read、User.readbasic.all、user. all、All、user. all。 All |
| 委派（个人 Microsoft 帐户） | User. Read、User.readbasic.all、user. all、All、user. all。 All |
| Application                            | User.readbasic.all、所有用户读写全部。 All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

|名称            |值    |说明                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |将响应限制为仅包含指定条件的那些对象。                                                                                             |
|$orderby        |string   |默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。 您可以使用 *$orderby*参数更改响应的顺序。|
|$select         |string   |要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。                                        |
|$skip           |int      |跳过前 n 个结果，对于分页非常有用。                                                                                                                                |
|$top            |int      |要返回的结果数。                                                                                                                                           |

## <a name="request-headers"></a>请求标头

| 名称           |说明                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}。必需。   |


## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[itemEmail](../resources/itememail.md)对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/emails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "address": "address-value",
      "displayName": "displayName-value",
      "type": "type-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List emails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
