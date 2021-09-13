---
title: educationClass： delta
description: 获取新创建或更新的类（包括成员身份更改）而无需执行整个类集合的完全读取。
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: aed767ea0e4cd9ca2542f3ef34692ca8cc4d1536
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59114678"
---
# <a name="educationclass-delta"></a>educationClass： delta

命名空间：microsoft.graph

获取新创建或更新的类（包括成员身份更改）而无需执行整个类集合的完全读取。 有关详细信息 [，请参阅使用 delta](/graph/delta-query-overview) 查询。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | EduRoster.ReadBasic、EduRoster.Read 或 EduRoster.ReadWrite              |
| 委派（个人 Microsoft 帐户） | 不支持。                                                           |
| 应用程序                            | EduRoster.ReadBasic.All、EduRoster.Read.All 或 EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [educationClass](../resources/educationclass.md) 集合。 该响应还包括 `nextLink`URL 或 `deltaLink`URL。

- 如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。 应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。
- 如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。 保留并使用 `deltaLink` URL 了解将来对资源的更改。

有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。 有关示例请求，请参阅 [获取用户的增量更改](/graph/delta-query-users)。

> [!IMPORTANT]
> educationClass deltas 不包括已删除的类。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationClass)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/delta?$skiptoken=sU1S4IJGk3hwxbia8...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "String (identifier)",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
