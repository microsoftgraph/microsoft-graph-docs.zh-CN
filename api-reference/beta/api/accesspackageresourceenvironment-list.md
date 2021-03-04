---
title: 列出 accessPackageResourceEnvironments
description: 检索 accessPackageResourceEnvironment 对象的列表。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c8319198ae13894f6f5498bc4c018a26615ce59
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50439488"
---
# <a name="list-accesspackageresourceenvironments"></a>列出 accessPackageResourceEnvironments
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象及其属性的列表。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|Application|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法需要 `$filter` [OData 查询参数](/graph/query-parameters)。 你必须申请 `$filter` **originSystem** 设置为 `eq` () `SharePointOnline` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

