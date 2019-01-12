---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 614a8cc5f6e52b770d905c439cc9441cce7c6494
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982447"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="62f9c-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="62f9c-104">reportRoot: getTeamsUserActivityCounts</span></span>

> <span data-ttu-id="62f9c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="62f9c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62f9c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="62f9c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62f9c-107">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="62f9c-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="62f9c-108">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="62f9c-108">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="62f9c-109">权限</span><span class="sxs-lookup"><span data-stu-id="62f9c-109">Permissions</span></span>

<span data-ttu-id="62f9c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62f9c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="62f9c-112">Permission type</span></span>                        | <span data-ttu-id="62f9c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62f9c-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62f9c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62f9c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="62f9c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62f9c-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62f9c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62f9c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62f9c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="62f9c-117">Not supported.</span></span>                           |
| <span data-ttu-id="62f9c-118">应用</span><span class="sxs-lookup"><span data-stu-id="62f9c-118">Application</span></span>                            | <span data-ttu-id="62f9c-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62f9c-119">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="62f9c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62f9c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="62f9c-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="62f9c-121">Function parameters</span></span>

<span data-ttu-id="62f9c-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="62f9c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="62f9c-123">参数</span><span class="sxs-lookup"><span data-stu-id="62f9c-123">Parameter</span></span> | <span data-ttu-id="62f9c-124">类型</span><span class="sxs-lookup"><span data-stu-id="62f9c-124">Type</span></span>   | <span data-ttu-id="62f9c-125">说明</span><span class="sxs-lookup"><span data-stu-id="62f9c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62f9c-126">period</span><span class="sxs-lookup"><span data-stu-id="62f9c-126">period</span></span>    | <span data-ttu-id="62f9c-127">string</span><span class="sxs-lookup"><span data-stu-id="62f9c-127">string</span></span> | <span data-ttu-id="62f9c-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="62f9c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62f9c-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="62f9c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62f9c-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="62f9c-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="62f9c-131">必需。</span><span class="sxs-lookup"><span data-stu-id="62f9c-131">Required.</span></span> |

<span data-ttu-id="62f9c-132">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="62f9c-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="62f9c-133">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="62f9c-133">The default output type is text/csv.</span></span> <span data-ttu-id="62f9c-134">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="62f9c-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62f9c-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="62f9c-135">Request headers</span></span>

| <span data-ttu-id="62f9c-136">名称</span><span class="sxs-lookup"><span data-stu-id="62f9c-136">Name</span></span>          | <span data-ttu-id="62f9c-137">说明</span><span class="sxs-lookup"><span data-stu-id="62f9c-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="62f9c-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="62f9c-138">Authorization</span></span> | <span data-ttu-id="62f9c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62f9c-141">响应</span><span class="sxs-lookup"><span data-stu-id="62f9c-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="62f9c-142">CSV</span><span class="sxs-lookup"><span data-stu-id="62f9c-142">CSV</span></span>

<span data-ttu-id="62f9c-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="62f9c-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62f9c-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="62f9c-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62f9c-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="62f9c-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62f9c-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="62f9c-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="62f9c-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="62f9c-147">Report Refresh Date</span></span>
- <span data-ttu-id="62f9c-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="62f9c-148">Report Date</span></span>
- <span data-ttu-id="62f9c-149">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="62f9c-149">Team Chat Messages</span></span>
- <span data-ttu-id="62f9c-150">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="62f9c-150">Private Chat Messages</span></span>
- <span data-ttu-id="62f9c-151">呼叫</span><span class="sxs-lookup"><span data-stu-id="62f9c-151">Calls</span></span>
- <span data-ttu-id="62f9c-152">会议</span><span class="sxs-lookup"><span data-stu-id="62f9c-152">Meetings</span></span>
- <span data-ttu-id="62f9c-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="62f9c-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="62f9c-154">JSON</span><span class="sxs-lookup"><span data-stu-id="62f9c-154">JSON</span></span>

<span data-ttu-id="62f9c-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="62f9c-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62f9c-156">示例</span><span class="sxs-lookup"><span data-stu-id="62f9c-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="62f9c-157">CSV</span><span class="sxs-lookup"><span data-stu-id="62f9c-157">CSV</span></span>

<span data-ttu-id="62f9c-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="62f9c-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="62f9c-159">请求</span><span class="sxs-lookup"><span data-stu-id="62f9c-159">Request</span></span>

<span data-ttu-id="62f9c-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62f9c-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="62f9c-161">响应</span><span class="sxs-lookup"><span data-stu-id="62f9c-161">Response</span></span>

<span data-ttu-id="62f9c-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62f9c-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="62f9c-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="62f9c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="62f9c-164">JSON</span><span class="sxs-lookup"><span data-stu-id="62f9c-164">JSON</span></span>

<span data-ttu-id="62f9c-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="62f9c-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="62f9c-166">请求</span><span class="sxs-lookup"><span data-stu-id="62f9c-166">Request</span></span>

<span data-ttu-id="62f9c-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62f9c-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="62f9c-168">响应</span><span class="sxs-lookup"><span data-stu-id="62f9c-168">Response</span></span>

<span data-ttu-id="62f9c-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62f9c-169">The following is an example of the response.</span></span>

> <span data-ttu-id="62f9c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
