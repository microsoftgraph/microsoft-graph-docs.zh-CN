---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: 获取用户执行的 Skype for Business 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e372af92c2306872ad564260c1d6c0414c544cba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336535"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="516d8-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="516d8-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516d8-104">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="516d8-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="516d8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="516d8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="516d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="516d8-106">Permissions</span></span>

<span data-ttu-id="516d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="516d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="516d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="516d8-109">Permission type</span></span>                        | <span data-ttu-id="516d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="516d8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="516d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="516d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="516d8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="516d8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="516d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="516d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="516d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="516d8-114">Not supported.</span></span>                           |
| <span data-ttu-id="516d8-115">应用</span><span class="sxs-lookup"><span data-stu-id="516d8-115">Application</span></span>                            | <span data-ttu-id="516d8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="516d8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="516d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="516d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="516d8-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="516d8-118">Function parameters</span></span>

<span data-ttu-id="516d8-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="516d8-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="516d8-120">参数</span><span class="sxs-lookup"><span data-stu-id="516d8-120">Parameter</span></span> | <span data-ttu-id="516d8-121">类型</span><span class="sxs-lookup"><span data-stu-id="516d8-121">Type</span></span>   | <span data-ttu-id="516d8-122">说明</span><span class="sxs-lookup"><span data-stu-id="516d8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="516d8-123">period</span><span class="sxs-lookup"><span data-stu-id="516d8-123">period</span></span>    | <span data-ttu-id="516d8-124">string</span><span class="sxs-lookup"><span data-stu-id="516d8-124">string</span></span> | <span data-ttu-id="516d8-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="516d8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="516d8-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="516d8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="516d8-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="516d8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="516d8-128">date</span><span class="sxs-lookup"><span data-stu-id="516d8-128">date</span></span>      | <span data-ttu-id="516d8-129">Date</span><span class="sxs-lookup"><span data-stu-id="516d8-129">Date</span></span>   | <span data-ttu-id="516d8-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="516d8-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="516d8-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="516d8-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="516d8-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="516d8-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="516d8-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="516d8-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="516d8-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="516d8-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="516d8-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="516d8-135">The default output type is text/csv.</span></span> <span data-ttu-id="516d8-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="516d8-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="516d8-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="516d8-137">Request headers</span></span>

| <span data-ttu-id="516d8-138">名称</span><span class="sxs-lookup"><span data-stu-id="516d8-138">Name</span></span>          | <span data-ttu-id="516d8-139">说明</span><span class="sxs-lookup"><span data-stu-id="516d8-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="516d8-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="516d8-140">Authorization</span></span> | <span data-ttu-id="516d8-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="516d8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="516d8-143">响应</span><span class="sxs-lookup"><span data-stu-id="516d8-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="516d8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="516d8-144">CSV</span></span>

<span data-ttu-id="516d8-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="516d8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="516d8-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="516d8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="516d8-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="516d8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="516d8-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="516d8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="516d8-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="516d8-149">Report Refresh Date</span></span>
- <span data-ttu-id="516d8-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="516d8-150">User Principal Name</span></span>
- <span data-ttu-id="516d8-151">已删除</span><span class="sxs-lookup"><span data-stu-id="516d8-151">Is Deleted</span></span>
- <span data-ttu-id="516d8-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="516d8-152">Deleted Date</span></span>
- <span data-ttu-id="516d8-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="516d8-153">Last Activity Date</span></span>
- <span data-ttu-id="516d8-154">对等会话总数</span><span class="sxs-lookup"><span data-stu-id="516d8-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="516d8-155">组织会议总数</span><span class="sxs-lookup"><span data-stu-id="516d8-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="516d8-156">参与会议总数</span><span class="sxs-lookup"><span data-stu-id="516d8-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="516d8-157">对等会话的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="516d8-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="516d8-158">组织会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="516d8-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="516d8-159">参与会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="516d8-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="516d8-160">对等 IM 次数</span><span class="sxs-lookup"><span data-stu-id="516d8-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="516d8-161">对等音频次数</span><span class="sxs-lookup"><span data-stu-id="516d8-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="516d8-162">对等音频分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="516d8-163">对等视频次数</span><span class="sxs-lookup"><span data-stu-id="516d8-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="516d8-164">对等视频分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="516d8-165">对等应用共享次数</span><span class="sxs-lookup"><span data-stu-id="516d8-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="516d8-166">对等文件传输次数</span><span class="sxs-lookup"><span data-stu-id="516d8-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="516d8-167">组织会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="516d8-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="516d8-168">组织会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="516d8-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="516d8-169">组织会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="516d8-170">组织会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="516d8-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="516d8-171">组织会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="516d8-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="516d8-172">组织会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="516d8-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="516d8-173">组织会议 - Microsoft 拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="516d8-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="516d8-174">组织会议 - Microsoft 拨入分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="516d8-175">组织会议 - Microsoft 拨出分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="516d8-176">参与会议的会议即时消息计数</span><span class="sxs-lookup"><span data-stu-id="516d8-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="516d8-177">参与会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="516d8-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="516d8-178">参与会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="516d8-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="516d8-179">参与会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="516d8-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="516d8-180">参与会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="516d8-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="516d8-181">参与会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="516d8-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="516d8-182">分配的产品</span><span class="sxs-lookup"><span data-stu-id="516d8-182">Assigned Products</span></span>
- <span data-ttu-id="516d8-183">报表周期</span><span class="sxs-lookup"><span data-stu-id="516d8-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="516d8-184">JSON</span><span class="sxs-lookup"><span data-stu-id="516d8-184">JSON</span></span>

