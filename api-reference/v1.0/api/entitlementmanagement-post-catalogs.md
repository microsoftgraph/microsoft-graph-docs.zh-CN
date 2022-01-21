---
title: 创建 accessPackageCatalog
description: 创建新的 accessPackageCatalog。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3d6d80f048fbaa7765fbf884e28afa5f00796826
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114979"
---
# <a name="create-accesspackagecatalog"></a>创建 accessPackageCatalog

命名空间：microsoft.graph


创建新的 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/catalogs
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 \{token\}。必需。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的 JSON 表示形式。

您可以在创建 **accessPackageCatalog** 时指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|访问显示名称目录的索引。|
|说明|String|访问包目录的说明。|
|state|accessPackageCatalogState|如果访问 `published` 包可用于管理，则具有 值。 可能的值是： `unpublished` 和 `published` 。|
|isExternallyVisible|布尔|租户外部的用户是否可以请求此目录中的访问包。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs
Content-Type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "state": "published",
  "isExternallyVisible": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accesspackagecatalog-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackagecatalog-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{

  "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "userManaged",
  "state": "published",
  "isExternallyVisible": true,
  "createdDateTime": "2021-11-10T01:08:30.9134953Z",
  "modifiedDateTime": "2021-11-10T01:08:30.9134953Z"
}
```

