---
title: 创建 qna
description: 创建新的 qna 对象。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d3b2266238a74b052aba433c75e5b91d08669386
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602719"
---
# <a name="create-qna"></a>创建 qna
命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [qna](../resources/search-qna.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| SearchConfiguration.Read.All、SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /search/qnas
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [qna](../resources/search-qna.md) 对象的 JSON 表示形式。

下表显示了创建 [qna](../resources/search-qna.md) 时可用的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|搜索结果中显示的问题。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|说明|String|搜索结果中显示的答案。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|webUrl|String|Qna URL 链接。 当用户在搜索结果中单击此 qna 时，他们将转到此 URL。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|availabilityStartDateTime|DateTimeOffset|qna 何时开始显示为搜索结果的时间戳。 `null`设置为始终可用。|
|availabilityEndDateTime|DateTimeOffset|qna 何时停止显示为搜索结果的时间戳。 `null`设置为始终可用。|
|languageTags|字符串集合|能够查看此 qna 的国家或地区的列表。|
|平台|microsoft.graph.devicePlatformType 集合|能够查看此 qna 的设备和操作系统的列表。 可取值为：`unknown`、`android`、`androidForWork`、`ios`、`macOS`、`windowsPhone81`、`windowsPhone81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidASOP`。|
|targetedVariations|[microsoft.graph.search.answerVariant](../resources/search-answerVariant.md) 集合|不同国家/地区或设备的 qna 变体。 需要根据用户的设备、国家/地区或两者向用户显示不同内容时使用。 日期和组设置将应用于所有变体。|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|触发此 qna 以显示在搜索结果中的关键字。|
|state|microsoft.graph.search.answerState|qna 的状态。 可能的值为：`published`、`draft`或 `excluded``unknownFutureValue`。|
|groupIds|String collection|能够查看此 qna 的安全组列表。|



## <a name="response"></a>响应

如果成功，此方法将返回包含 `201 Created` 所创建的问答 ID 的响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_qna_from_qnas"
}-->
```http
POST https://graph.microsoft.com/beta/search/qnas
Content-Type: application/json

{
  "displayName": "Global Country Holidays",
  "webUrl": "http://www.contoso.com/",
  "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>",
  "keywords":  {
    "keywords": ["new years day", "martin luther king day", "presidents day", "memorial day", "independence day", "labor day", "thanksgiving", "christmas"],
    "reservedKeywords": ["holidays", "paid days off"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": "2020-09-21T20:01:37Z",
  "availabilityEndDateTime": "2021-12-31T20:01:37Z",
  "languageTags": ["en-us"],
  "platforms": ["ios"],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-qna-from-qnas-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-qna-from-qnas-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-qna-from-qnas-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-qna-from-qnas-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-qna-from-qnas-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-qna-from-qnas-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面是一个响应示例。
<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.qna"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