<span data-ttu-id="516d8-185">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="516d8-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="516d8-186">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="516d8-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="516d8-187">示例</span><span class="sxs-lookup"><span data-stu-id="516d8-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="516d8-188">CSV</span><span class="sxs-lookup"><span data-stu-id="516d8-188">CSV</span></span>

<span data-ttu-id="516d8-189">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="516d8-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="516d8-190">请求</span><span class="sxs-lookup"><span data-stu-id="516d8-190">Request</span></span>

<span data-ttu-id="516d8-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516d8-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="516d8-192">响应</span><span class="sxs-lookup"><span data-stu-id="516d8-192">Response</span></span>

<span data-ttu-id="516d8-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="516d8-193">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="516d8-194">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="516d8-194">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Participated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="516d8-195">JSON</span><span class="sxs-lookup"><span data-stu-id="516d8-195">JSON</span></span>

<span data-ttu-id="516d8-196">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="516d8-196">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="516d8-197">请求</span><span class="sxs-lookup"><span data-stu-id="516d8-197">Request</span></span>

<span data-ttu-id="516d8-198">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="516d8-198">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="516d8-199">响应</span><span class="sxs-lookup"><span data-stu-id="516d8-199">Response</span></span>

<span data-ttu-id="516d8-200">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="516d8-200">The following is an example of the response.</span></span>

> <span data-ttu-id="516d8-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="516d8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserDetail)", 
  "value": [
    {
      "totalPeerToPeerSessionCount": 12, 
      "totalOrganizedConferenceCount": 0, 
      "totalParticipatedConferenceCount": 1, 
      "peerToPeerLastActivityDate": "2017-09-01", 
      "organizedConferenceLastActivityDate": null, 
      "participatedConferenceLastActivityDate": "2017-08-31", 
      "peerToPeerIMCount": 12, 
      "peerToPeerAudioCount": 0, 
      "peerToPeerAudioMinutes": 0, 
      "peerToPeerVideoCount": 0, 
      "peerToPeerVideoMinutes": 0, 
      "peerToPeerAppSharingCount": 0, 
      "peerToPeerFileTransferCount": 0, 
      "organizedConferenceIMCount": 0, 
      "organizedConferenceAudioVideoCount": 0, 
      "organizedConferenceAudioVideoMinutes": 0, 
      "organizedConferenceAppSharingCount": 0, 
      "organizedConferenceWebCount": 0, 
      "organizedConferenceDialInOut3rdPartyCount": 0, 
      "organizedConferenceCloudDialInOutMicrosoftCount": 0, 
      "organizedConferenceCloudDialInMicrosoftMinutes": 0, 
      "organizedConferenceCloudDialOutMicrosoftMinutes": 0, 
      "participatedConferenceIMCount": 0, 
      "participatedConferenceAudioVideoCount": 1, 
      "participatedConferenceAudioVideoMinutes": 69, 
      "participatedConferenceAppSharingCount": 0, 
      "participatedConferenceWebCount": 0, 
      "participatedConferenceDialInOut3rdPartyCount": 0, 
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5", 
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
