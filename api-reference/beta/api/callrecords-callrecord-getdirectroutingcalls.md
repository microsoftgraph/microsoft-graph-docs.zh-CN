---
title: callRecord： getDirectRoutingCalls
description: 获取直接路由呼叫的日志。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5dd389ddba5e3f081b850e2303833b47b832e7d7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872917"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord： getDirectRoutingCalls

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取作为 [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合的直接路由呼叫的日志。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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

|参数|类型|Description|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|要查询的起始时间范围。 UTC（包含两者）。<br/>时间范围基于呼叫开始时间。|
|toDateTime|DateTimeOffset|要查询的结束时间范围。 UTC（包含两者）。|

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回响应代码和 `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合。
  
如果日期范围内有 1000 多个条目，正文还包含一个 URL 以查询下一页 `@odata.NextLink` 的呼叫条目。 日期范围中的最后一页没有 `@odata.NextLink` 。 有关详细信息，请参阅 [在应用中](/graph/paging)分页 Microsoft Graph 数据。

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
            "callerNumber": "+12345678**_",
            "calleeNumber": "+01234567_*_",
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

_ [Microsoft Teams 管理中心](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) 中的 Microsoft Teams 直接路由使用情况报告
* [Microsoft Teams 管理中心中用于直接路由](/MicrosoftTeams/direct-routing-health-dashboard) 的运行状况仪表板
* [Microsoft Graph 中的 PSTN 呼叫报告](callrecords-callrecord-getpstncalls.md)