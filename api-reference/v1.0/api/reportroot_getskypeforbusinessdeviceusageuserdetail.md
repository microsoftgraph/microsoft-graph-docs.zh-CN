# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="2ec8d-101">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="2ec8d-101">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="2ec8d-102">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-102">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="2ec8d-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec8d-104">权限</span><span class="sxs-lookup"><span data-stu-id="2ec8d-104">Permissions</span></span>

<span data-ttu-id="2ec8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2ec8d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ec8d-107">Permission type</span></span>                        | <span data-ttu-id="2ec8d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ec8d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2ec8d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec8d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ec8d-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ec8d-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2ec8d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ec8d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec8d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-112">Not supported.</span></span>                           |
| <span data-ttu-id="2ec8d-113">应用</span><span class="sxs-lookup"><span data-stu-id="2ec8d-113">Application</span></span>                            | <span data-ttu-id="2ec8d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ec8d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2ec8d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ec8d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="2ec8d-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="2ec8d-116">Request parameters</span></span>

<span data-ttu-id="2ec8d-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2ec8d-118">参数</span><span class="sxs-lookup"><span data-stu-id="2ec8d-118">Parameter</span></span> | <span data-ttu-id="2ec8d-119">类型</span><span class="sxs-lookup"><span data-stu-id="2ec8d-119">Type</span></span>   | <span data-ttu-id="2ec8d-120">说明</span><span class="sxs-lookup"><span data-stu-id="2ec8d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2ec8d-121">period</span><span class="sxs-lookup"><span data-stu-id="2ec8d-121">period</span></span>    | <span data-ttu-id="2ec8d-122">string</span><span class="sxs-lookup"><span data-stu-id="2ec8d-122">string</span></span> | <span data-ttu-id="2ec8d-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2ec8d-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2ec8d-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2ec8d-126">date</span><span class="sxs-lookup"><span data-stu-id="2ec8d-126">date</span></span>      | <span data-ttu-id="2ec8d-127">Date</span><span class="sxs-lookup"><span data-stu-id="2ec8d-127">Date</span></span>   | <span data-ttu-id="2ec8d-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2ec8d-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2ec8d-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2ec8d-131">**注意：**需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ec8d-132">请求头</span><span class="sxs-lookup"><span data-stu-id="2ec8d-132">Request headers</span></span>

| <span data-ttu-id="2ec8d-133">名称</span><span class="sxs-lookup"><span data-stu-id="2ec8d-133">Name</span></span>          | <span data-ttu-id="2ec8d-134">说明</span><span class="sxs-lookup"><span data-stu-id="2ec8d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2ec8d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ec8d-135">Authorization</span></span> | <span data-ttu-id="2ec8d-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2ec8d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2ec8d-138">If-None-Match</span></span> | <span data-ttu-id="2ec8d-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2ec8d-140">可选。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2ec8d-141">响应</span><span class="sxs-lookup"><span data-stu-id="2ec8d-141">Response</span></span>

<span data-ttu-id="2ec8d-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2ec8d-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2ec8d-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2ec8d-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2ec8d-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2ec8d-146">Report Refresh Date</span></span>
- <span data-ttu-id="2ec8d-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2ec8d-147">User Principal Name</span></span>
- <span data-ttu-id="2ec8d-148">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="2ec8d-148">Last Activity Date</span></span>
- <span data-ttu-id="2ec8d-149">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="2ec8d-149">Used Windows</span></span>
- <span data-ttu-id="2ec8d-150">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="2ec8d-150">Used Windows Phone</span></span>
- <span data-ttu-id="2ec8d-151">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="2ec8d-151">Used Android Phone</span></span>
- <span data-ttu-id="2ec8d-152">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="2ec8d-152">Used iPhone</span></span>
- <span data-ttu-id="2ec8d-153">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="2ec8d-153">Used iPad</span></span>
- <span data-ttu-id="2ec8d-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="2ec8d-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2ec8d-155">示例</span><span class="sxs-lookup"><span data-stu-id="2ec8d-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2ec8d-156">请求</span><span class="sxs-lookup"><span data-stu-id="2ec8d-156">Request</span></span>

<span data-ttu-id="2ec8d-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2ec8d-158">响应</span><span class="sxs-lookup"><span data-stu-id="2ec8d-158">Response</span></span>

<span data-ttu-id="2ec8d-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2ec8d-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2ec8d-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
