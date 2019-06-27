---
title: 'outlookUser: supportedLanguages'
description: 获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bfcef9f61978fa0c00e6e3ba32af55a114ea0f9a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267779"
---
# <a name="outlookuser-supportedlanguages"></a>outlookUser: supportedLanguages

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取用户支持的区域设置和语言列表，用户的邮箱服务器上配置了此信息。

在设置 Outlook 客户端时，用户从此受支持的列表中选择首选语言。 随后可以通过[获取用户的邮箱设置](user-get-mailboxsettings.md)获取首选语言。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read、User.ReadBasic.All    |
|委派（个人 Microsoft 帐户） | User.Read    |
|Application | User.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedLanguages
GET /users/{id|userPrincipalName}/outlook/supportedLanguages
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |


## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [localeInfo](../resources/localeinfo.md) 对象的集合。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "user_supportedlanguages"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedLanguages
```

##### <a name="response"></a>响应
下面是一个响应示例。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localeInfo",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.localeInfo)",
  "value":[
    {
      "locale":"af-ZA",
      "displayName":"Afrikaans (Suid-Afrika)"
    },
    {
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    {
       "locale":"en-CA",
       "displayName":"English (Canada)"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedlanguages-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedLanguages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedlanguages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
