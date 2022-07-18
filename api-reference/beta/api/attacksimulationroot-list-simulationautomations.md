---
title: 列出 simulationAutomations
description: 获取租户的攻击模拟自动化列表。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 76e81e291d8975ed63ab02ed9a01a20a15cd6627
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203606"
---
# <a name="list-simulationautomations"></a>列出 simulationAutomations
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取租户的攻击模拟自动化列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | SecurityEvents.Read.All                     |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| Application                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$count`[OData](/graph/query-parameters) `$filter``$skip``$orderby`查询参数，`$top``$select`以帮助自定义响应。 可以在 **displayName** 和 **状态** 属性上使用`$filter`和`$orderby`查询参数。

如果结果集跨多个页面，则响应正文包含一个 `@odata.nextLink` 可用于对结果集进行分页的响应正文。

下面是使用它们的示例：

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

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [simulationAutomation](../resources/simulationautomation.md) 对象集合。

## <a name="examples"></a>示例

请求示例如下所示。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_simulationautomation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-simulationautomation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-simulationautomation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-simulationautomation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-simulationautomation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-simulationautomation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-simulationautomation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

