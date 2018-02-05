# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="113a5-101">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="113a5-101">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="113a5-102">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="113a5-102">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="113a5-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="113a5-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="113a5-104">权限</span><span class="sxs-lookup"><span data-stu-id="113a5-104">Permissions</span></span>

<span data-ttu-id="113a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="113a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="113a5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="113a5-107">Permission type</span></span>                        | <span data-ttu-id="113a5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="113a5-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="113a5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="113a5-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="113a5-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="113a5-110">Not supported.</span></span>                           |
| <span data-ttu-id="113a5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="113a5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113a5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="113a5-112">Not supported.</span></span>                           |
| <span data-ttu-id="113a5-113">应用</span><span class="sxs-lookup"><span data-stu-id="113a5-113">Application</span></span>                            | <span data-ttu-id="113a5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="113a5-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="113a5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="113a5-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="113a5-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="113a5-116">Request parameters</span></span>

<span data-ttu-id="113a5-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="113a5-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="113a5-118">参数</span><span class="sxs-lookup"><span data-stu-id="113a5-118">Parameter</span></span> | <span data-ttu-id="113a5-119">类型</span><span class="sxs-lookup"><span data-stu-id="113a5-119">Type</span></span>   | <span data-ttu-id="113a5-120">说明</span><span class="sxs-lookup"><span data-stu-id="113a5-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="113a5-121">period</span><span class="sxs-lookup"><span data-stu-id="113a5-121">period</span></span>    | <span data-ttu-id="113a5-122">string</span><span class="sxs-lookup"><span data-stu-id="113a5-122">string</span></span> | <span data-ttu-id="113a5-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="113a5-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="113a5-124">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="113a5-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="113a5-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="113a5-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="113a5-126">date</span><span class="sxs-lookup"><span data-stu-id="113a5-126">date</span></span>      | <span data-ttu-id="113a5-127">Date</span><span class="sxs-lookup"><span data-stu-id="113a5-127">Date</span></span>   | <span data-ttu-id="113a5-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="113a5-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="113a5-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="113a5-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="113a5-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="113a5-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="113a5-131">**注意：**需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="113a5-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="113a5-132">请求头</span><span class="sxs-lookup"><span data-stu-id="113a5-132">Request headers</span></span>

| <span data-ttu-id="113a5-133">名称</span><span class="sxs-lookup"><span data-stu-id="113a5-133">Name</span></span>          | <span data-ttu-id="113a5-134">说明</span><span class="sxs-lookup"><span data-stu-id="113a5-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="113a5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="113a5-135">Authorization</span></span> | <span data-ttu-id="113a5-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="113a5-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="113a5-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="113a5-138">If-None-Match</span></span> | <span data-ttu-id="113a5-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="113a5-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="113a5-140">可选。</span><span class="sxs-lookup"><span data-stu-id="113a5-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="113a5-141">响应</span><span class="sxs-lookup"><span data-stu-id="113a5-141">Response</span></span>

<span data-ttu-id="113a5-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="113a5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="113a5-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="113a5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="113a5-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="113a5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="113a5-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="113a5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="113a5-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="113a5-146">Report Refresh Date</span></span>
- <span data-ttu-id="113a5-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="113a5-147">User Principal Name</span></span>
- <span data-ttu-id="113a5-148">已删除</span><span class="sxs-lookup"><span data-stu-id="113a5-148">Is Deleted</span></span>
- <span data-ttu-id="113a5-149">删除日期</span><span class="sxs-lookup"><span data-stu-id="113a5-149">Deleted Date</span></span>
- <span data-ttu-id="113a5-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="113a5-150">Last Activity Date</span></span>
- <span data-ttu-id="113a5-151">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="113a5-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="113a5-152">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="113a5-152">Synced File Count</span></span>
- <span data-ttu-id="113a5-153">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="113a5-153">Shared Internally File Count</span></span>
- <span data-ttu-id="113a5-154">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="113a5-154">Shared Externally File Count</span></span>
- <span data-ttu-id="113a5-155">分配的产品</span><span class="sxs-lookup"><span data-stu-id="113a5-155">Assigned Products</span></span>
- <span data-ttu-id="113a5-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="113a5-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="113a5-157">示例</span><span class="sxs-lookup"><span data-stu-id="113a5-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="113a5-158">请求</span><span class="sxs-lookup"><span data-stu-id="113a5-158">Request</span></span>

<span data-ttu-id="113a5-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="113a5-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="113a5-160">响应</span><span class="sxs-lookup"><span data-stu-id="113a5-160">Response</span></span>

<span data-ttu-id="113a5-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="113a5-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="113a5-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="113a5-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
