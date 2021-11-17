---
title: 列出 tenantDetailedInformation
description: 获取 tenantDetailedInformation 对象及其属性的列表。
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 77a0d5e5f064a8ab5ed47a21318bae11c5cc599a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028425"
---
# <a name="list-tenantdetailedinformation"></a>列出 tenantDetailedInformation
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [tenantDetailedInformation 对象](../resources/managedtenants-tenantdetailedinformation.md) 及其属性的列表。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenants.Read.All、ManagedTenants.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenantdetailedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenantdetailedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenantdetailedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenantdetailedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-tenantdetailedinformation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantDetailedInformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#tenantDetailedInformation",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "companyName": "Fourth Coffee",
      "defaultDomainName": "fourthcoffee001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "companyName": "Consolidated Messenger",
      "defaultDomainName": "consoldiatedmessenger001.onmicrosoft.com",
      "countryName": "United States",
      "countryCode": "US",
      "city": "Redmond",
      "region": "NA",
      "verticalName": "Software",
      "industryName": "Computer",
      "segmentName": "Service"
    }
  ]
}
```
