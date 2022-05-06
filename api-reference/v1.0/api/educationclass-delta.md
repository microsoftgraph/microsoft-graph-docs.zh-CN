---
title: educationClass： delta
description: 获取新创建的或更新的类，包括成员身份更改，而无需对整个类集合执行完整读取。
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 254c72645bb4b21b7c81e20cb8ee9c4fe4809089
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247019"
---
# <a name="educationclass-delta"></a>educationClass： delta

命名空间：microsoft.graph

获取新创建的或更新的类，包括成员身份更改，而无需对整个类集合执行完整读取。 有关详细信息，请参阅 [“使用增量查询](/graph/delta-query-overview) ”。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | EduRoster.ReadBasic、EduRoster.Read 或 EduRoster.ReadWrite              |
| 委派（个人 Microsoft 帐户） | 不支持。                                                           |
| Application                            | EduRoster.ReadBasic.All、EduRoster.Read.All 或 EduRoster.ReadWrite.All |

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

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 集合。 该响应还包括 `@odata.nextLink`URL 或 `@odata.deltaLink`URL。

- `@odata.nextLink`如果返回 URL，则会话中将检索其他数据页。 应用程序继续使用 `@odata.nextLink` URL 发出请求，直到响应中包含 `@odata.deltaLink` URL。
- `@odata.deltaLink`如果返回 URL，则不再有关于要返回的资源的现有状态的数据。 保留并使用 `@odata.deltaLink` URL 了解将来对资源所做的更改。

有关详细信息，请参阅 [使用增量查询](/graph/delta-query-overview)。 有关请求的示例，请参阅 [获取用户的增量更改](/graph/delta-query-users)。

> [!IMPORTANT]
> educationClass 增量不包括已删除的类。

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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationclass-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/educationclass-delta-powershell-snippets.md)]
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
