---
title: 列出 auditEvents
description: 获取 auditEvent 对象及其属性的列表。
author: vkumar2015
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a2d32732a071d2c070d9b522939f400058833e2b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338303"
---
# <a name="list-auditevents"></a>列出 auditEvents
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [auditEvent](../resources/managedtenants-auditevent.md) 对象及其属性的列表。

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
GET /managedTenant/auditEvents
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/managedTenants-auditevent.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_auditevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/managedTenant/auditEvents
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.auditEvent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
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
  ]
}
```

