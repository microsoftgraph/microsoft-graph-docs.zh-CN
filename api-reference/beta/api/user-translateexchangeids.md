---
title: 用户： translateExchangeIds
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571287"
---
# <a name="user-translateexchangeids"></a>用户： translateExchangeIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对与 Outlook 相关的资源的标识符进行格式转换。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | User.ReadBasic、 User.Read、 User.ReadWrite、 User.ReadBasic.All、 User.Read.All、 User.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | User.ReadBasic，User.Read，User.ReadWrite |
| Application | User.Read.All、User.ReadWrite.All |

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
| inputIds | Edm.String 集合 | 要转换的标识符的集合。 集合中的所有标识符必须具有相同的源 ID 类型，并且必须是同一邮箱中项目的。 此集合的最大大小是 1000年字符串。 |
| sourceIdType | exchangeIdFormat | ID 类型的标识符的`InputIds`参数。 |
| targetIdType | exchangeIdFormat | 要转换的请求的 ID 类型。 |

### <a name="exchangeidformat-values"></a>exchangeIdFormat 值

| 值 | 说明 |
|:-------|:------------|
| entryId | MAPI 客户端使用二进制条目 ID 格式。 |
| ewsId | 使用 Exchange Web 服务客户端 ID 格式。 |
| immutableEntryId | 二进制 MAPI 兼容变 ID 的格式。 |
| restId | 由 Microsoft Graph 中使用的默认 ID 格式。 |
| restImmutableEntryId | 由 Microsoft Graph 变 ID 格式。 |

二进制格式 (`entryId`和`immutableEntryId`) 的 URL 安全 base64 编码。 URL safeness 实现通过修改 base64 编码的二进制数据采用以下方式：

- 替换`+`与`-`
- 替换`/`与`_`
- 删除任何尾随空白字符 (`=`)
- 指示在原始了多少填充字符的字符串的末尾添加一个整数 (`0`， `1`，或`2`)

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的[convertIdResult](../resources/convertidresult.md)集合。

## <a name="example"></a>示例

下面的示例演示如何将多个标识符转换从普通的 REST API 格式 (`restId`) 为 REST 变格式 (`restImmutableEntryId`)。

### <a name="request"></a>请求

下面展示了示例请求。
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
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
