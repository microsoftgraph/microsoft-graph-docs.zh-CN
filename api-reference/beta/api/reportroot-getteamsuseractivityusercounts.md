---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e3d1cdb8dc8afbc8b43902eb15ab394467afad8f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265091"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="c6cea-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c6cea-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6cea-105">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="c6cea-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="c6cea-106">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="c6cea-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6cea-107">权限</span><span class="sxs-lookup"><span data-stu-id="c6cea-107">Permissions</span></span>

<span data-ttu-id="c6cea-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6cea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6cea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6cea-110">Permission type</span></span>                        | <span data-ttu-id="c6cea-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6cea-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c6cea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6cea-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6cea-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6cea-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c6cea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6cea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6cea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6cea-115">Not supported.</span></span>                           |
| <span data-ttu-id="c6cea-116">应用</span><span class="sxs-lookup"><span data-stu-id="c6cea-116">Application</span></span>                            | <span data-ttu-id="c6cea-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6cea-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c6cea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6cea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="c6cea-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="c6cea-119">Function parameters</span></span>

<span data-ttu-id="c6cea-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c6cea-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c6cea-121">参数</span><span class="sxs-lookup"><span data-stu-id="c6cea-121">Parameter</span></span> | <span data-ttu-id="c6cea-122">类型</span><span class="sxs-lookup"><span data-stu-id="c6cea-122">Type</span></span>   | <span data-ttu-id="c6cea-123">说明</span><span class="sxs-lookup"><span data-stu-id="c6cea-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c6cea-124">period</span><span class="sxs-lookup"><span data-stu-id="c6cea-124">period</span></span>    | <span data-ttu-id="c6cea-125">string</span><span class="sxs-lookup"><span data-stu-id="c6cea-125">string</span></span> | <span data-ttu-id="c6cea-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c6cea-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c6cea-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c6cea-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c6cea-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c6cea-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c6cea-129">必需。</span><span class="sxs-lookup"><span data-stu-id="c6cea-129">Required.</span></span> |

<span data-ttu-id="c6cea-130">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c6cea-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c6cea-131">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="c6cea-131">The default output type is text/csv.</span></span> <span data-ttu-id="c6cea-132">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="c6cea-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6cea-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6cea-133">Request headers</span></span>

| <span data-ttu-id="c6cea-134">名称</span><span class="sxs-lookup"><span data-stu-id="c6cea-134">Name</span></span>          | <span data-ttu-id="c6cea-135">说明</span><span class="sxs-lookup"><span data-stu-id="c6cea-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c6cea-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6cea-136">Authorization</span></span> | <span data-ttu-id="c6cea-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6cea-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c6cea-139">响应</span><span class="sxs-lookup"><span data-stu-id="c6cea-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c6cea-140">CSV</span><span class="sxs-lookup"><span data-stu-id="c6cea-140">CSV</span></span>

<span data-ttu-id="c6cea-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c6cea-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c6cea-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c6cea-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c6cea-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="c6cea-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c6cea-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="c6cea-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c6cea-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c6cea-145">Report Refresh Date</span></span>
- <span data-ttu-id="c6cea-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="c6cea-146">Report Date</span></span>
- <span data-ttu-id="c6cea-147">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="c6cea-147">Team Chat Messages</span></span>
- <span data-ttu-id="c6cea-148">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="c6cea-148">Private Chat Messages</span></span>
- <span data-ttu-id="c6cea-149">呼叫</span><span class="sxs-lookup"><span data-stu-id="c6cea-149">Calls</span></span>
- <span data-ttu-id="c6cea-150">会议</span><span class="sxs-lookup"><span data-stu-id="c6cea-150">Meetings</span></span>
- <span data-ttu-id="c6cea-151">其他操作</span><span class="sxs-lookup"><span data-stu-id="c6cea-151">Other Actions</span></span>
- <span data-ttu-id="c6cea-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="c6cea-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c6cea-153">JSON</span><span class="sxs-lookup"><span data-stu-id="c6cea-153">JSON</span></span>

<span data-ttu-id="c6cea-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="c6cea-154">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6cea-155">示例</span><span class="sxs-lookup"><span data-stu-id="c6cea-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c6cea-156">CSV</span><span class="sxs-lookup"><span data-stu-id="c6cea-156">CSV</span></span>

<span data-ttu-id="c6cea-157">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="c6cea-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c6cea-158">请求</span><span class="sxs-lookup"><span data-stu-id="c6cea-158">Request</span></span>

<span data-ttu-id="c6cea-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6cea-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c6cea-160">响应</span><span class="sxs-lookup"><span data-stu-id="c6cea-160">Response</span></span>

<span data-ttu-id="c6cea-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c6cea-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6cea-162">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c6cea-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6cea-163">C#</span><span class="sxs-lookup"><span data-stu-id="c6cea-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6cea-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6cea-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6cea-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="c6cea-165">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c6cea-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c6cea-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="c6cea-167">JSON</span><span class="sxs-lookup"><span data-stu-id="c6cea-167">JSON</span></span>

<span data-ttu-id="c6cea-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="c6cea-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c6cea-169">请求</span><span class="sxs-lookup"><span data-stu-id="c6cea-169">Request</span></span>

<span data-ttu-id="c6cea-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6cea-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c6cea-171">响应</span><span class="sxs-lookup"><span data-stu-id="c6cea-171">Response</span></span>

<span data-ttu-id="c6cea-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c6cea-172">The following is an example of the response.</span></span>

> <span data-ttu-id="c6cea-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c6cea-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6cea-175">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c6cea-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6cea-176">C#</span><span class="sxs-lookup"><span data-stu-id="c6cea-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6cea-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6cea-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c6cea-178">目标-C</span><span class="sxs-lookup"><span data-stu-id="c6cea-178">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
