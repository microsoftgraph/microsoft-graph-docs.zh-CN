---
title: 创建书签
description: 创建新的书签对象。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 84283c08a8e80427ff34a310cbcae799bd26ecef
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602747"
---
# <a name="create-bookmark"></a>创建书签
命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [书签](../resources/search-bookmark.md) 对象。

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
}-->
```http
POST /search/bookmarks
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [书签](../resources/search-bookmark.md) 对象的 JSON 表示形式。

下表显示了创建 [书签](../resources/search-bookmark.md)时可用的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|搜索结果中显示的书签名称。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|说明|String|搜索结果页上显示的书签说明。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|webUrl|String|书签 URL 链接。 当用户在搜索结果中单击此书签时，他们将转到此 URL。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|类别|String 集合|通常用于描述此书签的类别。 例如，IT 和 HR。|
|availabilityStartDateTime|DateTimeOffset|书签何时开始显示为搜索结果的时间戳。 `null`设置为始终可用。|
|availabilityEndDateTime|DateTimeOffset|书签何时停止显示为搜索结果的时间戳。 `null`设置为始终可用。|
|languageTags|字符串集合|能够查看此书签的国家或地区的列表。|
|平台|microsoft.graph.devicePlatformType 集合|能够查看此书签的设备和操作系统的列表。 可取值为：`unknown`、`android`、`androidForWork`、`ios`、`macOS`、`windowsPhone81`、`windowsPhone81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidASOP`。|
|targetedVariations|[microsoft.graph.search.answerVariant](../resources/search-answerVariant.md) 集合|不同国家或设备的书签的变体。 需要根据用户的设备、国家/地区或两者向用户显示不同内容时使用。 日期和组设置将应用于所有变体。|
|powerAppIds|字符串集合|与此书签关联的Power Apps列表。 如果用户将现有Power Apps添加到书签，则他们可以完成任务，例如输入休假时间或在搜索结果页上报告费用。|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|触发此书签以显示在搜索结果中的关键字。|
|state|microsoft.graph.search.answerState|书签的状态。 可能的值为：`published`、`draft`或 `excluded``unknownFutureValue`。|
|groupIds|String collection|能够查看此书签的安全组列表。|



## <a name="response"></a>响应

如果成功，此方法将返回包含 `201 Created` 所创建书签 ID 的响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": null,
  "availabilityEndDateTime": null,
  "platforms": ["windows"],
  "targetedVariations": [
    {
      "languageTag": "es-es",
      "displayName": "Sitio de instalación Contoso",
      "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
    }
  ],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookmark-from-bookmarks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookmark-from-bookmarks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookmark-from-bookmarks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookmark-from-bookmarks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-bookmark-from-bookmarks-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-bookmark-from-bookmarks-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

