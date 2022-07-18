---
title: callRecord： getDirectRoutingCalls
description: 获取直接路由呼叫的日志。
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8463274bddbb940a9656f1c9f3237fa97b87b2f0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107724"
---
# <a name="callrecord-getdirectroutingcalls"></a>callRecord： getDirectRoutingCalls

命名空间：microsoft.graph.callRecords

获取作为 [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合的直接路由呼叫的日志。

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
|fromDateTime|DateTimeOffset|要查询的起始时间范围。 UTC（包含两者）。<br/>时间范围基于呼叫开始时间。|
|toDateTime|DateTimeOffset|要查询的结束时间范围。 UTC（包含两者）。|

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合。
  
如果日期范围内包含的条目超过 1000 个，正文中还包含 一个 URL，用于查询下一页 `@odata.NextLink` 的呼叫条目。 日期范围中的最后一页没有 `@odata.NextLink` 。 有关详细信息，请参阅分页[Microsoft Graph应用中的数据](/graph/paging)。

## <a name="example"></a>示例

以下示例显示获取指定日期范围内发生的直接路由呼叫的记录集合。 该响应包括枚举第一个响应中的记录数，以及获取前 `"@odata.count": 1000` `@odata.NextLink` 1000 条之后的记录。 为了可读性，该响应只显示 1 条记录的集合。 假设该日期范围内呼叫超过 1000 个。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/callrecord-getdirectroutingcalls-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/callrecord-getdirectroutingcalls-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/callrecord-getdirectroutingcalls-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/callrecord-getdirectroutingcalls-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/callrecord-getdirectroutingcalls-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/callrecord-getdirectroutingcalls-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
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
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a>另请参阅

* [Microsoft Teams管理中心中的](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing)直接路由Microsoft Teams报告。
* [用于直接路由的运行状况仪表板](/MicrosoftTeams/direct-routing-health-dashboard)Microsoft Teams管理中心。
* [Microsoft Graph 中的 PSTN 呼叫报告](callrecords-callrecord-getpstncalls.md)。
