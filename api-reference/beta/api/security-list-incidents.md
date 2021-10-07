---
title: 列出事件
description: 获取事件对象及其属性的列表。
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1e0dd929000299770d3e5240905e17890ba2ae7e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220821"
---
# <a name="list-incidents"></a>列出事件
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取事件对象 [及其](../resources/incident.md) 属性的列表。

列表事件操作允许你对事件进行排序，以创建明智的网络安全响应。 它公开在环境保留策略中指定的时间范围内网络中标记的事件集合。 最新事件显示在列表顶部。

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
GET /security/incidents
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持以下 OData 查询参数来帮助自定义响应 `$count` `$filter` ：、、、。 `$skip` `$top`

以下属性支持 `$filter` ： **assignedTo**、 **classification**、 **createdDateTime**、 **determination**、 **lastUpdateDateTime**、 **severity** 和 **status**。

用于 `@odata.nextLink` 分页。

以下是它们的使用示例：

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents?$count=true
GET /security/incidents?$filter={property}+eq+'{property-value}'
GET /security/incidents?$top=10
```

若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [incident](../resources/incident.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_incident"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/incidents
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.incident",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
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
  ]
}
```

