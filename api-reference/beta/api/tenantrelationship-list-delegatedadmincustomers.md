---
title: 列出 delegatedAdminCustomers
description: 获取 delegatedAdminCustomer 对象及其属性的列表。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 8d3e20b6f46ddf548f706c93680ac7d6b5b3b6ed
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704455"
---
# <a name="list-delegatedadmincustomers"></a>列出 delegatedAdminCustomers
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [delegatedAdminCustomer](../resources/delegatedadmincustomer.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| DelegatedAdminRelationship.Read.All、DelegatedAdminRelationship.ReadWrite.All |
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminCustomers
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select`[OData](/graph/query-parameters) `$filter``$orderBy``$top`查询参数，`$count``$skipToken`以帮助自定义响应。  

`$top` 最多支持 300 个对象。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [delegatedAdminCustomer](../resources/delegatedadmincustomer.md) 对象集合。

每个 **delegatedAdminCustomer** 对象都包含 **一个 @odata.etag** 属性（根据 RFC2616）。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_delegatedadmincustomer"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminCustomers
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminCustomer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminCustomers",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIxODAwMTMzZi0wMDAwLTAyMDAtMDAwMC02MTNjMGFhZTAwMDAiJw==\"",
      "id": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "tenantId": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "displayName": "Contoso Inc"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIwMDAwMTEwMS0wMDAwLTAyMDAtMDAwMC02MDI1OTQyMjAwMDAiJw==\"",
      "id": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "tenantId": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "displayName": "Contoso subsidiary Inc"
    }
  ]
}
```

