---
title: 更新权限
description: 更新网站上的权限对象。
author: BarrySh
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 709e4431235e43f50d70efcec502a4f677aa1af7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136945"
---
# <a name="update-permission"></a>更新权限
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [网站上](../resources/permission.md) 的权限对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）
|:--------------------------------------|:-------------------------------------
|委派（工作或学校帐户）     | 不支持。
|委派（个人 Microsoft 帐户） | 不支持。
|应用程序                            | Sites.FullControl.All

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 permission 对象的 JSON [表示](../resources/permission.md) 形式。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/permission.md) 代码和 permission 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-permission-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-permission-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"2",
   "@deprecated.GrantedToIdentities": "GrantedToIdentities has been deprecated. Refer to GrantedToIdentitiesV2",
   "roles":[
      "read"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Fabrikam Dashboard App"
         }
      }
   ],
  "grantedToIdentitiesV2":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Fabrikam Dashboard App"
         }
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission"
} -->
