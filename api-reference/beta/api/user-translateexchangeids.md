---
title: user： translateExchangeIds
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: abheek-das
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20fac290ea2baf68b2780e75224724616a2814c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341014"
---
# <a name="user-translateexchangeids"></a>user： translateExchangeIds

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对与 Outlook 相关的资源的标识符进行格式转换。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | User.ReadBasic.All、User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | User.ReadBasic.All、User.Read、User.ReadWrite |
| 应用程序 | User.Read.All、User.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a>请求标头

| 名称 | 值 |
|:-----|:------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

| 参数 | 类型 | 说明 |
|:----------|:-----|:------------|
| inputIds | String 集合 | 要转换的标识符的集合。 集合中所有标识符必须具有相同的源 ID 类型，并且必须为同一邮箱中的项目。 此集合的最大大小为 1000 个字符串。 |
| sourceIdType | exchangeIdFormat | 参数中标识符的 `InputIds` ID 类型。 |
| targetIdType | exchangeIdFormat | 要转换为的请求 ID 类型。 |

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

| 成员 | 说明 |
|:-------|:------------|
| entryId | MAPI 客户端使用的二进制条目 ID 格式。 |
| ewsId | Web 服务客户端使用的EXCHANGE ID 格式。 |
| immutableEntryId | 二进制 MAPI 兼容不可变 ID 格式。 |
| restId | Microsoft Graph 使用的默认 ID Graph。 |
| restImmutableEntryId | Microsoft Graph 使用的不可变 ID Graph。 |

二进制格式 (`entryId`) `immutableEntryId` URL 安全 base64 编码。 URL 安全通过按以下方式修改二进制数据的 base64 编码实现：

- 将 `+` 替换为 `-`
- 将 `/` 替换为 `_`
- 删除任何尾部填充字符 () `=`
- 在字符串末尾添加一`0`个整数，指示原始文本、、或 (填充 `1``2`) 

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 convertIdResult](../resources/convertidresult.md) 集合。

## <a name="example"></a>示例

以下示例演示如何将多个标识符从常规 REST API 格式 (`restId`) REST `restImmutableEntryId` 不可变格式 () 。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-translateexchangeids-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-translateexchangeids-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是示例响应
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


