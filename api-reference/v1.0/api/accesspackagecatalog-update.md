---
title: 更新 accessPackageCatalog
description: 更新 accessPackageCatalog 对象的属性。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c870b6c251d1d7539af33116dcc1e56127d7798b
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519612"
---
# <a name="update-accesspackagecatalog"></a>更新 accessPackageCatalog

命名空间：microsoft.graph


更新现有 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象以更改其一个或多个属性，如显示名称或说明。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|displayName|String|访问包目录名称。|
|说明|String|访问包目录的说明。|
|catalogType|accessPackageCatalogType|目录是由用户创建还是由权利管理创建。 可能的值包括 `userManaged`、`serviceDefault`、`serviceManaged`、`unknownFutureValue`。|
|state|accessPackageCatalogState|如果访问 `published` 包可用于管理，则具有 值。 可能的值包括 `unpublished`、`published`、`unknownFutureValue`。|
|isExternallyVisible|Boolean|租户外部的用户是否可以请求此目录中的访问包。|



## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。



## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
Content-Type: application/json

{
  "displayName":"Catalog One"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accesspackagecatalog-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-accesspackagecatalog-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response"
}
-->
```http
HTTP/1.1 204 No Content
Content-Type: application/json

```

