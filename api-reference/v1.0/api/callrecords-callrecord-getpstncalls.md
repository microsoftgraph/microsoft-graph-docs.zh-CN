---
title: callRecord： getPstnCalls
description: 获取 PSTN 呼叫日志。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b5aaea2800e64dea6743c0ae1a9265bdc136da55
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792020"
---
# <a name="callrecord-getpstncalls"></a>callRecord： getPstnCalls

命名空间：microsoft.graph.callRecords

以 [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) 条目集合方式获取 PSTN 呼叫日志。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | CallRecord-PstnCalls.Read.All、CallRecords.Read.All |

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
|fromDateTime|DateTimeOffset|要查询的起始时间范围。 UTC（包含两者）。<br/>时间范围基于呼叫开始时间。|
|toDateTime|DateTimeOffset|要查询的结束时间范围。 UTC（包含两者）。|

> [!IMPORTANT]
> **fromDateTime** 和 **toDateTime** 值不能超过 90 天的日期范围。

## <a name="request-headers"></a>请求头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) 条目集合。
  
如果日期范围内包含的条目超过 1000 个，正文中还包含 一个 URL，用于查询下一页 `@odata.NextLink` 的呼叫条目。 日期范围中的最后一页没有 `@odata.NextLink` 。 有关详细信息，请参阅分页[Microsoft Graph应用中的数据](/graph/paging)。

## <a name="example"></a>示例

以下示例显示获取指定日期范围内发生的 PSTN 呼叫的记录集合。 该响应包括枚举第一个响应中的记录数，以及获取前 `"@odata.count": 1000` `@odata.NextLink` 1000 条之后的记录。 为了可读性，该响应只显示 1 条记录的集合。 假设该日期范围内呼叫超过 1000 个。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
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
            "inventoryType": "Subscriber",
            "operator": "Microsoft",
            "callDurationSource": "microsoft"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>另请参阅

* [Microsoft Teams PSTN 用法报告](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)。
* [Microsoft Graph 中的直接路由报告](callrecords-callrecord-getdirectroutingcalls.md)。
