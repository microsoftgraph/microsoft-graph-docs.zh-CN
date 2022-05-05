---
title: documentSetVersion：restore
description: 还原 documentSetVersion。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 3a000fa0d7add3c225f545bde24dcf5983e8a7e9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205988"
---
# <a name="documentsetversion-restore"></a>documentSetVersion：restore
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

还原 [文档集版本](../resources/documentsetversion.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All、Sites.Selected|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/documentSetVersions/{documentSetVersionId}/restore
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "documentsetversionthis.restore"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/root/lists/Documents/items/2/documentSetVersions/1/restore
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/documentsetversionthisrestore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/documentsetversionthisrestore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/documentsetversionthisrestore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/documentsetversionthisrestore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/documentsetversionthisrestore-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "name": "documentsetversionthis.restore",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

