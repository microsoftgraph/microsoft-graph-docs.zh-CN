---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e221814d53c98d865a40a6c9e1d5d1917623f8d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358780"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="8ec0f-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="8ec0f-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec0f-105">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="8ec0f-106">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ec0f-107">权限</span><span class="sxs-lookup"><span data-stu-id="8ec0f-107">Permissions</span></span>

<span data-ttu-id="8ec0f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ec0f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ec0f-110">Permission type</span></span>                        | <span data-ttu-id="8ec0f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ec0f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8ec0f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ec0f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ec0f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ec0f-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8ec0f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ec0f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec0f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-115">Not supported.</span></span>                           |
| <span data-ttu-id="8ec0f-116">应用</span><span class="sxs-lookup"><span data-stu-id="8ec0f-116">Application</span></span>                            | <span data-ttu-id="8ec0f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ec0f-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8ec0f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ec0f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="8ec0f-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="8ec0f-119">Function parameters</span></span>

<span data-ttu-id="8ec0f-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8ec0f-121">参数</span><span class="sxs-lookup"><span data-stu-id="8ec0f-121">Parameter</span></span> | <span data-ttu-id="8ec0f-122">类型</span><span class="sxs-lookup"><span data-stu-id="8ec0f-122">Type</span></span>   | <span data-ttu-id="8ec0f-123">说明</span><span class="sxs-lookup"><span data-stu-id="8ec0f-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8ec0f-124">period</span><span class="sxs-lookup"><span data-stu-id="8ec0f-124">period</span></span>    | <span data-ttu-id="8ec0f-125">string</span><span class="sxs-lookup"><span data-stu-id="8ec0f-125">string</span></span> | <span data-ttu-id="8ec0f-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8ec0f-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8ec0f-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8ec0f-129">必需。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-129">Required.</span></span> |

<span data-ttu-id="8ec0f-130">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8ec0f-131">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-131">The default output type is text/csv.</span></span> <span data-ttu-id="8ec0f-132">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ec0f-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ec0f-133">Request headers</span></span>

| <span data-ttu-id="8ec0f-134">名称</span><span class="sxs-lookup"><span data-stu-id="8ec0f-134">Name</span></span>          | <span data-ttu-id="8ec0f-135">说明</span><span class="sxs-lookup"><span data-stu-id="8ec0f-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8ec0f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ec0f-136">Authorization</span></span> | <span data-ttu-id="8ec0f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8ec0f-139">响应</span><span class="sxs-lookup"><span data-stu-id="8ec0f-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8ec0f-140">CSV</span><span class="sxs-lookup"><span data-stu-id="8ec0f-140">CSV</span></span>

<span data-ttu-id="8ec0f-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8ec0f-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8ec0f-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8ec0f-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8ec0f-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8ec0f-145">Report Refresh Date</span></span>
- <span data-ttu-id="8ec0f-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="8ec0f-146">Report Date</span></span>
- <span data-ttu-id="8ec0f-147">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="8ec0f-147">Team Chat Messages</span></span>
- <span data-ttu-id="8ec0f-148">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="8ec0f-148">Private Chat Messages</span></span>
- <span data-ttu-id="8ec0f-149">呼叫</span><span class="sxs-lookup"><span data-stu-id="8ec0f-149">Calls</span></span>
- <span data-ttu-id="8ec0f-150">会议</span><span class="sxs-lookup"><span data-stu-id="8ec0f-150">Meetings</span></span>
- <span data-ttu-id="8ec0f-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="8ec0f-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8ec0f-152">JSON</span><span class="sxs-lookup"><span data-stu-id="8ec0f-152">JSON</span></span>

<span data-ttu-id="8ec0f-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec0f-154">示例</span><span class="sxs-lookup"><span data-stu-id="8ec0f-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8ec0f-155">CSV</span><span class="sxs-lookup"><span data-stu-id="8ec0f-155">CSV</span></span>

<span data-ttu-id="8ec0f-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8ec0f-157">请求</span><span class="sxs-lookup"><span data-stu-id="8ec0f-157">Request</span></span>

<span data-ttu-id="8ec0f-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ec0f-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8ec0f-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ec0f-160">C#</span><span class="sxs-lookup"><span data-stu-id="8ec0f-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ec0f-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ec0f-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ec0f-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="8ec0f-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ec0f-163">Java</span><span class="sxs-lookup"><span data-stu-id="8ec0f-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ec0f-164">响应</span><span class="sxs-lookup"><span data-stu-id="8ec0f-164">Response</span></span>

<span data-ttu-id="8ec0f-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="8ec0f-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8ec0f-167">JSON</span><span class="sxs-lookup"><span data-stu-id="8ec0f-167">JSON</span></span>

<span data-ttu-id="8ec0f-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8ec0f-169">请求</span><span class="sxs-lookup"><span data-stu-id="8ec0f-169">Request</span></span>

<span data-ttu-id="8ec0f-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ec0f-171">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8ec0f-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ec0f-172">C#</span><span class="sxs-lookup"><span data-stu-id="8ec0f-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ec0f-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ec0f-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ec0f-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="8ec0f-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ec0f-175">Java</span><span class="sxs-lookup"><span data-stu-id="8ec0f-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8ec0f-176">响应</span><span class="sxs-lookup"><span data-stu-id="8ec0f-176">Response</span></span>

<span data-ttu-id="8ec0f-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-177">The following is an example of the response.</span></span>

> <span data-ttu-id="8ec0f-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8ec0f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
