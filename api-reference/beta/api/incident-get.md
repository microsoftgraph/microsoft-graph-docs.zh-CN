---
title: 获取事件
description: 检索事件对象的属性和关系。
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b3bbf34ce02dfaeeee904c2016fc19c39d9ecd3e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220819"
---
# <a name="get-incident"></a>获取事件
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索事件对象的属性 [和](../resources/incident.md) 关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Incidents.Read.All、Incidents.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|Incidents.Read.All、Incidents.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents/{incidentId}
```


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [incident](../resources/incident.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_incident"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/incidents/{incidentId}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.incident"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.incident",
    "id": "2972395",
    "incidentWebUrl": "https://security.microsoft.com/incidents/2972395?tid=12f988bf-16f1-11af-11ab-1d7cd011db47",
    "redirectIncidentId": null,
    "displayName": "Multi-stage incident involving Initial access & Command and control on multiple endpoints reported by multiple sources",
    "createdDateTime": "2021-08-13T08:43:35.5533333Z",
    "lastUpdateDateTime": "2021-09-30T09:35:45.1133333Z",
    "assignedTo": "KaiC@contoso.onmicrosoft.com",
    "classification": "TruePositive",
    "determination": "MultiStagedAttack",
    "status": "Active",
    "severity": "Medium",
    "tags": [
      "Demo"
    ],
    "comments": [
      {
        "comment": "Demo incident",
        "createdBy": "DavidS@contoso.onmicrosoft.com",
        "createdTime": "2021-09-30T12:07:37.2756993Z"
      }
    ]
}
```

