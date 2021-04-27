---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: 获取用户执行的 Skype for Business 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 21c43c0098ae1a9efe7a018d51fd320a19caec17
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049742"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="dce14-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dce14-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="dce14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dce14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dce14-105">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dce14-105">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="dce14-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="dce14-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="dce14-107">权限</span><span class="sxs-lookup"><span data-stu-id="dce14-107">Permissions</span></span>

<span data-ttu-id="dce14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dce14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dce14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dce14-110">Permission type</span></span>                        | <span data-ttu-id="dce14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dce14-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dce14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dce14-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dce14-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dce14-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dce14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dce14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dce14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dce14-115">Not supported.</span></span>                           |
| <span data-ttu-id="dce14-116">应用</span><span class="sxs-lookup"><span data-stu-id="dce14-116">Application</span></span>                            | <span data-ttu-id="dce14-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dce14-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="dce14-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="dce14-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dce14-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="dce14-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dce14-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dce14-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dce14-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="dce14-121">Function parameters</span></span>

<span data-ttu-id="dce14-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="dce14-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dce14-123">参数</span><span class="sxs-lookup"><span data-stu-id="dce14-123">Parameter</span></span> | <span data-ttu-id="dce14-124">类型</span><span class="sxs-lookup"><span data-stu-id="dce14-124">Type</span></span>   | <span data-ttu-id="dce14-125">说明</span><span class="sxs-lookup"><span data-stu-id="dce14-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dce14-126">period</span><span class="sxs-lookup"><span data-stu-id="dce14-126">period</span></span>    | <span data-ttu-id="dce14-127">string</span><span class="sxs-lookup"><span data-stu-id="dce14-127">string</span></span> | <span data-ttu-id="dce14-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dce14-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dce14-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="dce14-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dce14-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dce14-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dce14-131">date</span><span class="sxs-lookup"><span data-stu-id="dce14-131">date</span></span>      | <span data-ttu-id="dce14-132">Date</span><span class="sxs-lookup"><span data-stu-id="dce14-132">Date</span></span>   | <span data-ttu-id="dce14-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="dce14-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dce14-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="dce14-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dce14-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="dce14-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dce14-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="dce14-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="dce14-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dce14-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dce14-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="dce14-138">The default output type is text/csv.</span></span> <span data-ttu-id="dce14-139">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="dce14-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dce14-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="dce14-140">Request headers</span></span>

| <span data-ttu-id="dce14-141">名称</span><span class="sxs-lookup"><span data-stu-id="dce14-141">Name</span></span>          | <span data-ttu-id="dce14-142">说明</span><span class="sxs-lookup"><span data-stu-id="dce14-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dce14-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="dce14-143">Authorization</span></span> | <span data-ttu-id="dce14-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dce14-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dce14-146">响应</span><span class="sxs-lookup"><span data-stu-id="dce14-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dce14-147">CSV</span><span class="sxs-lookup"><span data-stu-id="dce14-147">CSV</span></span>

