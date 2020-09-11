---
title: 'callRecord: getPstnCalls'
description: 获取 PSTN 呼叫日志。
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9d3c6d7f8ffe207324ca36929b65201daad866d5
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439848"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="31b44-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="31b44-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="31b44-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="31b44-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b44-105">以 [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) 项集合的形式获取 PSTN 呼叫日志。</span><span class="sxs-lookup"><span data-stu-id="31b44-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="31b44-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="31b44-106">Permissions</span></span>

<span data-ttu-id="31b44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31b44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31b44-109">Permission type</span></span>|<span data-ttu-id="31b44-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31b44-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31b44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31b44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31b44-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="31b44-112">Not supported.</span></span> |
| <span data-ttu-id="31b44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31b44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31b44-114">Not supported.</span></span> |
| <span data-ttu-id="31b44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31b44-115">Application</span></span>                            | <span data-ttu-id="31b44-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b44-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31b44-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31b44-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="31b44-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="31b44-118">Function parameters</span></span>

<span data-ttu-id="31b44-119">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="31b44-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="31b44-120">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="31b44-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="31b44-121">参数</span><span class="sxs-lookup"><span data-stu-id="31b44-121">Parameter</span></span>|<span data-ttu-id="31b44-122">类型</span><span class="sxs-lookup"><span data-stu-id="31b44-122">Type</span></span>|<span data-ttu-id="31b44-123">Description</span><span class="sxs-lookup"><span data-stu-id="31b44-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31b44-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="31b44-124">fromDateTime</span></span>|<span data-ttu-id="31b44-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31b44-125">DateTimeOffset</span></span>|<span data-ttu-id="31b44-126">要查询的时间范围的开始时间。</span><span class="sxs-lookup"><span data-stu-id="31b44-126">Start of time range to query.</span></span> <span data-ttu-id="31b44-127">UTC （含）。</span><span class="sxs-lookup"><span data-stu-id="31b44-127">UTC, inclusive.</span></span><br/><span data-ttu-id="31b44-128">时间范围基于呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="31b44-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="31b44-129">toDateTime</span><span class="sxs-lookup"><span data-stu-id="31b44-129">toDateTime</span></span>|<span data-ttu-id="31b44-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31b44-130">DateTimeOffset</span></span>|<span data-ttu-id="31b44-131">要查询的时间范围的结束时间。</span><span class="sxs-lookup"><span data-stu-id="31b44-131">End of time range to query.</span></span> <span data-ttu-id="31b44-132">UTC （含）。</span><span class="sxs-lookup"><span data-stu-id="31b44-132">UTC, inclusive.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="31b44-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="31b44-133">Request headers</span></span>

|<span data-ttu-id="31b44-134">名称</span><span class="sxs-lookup"><span data-stu-id="31b44-134">Name</span></span>|<span data-ttu-id="31b44-135">说明</span><span class="sxs-lookup"><span data-stu-id="31b44-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31b44-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="31b44-136">Authorization</span></span>|<span data-ttu-id="31b44-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31b44-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="31b44-139">响应</span><span class="sxs-lookup"><span data-stu-id="31b44-139">Response</span></span>

<span data-ttu-id="31b44-140">如果成功，此函数会在 `200 OK` 响应正文中返回响应代码和 [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) 条目集合。</span><span class="sxs-lookup"><span data-stu-id="31b44-140">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="31b44-141">如果日期范围中的条目数超过1000个，则正文还包含一个 `@odata.NextLink` URL，用于查询下一页的呼叫条目。</span><span class="sxs-lookup"><span data-stu-id="31b44-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="31b44-142">日期范围中的最后一页没有 `@odata.NextLink` 。</span><span class="sxs-lookup"><span data-stu-id="31b44-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="31b44-143">有关详细信息，请参阅 [在应用中分页 Microsoft Graph 数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="31b44-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="31b44-144">示例</span><span class="sxs-lookup"><span data-stu-id="31b44-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31b44-145">请求</span><span class="sxs-lookup"><span data-stu-id="31b44-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="31b44-146">响应</span><span class="sxs-lookup"><span data-stu-id="31b44-146">Response</span></span>

<span data-ttu-id="31b44-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31b44-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="31b44-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31b44-148">See also</span></span>

* [<span data-ttu-id="31b44-149">Microsoft 团队 PSTN 使用情况报告</span><span class="sxs-lookup"><span data-stu-id="31b44-149">Microsoft Teams PSTN usage report</span></span>](https://docs.microsoft.com/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="31b44-150">Microsoft Graph 中的直接路由报告</span><span class="sxs-lookup"><span data-stu-id="31b44-150">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
