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
# <a name="callrecord-getdirectroutingcalls"></a><span data-ttu-id="1b036-103">callRecord： getDirectRoutingCalls</span><span class="sxs-lookup"><span data-stu-id="1b036-103">callRecord: getDirectRoutingCalls</span></span>

<span data-ttu-id="1b036-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="1b036-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b036-105">获取作为 [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合的直接路由呼叫的日志。</span><span class="sxs-lookup"><span data-stu-id="1b036-105">Get a log of direct routing calls as a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b036-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b036-106">Permissions</span></span>

<span data-ttu-id="1b036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b036-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b036-109">Permission type</span></span>|<span data-ttu-id="1b036-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b036-110">Permissions (from least to most privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b036-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b036-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b036-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b036-112">Not supported.</span></span> |
| <span data-ttu-id="1b036-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b036-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b036-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b036-114">Not supported.</span></span> |
| <span data-ttu-id="1b036-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b036-115">Application</span></span>                            | <span data-ttu-id="1b036-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b036-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b036-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b036-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a><span data-ttu-id="1b036-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b036-118">Request headers</span></span>

|<span data-ttu-id="1b036-119">名称</span><span class="sxs-lookup"><span data-stu-id="1b036-119">Name</span></span>|<span data-ttu-id="1b036-120">说明</span><span class="sxs-lookup"><span data-stu-id="1b036-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b036-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b036-121">Authorization</span></span>|<span data-ttu-id="1b036-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b036-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="1b036-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="1b036-124">Function parameters</span></span>

<span data-ttu-id="1b036-125">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="1b036-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1b036-126">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="1b036-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1b036-127">参数</span><span class="sxs-lookup"><span data-stu-id="1b036-127">Parameter</span></span>|<span data-ttu-id="1b036-128">类型</span><span class="sxs-lookup"><span data-stu-id="1b036-128">Type</span></span>|<span data-ttu-id="1b036-129">Description</span><span class="sxs-lookup"><span data-stu-id="1b036-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b036-130">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="1b036-130">fromDateTime</span></span>|<span data-ttu-id="1b036-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b036-131">DateTimeOffset</span></span>|<span data-ttu-id="1b036-132">要查询的起始时间范围。</span><span class="sxs-lookup"><span data-stu-id="1b036-132">Start of time range to query.</span></span> <span data-ttu-id="1b036-133">UTC（包含两者）。</span><span class="sxs-lookup"><span data-stu-id="1b036-133">UTC, inclusive.</span></span><br/><span data-ttu-id="1b036-134">时间范围基于呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="1b036-134">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="1b036-135">toDateTime</span><span class="sxs-lookup"><span data-stu-id="1b036-135">toDateTime</span></span>|<span data-ttu-id="1b036-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b036-136">DateTimeOffset</span></span>|<span data-ttu-id="1b036-137">要查询的结束时间范围。</span><span class="sxs-lookup"><span data-stu-id="1b036-137">End of time range to query.</span></span> <span data-ttu-id="1b036-138">UTC（包含两者）。</span><span class="sxs-lookup"><span data-stu-id="1b036-138">UTC, inclusive.</span></span>|

## <a name="response"></a><span data-ttu-id="1b036-139">响应</span><span class="sxs-lookup"><span data-stu-id="1b036-139">Response</span></span>

<span data-ttu-id="1b036-140">如果成功，此函数在响应正文中返回响应代码和 `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) 条目集合。</span><span class="sxs-lookup"><span data-stu-id="1b036-140">If successful, this function returns a `200 OK` response code and a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="1b036-141">如果日期范围内有 1000 多个条目，正文还包含一个 URL 以查询下一页 `@odata.NextLink` 的呼叫条目。</span><span class="sxs-lookup"><span data-stu-id="1b036-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="1b036-142">日期范围中的最后一页没有 `@odata.NextLink` 。</span><span class="sxs-lookup"><span data-stu-id="1b036-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="1b036-143">有关详细信息，请参阅 [在应用中](/graph/paging)分页 Microsoft Graph 数据。</span><span class="sxs-lookup"><span data-stu-id="1b036-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="1b036-144">示例</span><span class="sxs-lookup"><span data-stu-id="1b036-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b036-145">请求</span><span class="sxs-lookup"><span data-stu-id="1b036-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="1b036-146">响应</span><span class="sxs-lookup"><span data-stu-id="1b036-146">Response</span></span>

<span data-ttu-id="1b036-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b036-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1b036-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b036-148">See also</span></span>

<span data-ttu-id="1b036-149">_ [Microsoft Teams 管理中心](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) 中的 Microsoft Teams 直接路由使用情况报告</span><span class="sxs-lookup"><span data-stu-id="1b036-149">_ [Microsoft Teams direct routing usage report](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) in the Microsoft Teams admin center</span></span>
* <span data-ttu-id="1b036-150">[Microsoft Teams 管理中心中用于直接路由](/MicrosoftTeams/direct-routing-health-dashboard) 的运行状况仪表板</span><span class="sxs-lookup"><span data-stu-id="1b036-150">[Health Dashboard for direct routing](/MicrosoftTeams/direct-routing-health-dashboard) in the Microsoft Teams admin center</span></span>
* [<span data-ttu-id="1b036-151">Microsoft Graph 中的 PSTN 呼叫报告</span><span class="sxs-lookup"><span data-stu-id="1b036-151">PSTN call report in Microsoft Graph</span></span>](callrecords-callrecord-getpstncalls.md)