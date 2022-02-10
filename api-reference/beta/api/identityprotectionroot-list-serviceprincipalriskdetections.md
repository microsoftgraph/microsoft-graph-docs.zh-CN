---
title: 列出 servicePrincipalRiskDetections
description: 检索 servicePrincipalRiskDetection 对象集合的属性。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7f847520356c448b2f001701daa149340c1fae1d
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519970"
---
# <a name="list-serviceprincipalriskdetections"></a>列出 servicePrincipalRiskDetections
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) 对象集合的属性。

>**注意：** 必须具有证书或 P2 Azure AD Premium P1才能使用 servicePrincipalRiskDetection API。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/servicePrincipalRiskDetections
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 和 `$filter` `$select` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-list-risk-detections"></a>示例 1：列出风险检测

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections
```


#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a>示例 2：列出风险检测并筛选结果

#### <a name="request"></a>请求
以下示例演示如何使用 获取`$filter``medium`风险级别为 或风险事件类型为 的服务主体风险检测集合`investigationsThreatIntelligence`。

<!-- {
  "blockType": "request",
  "name": "list_filter_serviceprincipalriskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/servicePrincipalRiskDetections?$filter=riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'
```

#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.servicePrincipalRiskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
    "id": "2856d6e87c5c3a74021ff70291fa68107570c150d8dc145bdea5",
    "requestId": null,
    "correlationId": null,
    "riskEventType": "investigationsThreatIntelligence",
    "riskState": "atRisk",
    "riskLevel": "high",
    "riskDetail": "none",
    "source": "IdentityProtection",
    "detectionTimingType": "offline",
    "activity": "servicePrincipal",
    "tokenIssuerType": "AzureAD",
    "ipAddress": null,
    "location": null,
    "activityDateTime": "2021-10-26T00:00:00Z",
    "detectedDateTime": "2021-10-26T00:00:00Z",
    "lastUpdatedDateTime": "2021-10-26T16:28:17.8202975Z)",
    "servicePrincipalId": "99b8d28b-11ae-4e84-9bef-0e767e286grg",
    "servicePrincipalDisplayName": "Contoso App",
    "appId": "0grb38ac-a572-491d-a9db-b07197643457",
    "keyIds": [
      "9d9fea30-d8e3-481b-b57c-0ef569a989e5"
    ],
    "additionalInfo": "[{\"Key\":\"alertUrl\",\"Value\":null}]"
    }
  ]
}
```
