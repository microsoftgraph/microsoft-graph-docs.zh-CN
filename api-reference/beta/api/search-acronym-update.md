---
title: 更新首字母缩略词
description: 更新首字母缩写词对象的属性。
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b82b09e80d4be7b3250707a1006b682e13d4e67d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338332"
---
# <a name="update-acronym"></a>更新首字母缩略词
命名空间：microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新首字母缩写 [词对象](../resources/search-acronym.md) 的属性。

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
PATCH /search/acronyms/{acronymsId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供首字母缩写词对象的 JSON [表示](../resources/search-acronym.md) 形式。 提供应更新的相关字段的值。 请求正文中未包含的现有属性将保留其以前的值或根据其他属性值的更改重新计算。 为了实现最佳性能，不得添加未变化的现有值。

|属性|类型|说明|
|:---|:---|:---|
|说明|String|A brief description of the acronym that gives users more info about the acronym and what it stands for. 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|displayName|String|实际的短格式或缩写。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|
|standsFor|String 集合|首字母缩写词代表什么。|
|state|microsoft.graph.search.answerState|首字母缩写词的状态。 可能的值是：、`published``draft`、`excluded`或 `unknownFutureValue`。|
|webUrl|String|用户可以访问的页面或网站的 URL，以了解有关缩写词详细信息。 继承自 [searchAnswer](../resources/search-searchAnswer.md)。|



## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_acronym"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/search/acronyms/{acronymsId}
Content-Type: application/json

{
  "description": "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-acronym-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-acronym-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-acronym-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-acronym-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-acronym-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-acronym-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

