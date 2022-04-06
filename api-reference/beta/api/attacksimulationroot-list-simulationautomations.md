---
title: 列出 simulationAutomations
description: 获取租户的攻击模拟自动化列表。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 13bdd574c1b783992b27144ded3ab3a31f2da5a7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758310"
---
# <a name="list-simulationautomations"></a>列出 simulationAutomations
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取租户的攻击模拟自动化列表。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | SecurityEvents.Read.All                     |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持`$count`使用 、 、 `$filter``$orderby`、 `$skip`、 和 `$top``$select` [OData](/graph/query-parameters) 查询参数来帮助自定义响应。 可以在 **displayName** 和 `$filter` `$orderby` status 属性上使用 和 **查询** 参数。

如果结果集跨多个页面 `@odata.nextLink` ，响应正文将包含 可用于分页浏览结果集。

以下是它们的使用示例：

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations?$count=true
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulationAutomations?$orderby={property}
GET /security/attackSimulation/simulationAutomations?$skip={skipCount}
GET /security/attackSimulation/simulationAutomations?$top=1
GET /security/attackSimulation/simulationAutomations?$select={property}
```

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [simulationAutomation](../resources/simulationautomation.md) 对象集合。

## <a name="examples"></a>示例

请求示例如下所示。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_simulationautomation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations
```


### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulationAutomation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomation",
      "id": "fbad62b0-b32d-b6ac-9f48-d84bbea08f96",
      "displayName": "Reed Flores",
      "description": "Sample Simulation Automation Description",
      "status": "running",
      "createdDateTime": "2022-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastModifiedDateTime": "2022-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastRunDateTime": "2022-01-01T01:01:01.01Z",
      "nextRunDateTime": "2022-01-01T01:01:01.01Z"
    }
  ]
}
```

