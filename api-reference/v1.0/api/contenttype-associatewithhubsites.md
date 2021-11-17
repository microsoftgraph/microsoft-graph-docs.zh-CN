---
author: swapnil1993
title: contentType：associateWithHubSites
description: 将内容类型与中心网站列表关联。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1f55baa3c64195f66cb9ef2f9df4db0c63426131
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974171"
---
# <a name="contenttype-associatewithhubsites"></a>contentType：associateWithHubSites

命名空间：microsoft.graph


将内容 [类型中心][contentType] 中的已发布内容类型与中心网站列表关联。

>**注意：** 此功能仅限于拥有许可证SharePoint Syntex租户。
  

## <a name="permissions"></a>权限  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites
```
>**注意：**_siteId_ 表示内容类型中心网站。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|-|-|-|
|hubSiteUrls| 集合 (字符串)  |需要强制执行内容类型的中心网站的规范 URL 列表。 必需。|
|propagateToExistingLists| 布尔 |如果 `true` 为 ，内容类型将强制应用于中心网站中的现有列表;否则，将仅应用于新创建的列表。|

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentTypeId}/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/v1.0/sites/{site-id}"
   ],
   "propagateToExistingLists":false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-associatewithhubsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-associatewithhubsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-associatewithhubsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-associatewithhubsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/contenttype-associatewithhubsites-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---




### <a name="response"></a>响应


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
