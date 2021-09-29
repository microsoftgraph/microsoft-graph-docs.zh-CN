---
title: reportRoot： getAttackSimulationSimulationUserCoverage
description: 列出攻击模拟和营销活动中租户用户的模拟覆盖范围。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: c01c89ead4e21c5e456b78102800e48f63cb99e1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996376"
---
# <a name="reportroot-getattacksimulationsimulationusercoverage"></a>reportRoot： getAttackSimulationSimulationUserCoverage
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [攻击模拟](../resources/attacksimulationsimulationusercoverage.md) 和营销活动中获取租户用户的模拟覆盖范围。

此函数 `@odata.nextLink` 支持分页。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Reports.Read.All                            |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用                            | Reports.Read.All                            |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getAttackSimulationSimulationUserCoverage
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [attackSimulationSimulationUserCoverage](../resources/attacksimulationsimulationusercoverage.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationsimulationusercoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationSimulationUserCoverage
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getattacksimulationsimulationusercoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getattacksimulationsimulationusercoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getattacksimulationsimulationusercoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getattacksimulationsimulationusercoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationSimulationUserCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "simulationCount": 2,
      "latestSimulationDateTime": "2021-01-01T01:01:01.01Z",
      "clickCount": 1,
      "compromisedCount": 1,
      "attackSimulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