<span data-ttu-id="dce14-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="dce14-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dce14-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="dce14-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dce14-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="dce14-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dce14-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="dce14-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dce14-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="dce14-152">Report Refresh Date</span></span>
- <span data-ttu-id="dce14-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="dce14-153">User Principal Name</span></span>
- <span data-ttu-id="dce14-154">已删除</span><span class="sxs-lookup"><span data-stu-id="dce14-154">Is Deleted</span></span>
- <span data-ttu-id="dce14-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="dce14-155">Deleted Date</span></span>
- <span data-ttu-id="dce14-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="dce14-156">Last Activity Date</span></span>
- <span data-ttu-id="dce14-157">对等会话总数</span><span class="sxs-lookup"><span data-stu-id="dce14-157">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="dce14-158">组织会议总数</span><span class="sxs-lookup"><span data-stu-id="dce14-158">Total Organized Conference Count</span></span>
- <span data-ttu-id="dce14-159">参与会议总数</span><span class="sxs-lookup"><span data-stu-id="dce14-159">Total Participated Conference Count</span></span>
- <span data-ttu-id="dce14-160">对等会话的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="dce14-160">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="dce14-161">组织会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="dce14-161">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="dce14-162">参与会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="dce14-162">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="dce14-163">对等 IM 次数</span><span class="sxs-lookup"><span data-stu-id="dce14-163">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="dce14-164">对等音频次数</span><span class="sxs-lookup"><span data-stu-id="dce14-164">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="dce14-165">对等音频分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-165">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="dce14-166">对等视频次数</span><span class="sxs-lookup"><span data-stu-id="dce14-166">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="dce14-167">对等视频分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-167">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="dce14-168">对等应用共享次数</span><span class="sxs-lookup"><span data-stu-id="dce14-168">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="dce14-169">对等文件传输次数</span><span class="sxs-lookup"><span data-stu-id="dce14-169">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="dce14-170">组织会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="dce14-170">Organized Conference IM Count</span></span>
- <span data-ttu-id="dce14-171">组织会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="dce14-171">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="dce14-172">组织会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-172">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="dce14-173">组织会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="dce14-173">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="dce14-174">组织会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="dce14-174">Organized Conference Web Count</span></span>
- <span data-ttu-id="dce14-175">组织会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="dce14-175">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="dce14-176">组织会议 - Microsoft 拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="dce14-176">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="dce14-177">组织会议 - Microsoft 拨入分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-177">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="dce14-178">组织会议 - Microsoft 拨出分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-178">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="dce14-179">参与会议 IM 计数</span><span class="sxs-lookup"><span data-stu-id="dce14-179">Participated Conference IM Count</span></span>
- <span data-ttu-id="dce14-180">参与会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="dce14-180">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="dce14-181">参与会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="dce14-181">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="dce14-182">参与会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="dce14-182">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="dce14-183">参与会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="dce14-183">Participated Conference Web Count</span></span>
- <span data-ttu-id="dce14-184">参与会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="dce14-184">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="dce14-185">分配的产品</span><span class="sxs-lookup"><span data-stu-id="dce14-185">Assigned Products</span></span>
- <span data-ttu-id="dce14-186">报表周期</span><span class="sxs-lookup"><span data-stu-id="dce14-186">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dce14-187">JSON</span><span class="sxs-lookup"><span data-stu-id="dce14-187">JSON</span></span>

<span data-ttu-id="dce14-188">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="dce14-188">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="dce14-189">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="dce14-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="dce14-190">示例</span><span class="sxs-lookup"><span data-stu-id="dce14-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dce14-191">CSV</span><span class="sxs-lookup"><span data-stu-id="dce14-191">CSV</span></span>

<span data-ttu-id="dce14-192">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="dce14-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dce14-193">请求</span><span class="sxs-lookup"><span data-stu-id="dce14-193">Request</span></span>

<span data-ttu-id="dce14-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dce14-194">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="dce14-195">响应</span><span class="sxs-lookup"><span data-stu-id="dce14-195">Response</span></span>

<span data-ttu-id="dce14-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dce14-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dce14-197">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="dce14-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="dce14-198">JSON</span><span class="sxs-lookup"><span data-stu-id="dce14-198">JSON</span></span>

<span data-ttu-id="dce14-199">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="dce14-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dce14-200">请求</span><span class="sxs-lookup"><span data-stu-id="dce14-200">Request</span></span>

<span data-ttu-id="dce14-201">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dce14-201">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="dce14-202">响应</span><span class="sxs-lookup"><span data-stu-id="dce14-202">Response</span></span>

<span data-ttu-id="dce14-203">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dce14-203">The following is an example of the response.</span></span>

> <span data-ttu-id="dce14-204">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dce14-204">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "Microsoft 365 ENTERPRISE E5", 
      ], 
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


