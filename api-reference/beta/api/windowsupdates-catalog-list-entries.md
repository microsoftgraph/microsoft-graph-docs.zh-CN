---
title: 列表条目
description: 从目录中获取 catalogEntry 资源列表。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 836dcf23ae3e90b078af9775b7a44fe363bae930
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792069"
---
# <a name="list-entries"></a>列表条目
命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从目录获取 [catalogEntry](../resources/windowsupdates-catalogentry.md) 资源 [的列表](../resources/windowsupdates-catalog.md)。

当前，此操作返回 [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) 或 [qualityUpdateCatalog](../resources/windowsupdates-qualityupdatecatalogentry.md) 类型的条目，继承自 **catalogEntry**。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|WindowsUpdates.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/catalog/entries
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

若要对不是从 **catalogEntry** 继承的属性使用查询参数，请包含属性的完整资源类型。 例如，若要筛选 [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md)**的版本属性**，请使用 `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` catalogEntry 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_catalogentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-catalogentry-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-catalogentry-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-catalogentry-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-catalogentry-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-catalogentry-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.catalogEntry)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
      "id": "c1dec151-c151-c1de-51c1-dec151c1dec1",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "version": "String"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
      "id": "d0c03fbb-43b9-4dff-840b-974ef227384d",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "isExpeditable": true,
      "qualityUpdateClassification": "security"
    }
  ]
}
```

