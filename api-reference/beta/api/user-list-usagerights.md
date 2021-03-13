---
title: 列出用户使用情况Rights
description: 检索用户的 usageRights 对象列表。
author: jeeshnair
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2df51b15de635df52ff4b667c3a9266fafea1511
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761491"
---
# <a name="list-user-usagerights"></a>列出用户使用情况Rights
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索给定用户的 [usageRight](../resources/usageright.md) 对象列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{userId}/usageRights
```

## <a name="optional-query-parameters"></a>可选的查询参数
此 API 支持 $filter [OData 查询参数](/graph/query-parameters)。 支持以下$filter模式：

- $filter = state eq 'value'
- $filter = serviceIdentifier eq 'value'
- $filter = state eq 'value' and serviceIdentifier eq 'value'
- $filter = ( value1、value2") 
- $filter =serviceIdentifier in ('value1'， 'value2') 
- $filter = ( value1、value2") 和 serviceIdentifier 中的 state ( value1"，"value2") 

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|odata.maxpagesize|设置每个结果页的最大大小。 可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [usageRight](../resources/usageright.md) 对象集合。

此外，如果响应中有更多的页面，@odata.nextLink。

## <a name="examples"></a>示例

### <a name="example-1-get-all-usage-rights-for-a-user"></a>示例 1：获取用户的所有使用权限

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/users/64952b80-51fd-4378-9ba5-589a840afb80/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "c2e034cb-3cbc-41be-a496-bfcd031e4cfc",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-user-with-specific-service-identifiers-and-states"></a>示例 2：获取具有特定服务标识符和状态的用户的使用权限

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "value": [
    {
      "id": "505261eb-b4ee-421c-8206-05529ae2c150",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
