---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8bc7f93f0810423fa3e58fe10a9848342372d35b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639115"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="83ad4-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="83ad4-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ad4-105">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="83ad4-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="83ad4-106">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="83ad4-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="83ad4-107">权限</span><span class="sxs-lookup"><span data-stu-id="83ad4-107">Permissions</span></span>

<span data-ttu-id="83ad4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83ad4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83ad4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83ad4-110">Permission type</span></span>                        | <span data-ttu-id="83ad4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83ad4-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83ad4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83ad4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="83ad4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ad4-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83ad4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83ad4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83ad4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83ad4-115">Not supported.</span></span>                           |
| <span data-ttu-id="83ad4-116">应用</span><span class="sxs-lookup"><span data-stu-id="83ad4-116">Application</span></span>                            | <span data-ttu-id="83ad4-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83ad4-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="83ad4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83ad4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="83ad4-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="83ad4-119">Function parameters</span></span>

<span data-ttu-id="83ad4-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="83ad4-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="83ad4-121">参数</span><span class="sxs-lookup"><span data-stu-id="83ad4-121">Parameter</span></span> | <span data-ttu-id="83ad4-122">类型</span><span class="sxs-lookup"><span data-stu-id="83ad4-122">Type</span></span>   | <span data-ttu-id="83ad4-123">说明</span><span class="sxs-lookup"><span data-stu-id="83ad4-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83ad4-124">period</span><span class="sxs-lookup"><span data-stu-id="83ad4-124">period</span></span>    | <span data-ttu-id="83ad4-125">string</span><span class="sxs-lookup"><span data-stu-id="83ad4-125">string</span></span> | <span data-ttu-id="83ad4-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="83ad4-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83ad4-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="83ad4-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83ad4-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="83ad4-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="83ad4-129">必需。</span><span class="sxs-lookup"><span data-stu-id="83ad4-129">Required.</span></span> |

<span data-ttu-id="83ad4-130">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="83ad4-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="83ad4-131">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="83ad4-131">The default output type is text/csv.</span></span> <span data-ttu-id="83ad4-132">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="83ad4-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83ad4-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="83ad4-133">Request headers</span></span>

| <span data-ttu-id="83ad4-134">名称</span><span class="sxs-lookup"><span data-stu-id="83ad4-134">Name</span></span>          | <span data-ttu-id="83ad4-135">说明</span><span class="sxs-lookup"><span data-stu-id="83ad4-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="83ad4-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="83ad4-136">Authorization</span></span> | <span data-ttu-id="83ad4-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83ad4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="83ad4-139">响应</span><span class="sxs-lookup"><span data-stu-id="83ad4-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="83ad4-140">CSV</span><span class="sxs-lookup"><span data-stu-id="83ad4-140">CSV</span></span>

<span data-ttu-id="83ad4-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="83ad4-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83ad4-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="83ad4-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83ad4-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="83ad4-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83ad4-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="83ad4-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83ad4-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="83ad4-145">Report Refresh Date</span></span>
- <span data-ttu-id="83ad4-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="83ad4-146">Report Date</span></span>
- <span data-ttu-id="83ad4-147">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="83ad4-147">Team Chat Messages</span></span>
- <span data-ttu-id="83ad4-148">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="83ad4-148">Private Chat Messages</span></span>
- <span data-ttu-id="83ad4-149">呼叫</span><span class="sxs-lookup"><span data-stu-id="83ad4-149">Calls</span></span>
- <span data-ttu-id="83ad4-150">会议</span><span class="sxs-lookup"><span data-stu-id="83ad4-150">Meetings</span></span>
- <span data-ttu-id="83ad4-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="83ad4-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="83ad4-152">JSON</span><span class="sxs-lookup"><span data-stu-id="83ad4-152">JSON</span></span>

<span data-ttu-id="83ad4-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="83ad4-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ad4-154">示例</span><span class="sxs-lookup"><span data-stu-id="83ad4-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="83ad4-155">CSV</span><span class="sxs-lookup"><span data-stu-id="83ad4-155">CSV</span></span>

<span data-ttu-id="83ad4-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="83ad4-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="83ad4-157">请求</span><span class="sxs-lookup"><span data-stu-id="83ad4-157">Request</span></span>

<span data-ttu-id="83ad4-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83ad4-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="83ad4-159">响应</span><span class="sxs-lookup"><span data-stu-id="83ad4-159">Response</span></span>

<span data-ttu-id="83ad4-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="83ad4-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="83ad4-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="83ad4-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83ad4-162">语言</span><span class="sxs-lookup"><span data-stu-id="83ad4-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83ad4-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="83ad4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<span data-ttu-id="83ad4-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="83ad4-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="83ad4-165">JSON</span><span class="sxs-lookup"><span data-stu-id="83ad4-165">JSON</span></span>

<span data-ttu-id="83ad4-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="83ad4-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="83ad4-167">请求</span><span class="sxs-lookup"><span data-stu-id="83ad4-167">Request</span></span>

<span data-ttu-id="83ad4-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83ad4-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="83ad4-169">响应</span><span class="sxs-lookup"><span data-stu-id="83ad4-169">Response</span></span>

<span data-ttu-id="83ad4-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83ad4-170">The following is an example of the response.</span></span>

> <span data-ttu-id="83ad4-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83ad4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="83ad4-173">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="83ad4-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83ad4-174">语言</span><span class="sxs-lookup"><span data-stu-id="83ad4-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83ad4-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="83ad4-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
