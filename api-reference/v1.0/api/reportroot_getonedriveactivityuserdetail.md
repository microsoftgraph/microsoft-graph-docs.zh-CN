# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="cefca-101">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="cefca-101">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="cefca-102">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cefca-102">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="cefca-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="cefca-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="cefca-104">权限</span><span class="sxs-lookup"><span data-stu-id="cefca-104">Permissions</span></span>

<span data-ttu-id="cefca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cefca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cefca-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cefca-107">Permission type</span></span>                        | <span data-ttu-id="cefca-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cefca-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cefca-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cefca-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="cefca-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cefca-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cefca-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cefca-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cefca-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cefca-112">Not supported.</span></span>                           |
| <span data-ttu-id="cefca-113">应用</span><span class="sxs-lookup"><span data-stu-id="cefca-113">Application</span></span>                            | <span data-ttu-id="cefca-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cefca-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cefca-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cefca-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="cefca-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="cefca-116">Request parameters</span></span>

<span data-ttu-id="cefca-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="cefca-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="cefca-118">参数</span><span class="sxs-lookup"><span data-stu-id="cefca-118">Parameter</span></span> | <span data-ttu-id="cefca-119">类型</span><span class="sxs-lookup"><span data-stu-id="cefca-119">Type</span></span>   | <span data-ttu-id="cefca-120">说明</span><span class="sxs-lookup"><span data-stu-id="cefca-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cefca-121">period</span><span class="sxs-lookup"><span data-stu-id="cefca-121">period</span></span>    | <span data-ttu-id="cefca-122">string</span><span class="sxs-lookup"><span data-stu-id="cefca-122">string</span></span> | <span data-ttu-id="cefca-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cefca-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cefca-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cefca-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cefca-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cefca-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cefca-126">date</span><span class="sxs-lookup"><span data-stu-id="cefca-126">date</span></span>      | <span data-ttu-id="cefca-127">Date</span><span class="sxs-lookup"><span data-stu-id="cefca-127">Date</span></span>   | <span data-ttu-id="cefca-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="cefca-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cefca-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="cefca-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cefca-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="cefca-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="cefca-131">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="cefca-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cefca-132">请求头</span><span class="sxs-lookup"><span data-stu-id="cefca-132">Request headers</span></span>

| <span data-ttu-id="cefca-133">名称</span><span class="sxs-lookup"><span data-stu-id="cefca-133">Name</span></span>          | <span data-ttu-id="cefca-134">说明</span><span class="sxs-lookup"><span data-stu-id="cefca-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cefca-135">授权</span><span class="sxs-lookup"><span data-stu-id="cefca-135">Authorization</span></span> | <span data-ttu-id="cefca-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="cefca-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cefca-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cefca-138">If-None-Match</span></span> | <span data-ttu-id="cefca-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cefca-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cefca-140">可选。</span><span class="sxs-lookup"><span data-stu-id="cefca-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cefca-141">响应</span><span class="sxs-lookup"><span data-stu-id="cefca-141">Response</span></span>

<span data-ttu-id="cefca-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cefca-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cefca-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cefca-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cefca-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cefca-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cefca-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cefca-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cefca-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cefca-146">Report Refresh Date</span></span>
- <span data-ttu-id="cefca-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="cefca-147">User Principal Name</span></span>
- <span data-ttu-id="cefca-148">已删除</span><span class="sxs-lookup"><span data-stu-id="cefca-148">Is Deleted</span></span>
- <span data-ttu-id="cefca-149">删除日期</span><span class="sxs-lookup"><span data-stu-id="cefca-149">Deleted Date</span></span>
- <span data-ttu-id="cefca-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="cefca-150">Last Activity Date</span></span>
- <span data-ttu-id="cefca-151">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="cefca-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="cefca-152">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="cefca-152">Synced File Count</span></span>
- <span data-ttu-id="cefca-153">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="cefca-153">Shared Internally File Count</span></span>
- <span data-ttu-id="cefca-154">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="cefca-154">Shared Externally File Count</span></span>
- <span data-ttu-id="cefca-155">分配的产品</span><span class="sxs-lookup"><span data-stu-id="cefca-155">Assigned Products</span></span>
- <span data-ttu-id="cefca-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="cefca-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cefca-157">示例</span><span class="sxs-lookup"><span data-stu-id="cefca-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cefca-158">请求</span><span class="sxs-lookup"><span data-stu-id="cefca-158">Request</span></span>

<span data-ttu-id="cefca-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cefca-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="cefca-160">响应</span><span class="sxs-lookup"><span data-stu-id="cefca-160">Response</span></span>

<span data-ttu-id="cefca-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cefca-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="cefca-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cefca-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
