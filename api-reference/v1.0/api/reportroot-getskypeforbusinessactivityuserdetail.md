---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: 获取用户执行的 Skype for Business 活动的详细信息。
localization_priority: Normal
ms.openlocfilehash: 095367ea3d4955010df26deb8528501ed7a26f4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882836"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="05f37-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="05f37-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="05f37-104">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="05f37-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="05f37-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="05f37-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="05f37-106">权限</span><span class="sxs-lookup"><span data-stu-id="05f37-106">Permissions</span></span>

<span data-ttu-id="05f37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05f37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05f37-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05f37-109">Permission type</span></span>                        | <span data-ttu-id="05f37-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05f37-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="05f37-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05f37-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05f37-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05f37-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="05f37-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05f37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05f37-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05f37-114">Not supported.</span></span>                           |
| <span data-ttu-id="05f37-115">应用</span><span class="sxs-lookup"><span data-stu-id="05f37-115">Application</span></span>                            | <span data-ttu-id="05f37-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05f37-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="05f37-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05f37-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="05f37-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="05f37-118">Function parameters</span></span>

<span data-ttu-id="05f37-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="05f37-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="05f37-120">参数</span><span class="sxs-lookup"><span data-stu-id="05f37-120">Parameter</span></span> | <span data-ttu-id="05f37-121">类型</span><span class="sxs-lookup"><span data-stu-id="05f37-121">Type</span></span>   | <span data-ttu-id="05f37-122">说明</span><span class="sxs-lookup"><span data-stu-id="05f37-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="05f37-123">period</span><span class="sxs-lookup"><span data-stu-id="05f37-123">period</span></span>    | <span data-ttu-id="05f37-124">string</span><span class="sxs-lookup"><span data-stu-id="05f37-124">string</span></span> | <span data-ttu-id="05f37-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="05f37-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="05f37-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="05f37-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="05f37-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="05f37-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="05f37-128">date</span><span class="sxs-lookup"><span data-stu-id="05f37-128">date</span></span>      | <span data-ttu-id="05f37-129">Date</span><span class="sxs-lookup"><span data-stu-id="05f37-129">Date</span></span>   | <span data-ttu-id="05f37-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="05f37-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="05f37-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="05f37-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="05f37-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="05f37-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="05f37-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="05f37-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05f37-134">请求头</span><span class="sxs-lookup"><span data-stu-id="05f37-134">Request headers</span></span>

| <span data-ttu-id="05f37-135">名称</span><span class="sxs-lookup"><span data-stu-id="05f37-135">Name</span></span>          | <span data-ttu-id="05f37-136">说明</span><span class="sxs-lookup"><span data-stu-id="05f37-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="05f37-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="05f37-137">Authorization</span></span> | <span data-ttu-id="05f37-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="05f37-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="05f37-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="05f37-140">If-None-Match</span></span> | <span data-ttu-id="05f37-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="05f37-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="05f37-142">可选。</span><span class="sxs-lookup"><span data-stu-id="05f37-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="05f37-143">响应</span><span class="sxs-lookup"><span data-stu-id="05f37-143">Response</span></span>

<span data-ttu-id="05f37-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="05f37-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="05f37-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="05f37-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="05f37-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="05f37-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="05f37-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="05f37-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="05f37-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="05f37-148">Report Refresh Date</span></span>
- <span data-ttu-id="05f37-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="05f37-149">User Principal Name</span></span>
- <span data-ttu-id="05f37-150">已删除</span><span class="sxs-lookup"><span data-stu-id="05f37-150">Is Deleted</span></span>
- <span data-ttu-id="05f37-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="05f37-151">Deleted Date</span></span>
- <span data-ttu-id="05f37-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="05f37-152">Last Activity Date</span></span>
- <span data-ttu-id="05f37-153">对等会话总数</span><span class="sxs-lookup"><span data-stu-id="05f37-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="05f37-154">组织会议总数</span><span class="sxs-lookup"><span data-stu-id="05f37-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="05f37-155">参与会议总数</span><span class="sxs-lookup"><span data-stu-id="05f37-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="05f37-156">对等会话的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="05f37-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="05f37-157">组织会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="05f37-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="05f37-158">参与会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="05f37-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="05f37-159">对等 IM 次数</span><span class="sxs-lookup"><span data-stu-id="05f37-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="05f37-160">对等音频次数</span><span class="sxs-lookup"><span data-stu-id="05f37-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="05f37-161">对等音频分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="05f37-162">对等视频次数</span><span class="sxs-lookup"><span data-stu-id="05f37-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="05f37-163">对等视频分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="05f37-164">对等应用共享次数</span><span class="sxs-lookup"><span data-stu-id="05f37-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="05f37-165">对等文件传输次数</span><span class="sxs-lookup"><span data-stu-id="05f37-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="05f37-166">组织会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="05f37-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="05f37-167">组织会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="05f37-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="05f37-168">组织会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="05f37-169">组织会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="05f37-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="05f37-170">组织会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="05f37-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="05f37-171">组织会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="05f37-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="05f37-172">组织会议 - Microsoft 拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="05f37-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="05f37-173">组织会议 - Microsoft 拨入分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="05f37-174">组织会议 - Microsoft 拨出分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="05f37-175">参与会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="05f37-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="05f37-176">参与会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="05f37-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="05f37-177">参与会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="05f37-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="05f37-178">参与会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="05f37-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="05f37-179">参与会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="05f37-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="05f37-180">参与会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="05f37-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="05f37-181">分配的产品</span><span class="sxs-lookup"><span data-stu-id="05f37-181">Assigned Products</span></span>
- <span data-ttu-id="05f37-182">报表周期</span><span class="sxs-lookup"><span data-stu-id="05f37-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="05f37-183">示例</span><span class="sxs-lookup"><span data-stu-id="05f37-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="05f37-184">请求</span><span class="sxs-lookup"><span data-stu-id="05f37-184">Request</span></span>

<span data-ttu-id="05f37-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05f37-185">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="05f37-186">响应</span><span class="sxs-lookup"><span data-stu-id="05f37-186">Response</span></span>

<span data-ttu-id="05f37-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05f37-187">The following is an example of the response.</span></span>

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

<span data-ttu-id="05f37-188">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="05f37-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
