---
title: contentType：addCopyFromContentTypeHub
description: 将已发布内容类型的副本从内容类型中心添加或同步到目标网站或列表。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: de18d986844057dbf9e592f3b1d33d1fe87ed425
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262181"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType：addCopyFromContentTypeHub
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将已发布内容类型的副本从内容类型中心添加或同步到目标[网站或](../resources/site.md)[列表](../resources/list.md)。

此方法是内容类型发布更改的一部分，可优化已发布内容类型到网站和列表的同步，从而有效地从"推送无处不在"切换到"根据需要拉取"方法。 此方法允许用户将内容类型直接从内容类型中心拉取到站点或列表。 有关详细信息，请参阅 [getCompatibleHubContentTypes](contenttype-getcompatiblehubcontenttypes.md) 和博客文章 [Syntex Product Updates – August 2021](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438)。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
POST /sites/{siteId}/contentTypes/addCopyFromContentTypeHub
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|contentTypeId|String| 要添加到目标网站或列表的内容类型集线器中的内容类型的 ID。|



## <a name="response"></a>响应

如果成功，此操作将在 `200 OK` 响应正文中返回 响应代码和 [contentType](../resources/contenttype.md) `202 Accepted` 对象（如果内容类型是同步添加的）或响应代码（如果内容类型将异步同步）。 该响应还将包含 `Location` 一个标头，其中包含为处理复制/同步而创建的 [richLongRunningOperation](../resources/richLongRunningOperation.md) 的位置。对于异步操作，最多可能需要 70 分钟才能同步或添加内容类型。

## <a name="examples"></a>示例

### <a name="example-1-synchronous-pull"></a>示例 1：同步拉取

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "0x0101"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopyfromcontenttypehub-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopyfromcontenttypehub-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopyfromcontenttypehub-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopyfromcontenttypehub-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/contenttype-addcopyfromcontenttypehub-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.contentType",
    "id": "0x0101",
    "description": "Document content type",
    "group": "Document Content Types",
    "hidden": false,
    "isBuiltIn": true,
    "name": "Document"
}
```
### <a name="example-2-asynchronous-pull"></a>示例 2：异步拉取

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/operations/{operationId}
```
