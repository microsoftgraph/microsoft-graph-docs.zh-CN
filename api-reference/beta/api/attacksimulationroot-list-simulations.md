---
title: 列出模拟
description: 获取租户的攻击模拟市场活动列表。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 24c73af15cdffa97007caa367a37a780f3cdbb4f
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758030"
---
# <a name="list-simulations"></a>列出模拟
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取租户的攻击模拟市场活动列表。

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
GET /security/attackSimulation/simulations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持以下 OData 查询参数来帮助自定义响应：`$count``$filter``$skiptoken``$orderby``$top`、、。 `$select`

以下属性支持 `$filter` `$orderby`和 ：**attackTechnique**、**attackType**、**completionDateTime**、**displayName**、**isAutomated**、**launchDateTime****、status**。

用于 `@odata.nextLink` 分页。

以下是它们的使用示例：

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations?$count=true
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulations?$orderby={property}
GET /security/attackSimulation/simulations?$top=1
GET /security/attackSimulation/simulations?$select={property}
```

若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [模拟](../resources/simulation.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_simulation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f1b13829-3829-f1b1-2938-b1f12938b1f1",
      "displayName": "Sample Simulation",
      "description": "Sample Simulation Description",
      "attackType": "social",
      "attackTechnique": "credentialHarvesting",
      "status": "scheduled",
      "createdDateTime": "2021-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "lastModifiedDateTime": "2021-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "launchDateTime": "2021-01-01T02:01:01.01Z",
      "completionDateTime": "2021-01-07T01:01:01.01Z",
      "isAutomated": false,
      "automationId": "f1b13829-3829-f1b1-2938-b1f12938b1ab",
      "payloadDeliveryPlatform": "email"
    }
  ]
}
```

