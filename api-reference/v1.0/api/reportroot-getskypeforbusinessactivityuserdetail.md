---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: 获取用户执行的 Skype for Business 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ebab2c3919b5126772528b39e7e570ccba3c54fa
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728018"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="7e56e-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7e56e-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="7e56e-104">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7e56e-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="7e56e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="7e56e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e56e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e56e-106">Permissions</span></span>

<span data-ttu-id="7e56e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e56e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e56e-109">Permission type</span></span>                        | <span data-ttu-id="7e56e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e56e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7e56e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e56e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e56e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e56e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7e56e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e56e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e56e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e56e-114">Not supported.</span></span>                           |
| <span data-ttu-id="7e56e-115">应用</span><span class="sxs-lookup"><span data-stu-id="7e56e-115">Application</span></span>                            | <span data-ttu-id="7e56e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e56e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7e56e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e56e-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7e56e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="7e56e-118">Function parameters</span></span>

<span data-ttu-id="7e56e-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7e56e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7e56e-120">参数</span><span class="sxs-lookup"><span data-stu-id="7e56e-120">Parameter</span></span> | <span data-ttu-id="7e56e-121">类型</span><span class="sxs-lookup"><span data-stu-id="7e56e-121">Type</span></span>   | <span data-ttu-id="7e56e-122">说明</span><span class="sxs-lookup"><span data-stu-id="7e56e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7e56e-123">period</span><span class="sxs-lookup"><span data-stu-id="7e56e-123">period</span></span>    | <span data-ttu-id="7e56e-124">string</span><span class="sxs-lookup"><span data-stu-id="7e56e-124">string</span></span> | <span data-ttu-id="7e56e-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e56e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7e56e-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7e56e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7e56e-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e56e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7e56e-128">date</span><span class="sxs-lookup"><span data-stu-id="7e56e-128">date</span></span>      | <span data-ttu-id="7e56e-129">Date</span><span class="sxs-lookup"><span data-stu-id="7e56e-129">Date</span></span>   | <span data-ttu-id="7e56e-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="7e56e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7e56e-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="7e56e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7e56e-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="7e56e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7e56e-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="7e56e-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e56e-134">请求头</span><span class="sxs-lookup"><span data-stu-id="7e56e-134">Request headers</span></span>

| <span data-ttu-id="7e56e-135">名称</span><span class="sxs-lookup"><span data-stu-id="7e56e-135">Name</span></span>          | <span data-ttu-id="7e56e-136">说明</span><span class="sxs-lookup"><span data-stu-id="7e56e-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7e56e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e56e-137">Authorization</span></span> | <span data-ttu-id="7e56e-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e56e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7e56e-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7e56e-140">If-None-Match</span></span> | <span data-ttu-id="7e56e-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7e56e-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7e56e-142">可选。</span><span class="sxs-lookup"><span data-stu-id="7e56e-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7e56e-143">响应</span><span class="sxs-lookup"><span data-stu-id="7e56e-143">Response</span></span>

<span data-ttu-id="7e56e-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7e56e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7e56e-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7e56e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7e56e-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7e56e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7e56e-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7e56e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7e56e-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-148">Report Refresh Date</span></span>
- <span data-ttu-id="7e56e-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="7e56e-149">User Principal Name</span></span>
- <span data-ttu-id="7e56e-150">已删除</span><span class="sxs-lookup"><span data-stu-id="7e56e-150">Is Deleted</span></span>
- <span data-ttu-id="7e56e-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-151">Deleted Date</span></span>
- <span data-ttu-id="7e56e-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-152">Last Activity Date</span></span>
- <span data-ttu-id="7e56e-153">对等会话总数</span><span class="sxs-lookup"><span data-stu-id="7e56e-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="7e56e-154">组织会议总数</span><span class="sxs-lookup"><span data-stu-id="7e56e-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="7e56e-155">参与会议总数</span><span class="sxs-lookup"><span data-stu-id="7e56e-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="7e56e-156">对等会话的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="7e56e-157">组织会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="7e56e-158">参与会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7e56e-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="7e56e-159">对等 IM 次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="7e56e-160">对等音频次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="7e56e-161">对等音频分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="7e56e-162">对等视频次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="7e56e-163">对等视频分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="7e56e-164">对等应用共享次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="7e56e-165">对等文件传输次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="7e56e-166">组织会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="7e56e-167">组织会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="7e56e-168">组织会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="7e56e-169">组织会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="7e56e-170">组织会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="7e56e-171">组织会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="7e56e-172">组织会议 - Microsoft 拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="7e56e-173">组织会议 - Microsoft 拨入分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="7e56e-174">组织会议 - Microsoft 拨出分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="7e56e-175">参与会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="7e56e-176">参与会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="7e56e-177">参与会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="7e56e-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="7e56e-178">参与会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="7e56e-179">参与会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="7e56e-180">参与会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="7e56e-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="7e56e-181">分配的产品</span><span class="sxs-lookup"><span data-stu-id="7e56e-181">Assigned Products</span></span>
- <span data-ttu-id="7e56e-182">报表周期</span><span class="sxs-lookup"><span data-stu-id="7e56e-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7e56e-183">示例</span><span class="sxs-lookup"><span data-stu-id="7e56e-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e56e-184">请求</span><span class="sxs-lookup"><span data-stu-id="7e56e-184">Request</span></span>

<span data-ttu-id="7e56e-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e56e-185">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e56e-186">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7e56e-186">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e56e-187">C#</span><span class="sxs-lookup"><span data-stu-id="7e56e-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e56e-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e56e-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e56e-189">目标-C</span><span class="sxs-lookup"><span data-stu-id="7e56e-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e56e-190">Java</span><span class="sxs-lookup"><span data-stu-id="7e56e-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e56e-191">响应</span><span class="sxs-lookup"><span data-stu-id="7e56e-191">Response</span></span>

<span data-ttu-id="7e56e-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e56e-192">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7e56e-193">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7e56e-193">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
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
