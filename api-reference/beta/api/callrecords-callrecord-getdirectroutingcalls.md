---
title: 'callRecord: getDirectRoutingCalls'
description: 获取直接路由呼叫的日志记录。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a99b776eda23bd1ebaef63bc3f190cb66bd794a7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601109"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord: getDirectRoutingCalls

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将直接路由呼叫的日志作为 [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目的集合获取。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | CallRecords.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="function-parameters"></a>函数参数

在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|要查询的时间范围的开始时间。 UTC （含）。<br/>时间范围基于呼叫开始时间。|
|toDateTime|DateTimeOffset|要查询的时间范围的结束时间。 UTC （含）。|

## <a name="response"></a>响应

如果成功，此函数会在 `200 OK` 响应正文中返回响应代码和 [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合。
  
如果日期范围中的条目数超过1000个，则正文还包含一个 `@odata.NextLink` URL，用于查询下一页的呼叫条目。 日期范围中的最后一页没有 `@odata.NextLink` 。 有关详细信息，请参阅 [在应用中分页 Microsoft Graph 数据](/graph/paging)。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9e8bba57-dc14-533a-a7dd-f0da6575eed1",
            "correlationId": "c98e1515-a937-4b81-b8a8-3992afde64e0",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:25.105Z",
            "inviteDateTime": "2019-11-01T00:00:21.949Z",
            "failureDateTime": "0001-01-01T00:00:00Z",
            "endDateTime": "2019-11-01T00:00:30.105Z",
            "duration": 5,
            "callType": "ByotIn",
            "successfulCall": true,
            "callerNumber": "+12345678***",
            "calleeNumber": "+01234567***",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>另请参阅

* Microsoft 团队管理中心中的[Microsoft 团队直接路由使用情况报告](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing)
* Microsoft 团队管理中心中[用于直接路由的运行状况仪表板](/MicrosoftTeams/direct-routing-health-dashboard)
* [Microsoft Graph 中的 PSTN 呼叫报告](callrecords-callrecord-getpstncalls.md)