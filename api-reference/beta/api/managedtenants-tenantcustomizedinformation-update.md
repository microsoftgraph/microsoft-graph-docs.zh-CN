---
title: 更新 tenantCustomizedInformation
description: 更新 tenantCustomizedInformation 对象的属性。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 3f43e7e3f543c0a74b27a3594f573d4fe3cc68c6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441799"
---
# <a name="update-tenantcustomizedinformation"></a>更新 tenantCustomizedInformation
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [tenantCustomizedInformation 对象](../resources/managedtenants-tenantcustomizedinformation.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenants.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象的 JSON 表示形式。

下表显示更新 [tenantCustomizedInformation 时所需的属性](../resources/managedtenants-tenantcustomizedinformation.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|托管Azure Active Directory租户的租户标识符。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。|
|contacts|[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) 集合|与托管租户关联的联系人集合。|
|website|String|托管租户的网站。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenantcustomizedinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
Content-Type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenantcustomizedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenantcustomizedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenantcustomizedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenantcustomizedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "website": "https://www.fourthcoffee.com",
  "contacts": [
    {
      "name": "Sally",
      "email": "sally@fourthcoffee.com",
      "phone": "5558009731"
    },
    {
      "name": "Hector",
      "email": "hector@fourthcoffee.com",
      "phone": "5558009732"
    }
  ]
}
```
