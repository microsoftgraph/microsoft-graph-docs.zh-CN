# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="ac031-101">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ac031-101">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="ac031-102">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ac031-102">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="ac031-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="ac031-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac031-104">权限</span><span class="sxs-lookup"><span data-stu-id="ac031-104">Permissions</span></span>

<span data-ttu-id="ac031-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ac031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ac031-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac031-107">Permission type</span></span>                        | <span data-ttu-id="ac031-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac031-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ac031-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac031-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac031-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac031-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ac031-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac031-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac031-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac031-112">Not supported.</span></span>                           |
| <span data-ttu-id="ac031-113">应用</span><span class="sxs-lookup"><span data-stu-id="ac031-113">Application</span></span>                            | <span data-ttu-id="ac031-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac031-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ac031-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac031-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="ac031-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="ac031-116">Request parameters</span></span>

<span data-ttu-id="ac031-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="ac031-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ac031-118">参数</span><span class="sxs-lookup"><span data-stu-id="ac031-118">Parameter</span></span> | <span data-ttu-id="ac031-119">类型</span><span class="sxs-lookup"><span data-stu-id="ac031-119">Type</span></span>   | <span data-ttu-id="ac031-120">说明</span><span class="sxs-lookup"><span data-stu-id="ac031-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ac031-121">period</span><span class="sxs-lookup"><span data-stu-id="ac031-121">period</span></span>    | <span data-ttu-id="ac031-122">string</span><span class="sxs-lookup"><span data-stu-id="ac031-122">string</span></span> | <span data-ttu-id="ac031-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ac031-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ac031-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ac031-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ac031-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ac031-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ac031-126">date</span><span class="sxs-lookup"><span data-stu-id="ac031-126">date</span></span>      | <span data-ttu-id="ac031-127">Date</span><span class="sxs-lookup"><span data-stu-id="ac031-127">Date</span></span>   | <span data-ttu-id="ac031-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="ac031-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ac031-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="ac031-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ac031-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="ac031-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ac031-131">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="ac031-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac031-132">请求头</span><span class="sxs-lookup"><span data-stu-id="ac031-132">Request headers</span></span>

| <span data-ttu-id="ac031-133">名称</span><span class="sxs-lookup"><span data-stu-id="ac031-133">Name</span></span>          | <span data-ttu-id="ac031-134">说明</span><span class="sxs-lookup"><span data-stu-id="ac031-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ac031-135">授权</span><span class="sxs-lookup"><span data-stu-id="ac031-135">Authorization</span></span> | <span data-ttu-id="ac031-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac031-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ac031-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ac031-138">If-None-Match</span></span> | <span data-ttu-id="ac031-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ac031-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ac031-140">可选。</span><span class="sxs-lookup"><span data-stu-id="ac031-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ac031-141">响应</span><span class="sxs-lookup"><span data-stu-id="ac031-141">Response</span></span>

<span data-ttu-id="ac031-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ac031-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ac031-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ac031-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ac031-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ac031-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ac031-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ac031-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ac031-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ac031-146">Report Refresh Date</span></span>
- <span data-ttu-id="ac031-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ac031-147">User Principal Name</span></span>
- <span data-ttu-id="ac031-148">显示名称</span><span class="sxs-lookup"><span data-stu-id="ac031-148">Display Name</span></span>
- <span data-ttu-id="ac031-149">已删除</span><span class="sxs-lookup"><span data-stu-id="ac031-149">Is Deleted</span></span>
- <span data-ttu-id="ac031-150">删除日期</span><span class="sxs-lookup"><span data-stu-id="ac031-150">Deleted Date</span></span>
- <span data-ttu-id="ac031-151">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="ac031-151">Last Activity Date</span></span>
- <span data-ttu-id="ac031-152">已发送数</span><span class="sxs-lookup"><span data-stu-id="ac031-152">Send Count</span></span>
- <span data-ttu-id="ac031-153">已接收数</span><span class="sxs-lookup"><span data-stu-id="ac031-153">Receive Count</span></span>
- <span data-ttu-id="ac031-154">已阅读数</span><span class="sxs-lookup"><span data-stu-id="ac031-154">Read Count</span></span>
- <span data-ttu-id="ac031-155">分配的产品</span><span class="sxs-lookup"><span data-stu-id="ac031-155">Assigned Products</span></span>
- <span data-ttu-id="ac031-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="ac031-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ac031-157">示例</span><span class="sxs-lookup"><span data-stu-id="ac031-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ac031-158">请求</span><span class="sxs-lookup"><span data-stu-id="ac031-158">Request</span></span>

<span data-ttu-id="ac031-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac031-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ac031-160">响应</span><span class="sxs-lookup"><span data-stu-id="ac031-160">Response</span></span>

<span data-ttu-id="ac031-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac031-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="ac031-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ac031-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```
