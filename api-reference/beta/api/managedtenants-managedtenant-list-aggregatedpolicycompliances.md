---
title: 列出 aggregatedPolicyCompliances
description: 获取聚合PolicyCompliance 对象及其属性的列表。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 7ba26a6ea4029184862feffac3e918d83b2b6827
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791544"
---
# <a name="list-aggregatedpolicycompliances"></a>列出 aggregatedPolicyCompliances
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取聚合 [PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [聚合PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-aggregatedpolicycompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-aggregatedpolicycompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-aggregatedpolicycompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-aggregatedpolicycompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-aggregatedpolicycompliance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.aggregatedPolicyCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#aggregatedPolicyCompliances",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyName": "Baseline - Setup Compliance Policy for Windows devices",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 0,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-06-22T17:01:46Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyId": "3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyName": "Windows Level 2 Compliance Policy",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 4,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-04-20T22:27:20Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
