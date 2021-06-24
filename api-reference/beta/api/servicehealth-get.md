---
title: 获取 serviceHealth
description: 检索 serviceHealth 对象的属性和关系。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: f36a4f1787415956c486d2ed74a3ab0acb327c88
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107816"
---
# <a name="get-servicehealth"></a>获取 serviceHealth
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [serviceHealth 对象的属性和](../resources/servicehealth.md) 关系。

此操作为租户提供指定服务的运行状况信息。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ServiceHealth.Read.All|
|委派（个人 Microsoft 帐户）|ServiceHealth.Read.All|
|应用程序|ServiceHealth.Read.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /admin/serviceAnnouncement/healthOverviews/{ServiceName}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [serviceHealth](../resources/servicehealth.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-the-properties-of-a-servicehealth-object"></a>示例 1：获取 serviceHealth 对象的属性

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews/$entity",
    "service": "Microsoft 365 suite",
    "status": "RestoringService",
    "id": "OSDPPlatform"
}
```

### <a name="example-2-include-navigation-property-issues"></a>示例 2：包含导航属性问题

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite?$expand=issues
```

#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())/$entity",
  "service": "Microsoft 365 suite",
  "status": "ServiceOperational",
  "id": "OSDPPlatform",
  "issues": [
        {
          "startDateTime": "2020-11-04T00:00:00Z",
          "endDateTime": "2020-11-20T17:00:00Z",
          "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
          "title": "Intermittently unable to access some Microsoft 365 services",
          "id": "MO226574",
          "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
          "classification": "Advisory",
          "origin": "Microsoft",
          "status": "ServiceRestored",
          "service": "Exchange Online",
          "feature": "Tenant Administration (Provisioning, Remote PowerShell)",
          "featureGroup": "Management and Provisioning",
          "isResolved": true,
          "details": [],
          "posts": [
              {
                "createdDateTime": "2020-11-12T07:07:38.97Z",
                "postType": "Regular",
                "description": {
                    "contentType": "Text",
                    "content": "Users may have been intermittently unable to access some Microsoft 365 services. We'll provide an update within 30 minutes."
                  }
              }
          ]
        }
    ]
}
```