---
title: 'callRecord: getPstnCalls'
description: 获取 PSTN 呼叫日志。
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 32e130edfde3384036d0f744b2094811c940aa80
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509978"
---
# <a name="callrecord-getpstncalls"></a>callRecord: getPstnCalls

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以[pstnCallLogRow](../resources/callrecords-pstncalllogrow.md)项集合的形式获取 PSTN 呼叫日志。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序| CallRecords。 PstnCalls|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|要查询的时间范围的开始时间。 UTC （含）。<br/>时间范围基于呼叫开始时间。|
|toDateTime|DateTimeOffset|要查询的时间范围的结束时间。 UTC （含）。|

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="response"></a>响应

如果成功，此函数会在 `200 OK` 响应正文中返回响应代码和[pstnCallLogRow](../resources/callrecords-pstncalllogrow.md)条目集合。
  
如果日期范围中的条目数超过1000个，则正文还包含一个 `@odata.NextLink` URL，用于查询下一页的呼叫条目。 日期范围中的最后一页没有 `@odata.NextLink` 。 有关详细信息，请参阅[在应用中分页 Microsoft Graph 数据](/graph/paging)。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9c4984c7-6c3c-427d-a30c-bd0b2eacee90",
            "callId": "1835317186_112562680@61.221.3.176",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:08.2589935Z",
            "endDateTime": "2019-11-01T00:03:47.2589935Z",
            "duration": 219,
            "charge": 0.00,
            "callType": "user_in",
            "currency": "USD",
            "calleeNumber": "+1234567890",
            "usageCountryCode": "US",
            "tenantCountryCode": "US",
            "connectionCharge": 0.00,
            "callerNumber": "+0123456789",
            "destinationContext": null,
            "destinationName": "United States",
            "conferenceId": null,
            "licenseCapability": "MCOPSTNU",
            "inventoryType": "Subscriber"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>另请参阅

* [Microsoft 团队 PSTN 使用情况报告](https://docs.microsoft.com/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [Microsoft Graph 中的直接路由报告](callrecords-callrecord-getdirectroutingcalls.md)
