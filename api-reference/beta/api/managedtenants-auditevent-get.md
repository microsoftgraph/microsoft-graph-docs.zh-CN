---
title: 获取 auditEvent
description: 读取 auditEvent 对象的属性和关系。
author: vkumar2015
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9df01732d85fb1a1ed62ab584d7cb705db5f8b96
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393856"
---
# <a name="get-auditevent"></a>获取 auditEvent
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [auditEvent 对象的属性和](../resources/managedtenants-auditevent.md) 关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenant.Read.All、ManagedTenant.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /auditEvent
GET /managedTenant/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [auditEvent](../resources/managedtenants-auditevent.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/auditEvent
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.auditEvent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
      "id": "c3b0d319-9913-bd52-7376-1125f0594129",
      "activityDateTime": "2021-12-21T16:48:23.0330765Z",
      "activityId": "64be6675-3cb8-4b14-95f3-6d5ce9eecd79",
      "initiatedByAppId": "00000003-0000-0000-c000-000000000000",
      "initiatedByUpn": "meganb@contoso.onmicrosoft.com",
      "category": "Baselines",
      "activity": "/managementActionTenantDeploymentStatuses/microsoft.graph.managedTenants.changeDeploymentStatus",
      "httpVerb": "POST",
      "path": "/managementActionTenantDeploymentStatuses/microsoft.graph.managedTenants.changeDeploymentStatus",
      "url": "https://graph.microsoft.com/managementActionTenantDeploymentStatuses/microsoft.graph.managedTenants.changeDeploymentStatus",
      "requestBody": ""
}
```

