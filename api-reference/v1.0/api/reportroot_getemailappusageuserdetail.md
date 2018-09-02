# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="6ae7e-101">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="6ae7e-101">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="6ae7e-102">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-102">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="6ae7e-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ae7e-104">权限</span><span class="sxs-lookup"><span data-stu-id="6ae7e-104">Permissions</span></span>

<span data-ttu-id="6ae7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6ae7e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ae7e-107">Permission type</span></span>                        | <span data-ttu-id="6ae7e-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ae7e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6ae7e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ae7e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ae7e-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ae7e-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6ae7e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ae7e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ae7e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-112">Not supported.</span></span>                           |
| <span data-ttu-id="6ae7e-113">应用</span><span class="sxs-lookup"><span data-stu-id="6ae7e-113">Application</span></span>                            | <span data-ttu-id="6ae7e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ae7e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6ae7e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ae7e-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6ae7e-116">函数参数</span><span class="sxs-lookup"><span data-stu-id="6ae7e-116">Function parameters</span></span>

<span data-ttu-id="6ae7e-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6ae7e-118">参数</span><span class="sxs-lookup"><span data-stu-id="6ae7e-118">Parameter</span></span> | <span data-ttu-id="6ae7e-119">类型</span><span class="sxs-lookup"><span data-stu-id="6ae7e-119">Type</span></span>   | <span data-ttu-id="6ae7e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6ae7e-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6ae7e-121">period</span><span class="sxs-lookup"><span data-stu-id="6ae7e-121">period</span></span>    | <span data-ttu-id="6ae7e-122">字符串</span><span class="sxs-lookup"><span data-stu-id="6ae7e-122">string</span></span> | <span data-ttu-id="6ae7e-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6ae7e-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6ae7e-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6ae7e-126">date</span><span class="sxs-lookup"><span data-stu-id="6ae7e-126">date</span></span>      | <span data-ttu-id="6ae7e-127">日期</span><span class="sxs-lookup"><span data-stu-id="6ae7e-127">Date</span></span>   | <span data-ttu-id="6ae7e-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6ae7e-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6ae7e-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6ae7e-131">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ae7e-132">请求头</span><span class="sxs-lookup"><span data-stu-id="6ae7e-132">Request headers</span></span>

| <span data-ttu-id="6ae7e-133">名称</span><span class="sxs-lookup"><span data-stu-id="6ae7e-133">Name</span></span>          | <span data-ttu-id="6ae7e-134">说明</span><span class="sxs-lookup"><span data-stu-id="6ae7e-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6ae7e-135">授权</span><span class="sxs-lookup"><span data-stu-id="6ae7e-135">Authorization</span></span> | <span data-ttu-id="6ae7e-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6ae7e-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6ae7e-138">If-None-Match</span></span> | <span data-ttu-id="6ae7e-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6ae7e-140">可选。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6ae7e-141">响应</span><span class="sxs-lookup"><span data-stu-id="6ae7e-141">Response</span></span>

<span data-ttu-id="6ae7e-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6ae7e-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6ae7e-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6ae7e-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6ae7e-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6ae7e-146">Report Refresh Date</span></span>
- <span data-ttu-id="6ae7e-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6ae7e-147">User Principal Name</span></span>
- <span data-ttu-id="6ae7e-148">显示名称</span><span class="sxs-lookup"><span data-stu-id="6ae7e-148">Display Name</span></span>
- <span data-ttu-id="6ae7e-149">已删除</span><span class="sxs-lookup"><span data-stu-id="6ae7e-149">Is Deleted</span></span>
- <span data-ttu-id="6ae7e-150">删除日期</span><span class="sxs-lookup"><span data-stu-id="6ae7e-150">Deleted Date</span></span>
- <span data-ttu-id="6ae7e-151">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6ae7e-151">Last Activity Date</span></span>
- <span data-ttu-id="6ae7e-152">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="6ae7e-152">Mail For Mac</span></span>
- <span data-ttu-id="6ae7e-153">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="6ae7e-153">Outlook For Mac</span></span>
- <span data-ttu-id="6ae7e-154">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="6ae7e-154">Outlook For Windows</span></span>
- <span data-ttu-id="6ae7e-155">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="6ae7e-155">Outlook For Mobile</span></span>
- <span data-ttu-id="6ae7e-156">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="6ae7e-156">Other For Mobile</span></span>
- <span data-ttu-id="6ae7e-157">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="6ae7e-157">Outlook For Web</span></span>
- <span data-ttu-id="6ae7e-158">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="6ae7e-158">POP3 App</span></span>
- <span data-ttu-id="6ae7e-159">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="6ae7e-159">IMAP4 App</span></span>
- <span data-ttu-id="6ae7e-160">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="6ae7e-160">SMTP App</span></span>
- <span data-ttu-id="6ae7e-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="6ae7e-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6ae7e-162">示例</span><span class="sxs-lookup"><span data-stu-id="6ae7e-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6ae7e-163">请求</span><span class="sxs-lookup"><span data-stu-id="6ae7e-163">Request</span></span>

<span data-ttu-id="6ae7e-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6ae7e-165">响应</span><span class="sxs-lookup"><span data-stu-id="6ae7e-165">Response</span></span>

<span data-ttu-id="6ae7e-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="6ae7e-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6ae7e-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
