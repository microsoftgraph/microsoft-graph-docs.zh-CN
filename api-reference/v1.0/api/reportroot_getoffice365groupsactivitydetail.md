# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="a70cf-101">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a70cf-101">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="a70cf-102">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a70cf-102">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="a70cf-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="a70cf-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="a70cf-104">权限</span><span class="sxs-lookup"><span data-stu-id="a70cf-104">Permissions</span></span>

<span data-ttu-id="a70cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a70cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a70cf-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a70cf-107">Permission type</span></span>                        | <span data-ttu-id="a70cf-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a70cf-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a70cf-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a70cf-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a70cf-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a70cf-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a70cf-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a70cf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a70cf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a70cf-112">Not supported.</span></span>                           |
| <span data-ttu-id="a70cf-113">应用</span><span class="sxs-lookup"><span data-stu-id="a70cf-113">Application</span></span>                            | <span data-ttu-id="a70cf-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a70cf-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a70cf-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a70cf-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a70cf-116">函数参数</span><span class="sxs-lookup"><span data-stu-id="a70cf-116">Function parameters</span></span>

<span data-ttu-id="a70cf-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="a70cf-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a70cf-118">参数</span><span class="sxs-lookup"><span data-stu-id="a70cf-118">Parameter</span></span> | <span data-ttu-id="a70cf-119">类型</span><span class="sxs-lookup"><span data-stu-id="a70cf-119">Type</span></span>   | <span data-ttu-id="a70cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="a70cf-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a70cf-121">period</span><span class="sxs-lookup"><span data-stu-id="a70cf-121">period</span></span>    | <span data-ttu-id="a70cf-122">字符串</span><span class="sxs-lookup"><span data-stu-id="a70cf-122">string</span></span> | <span data-ttu-id="a70cf-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a70cf-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a70cf-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a70cf-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a70cf-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a70cf-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a70cf-126">date</span><span class="sxs-lookup"><span data-stu-id="a70cf-126">date</span></span>      | <span data-ttu-id="a70cf-127">日期</span><span class="sxs-lookup"><span data-stu-id="a70cf-127">Date</span></span>   | <span data-ttu-id="a70cf-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a70cf-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a70cf-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a70cf-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a70cf-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a70cf-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a70cf-131">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a70cf-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a70cf-132">请求头</span><span class="sxs-lookup"><span data-stu-id="a70cf-132">Request headers</span></span>

| <span data-ttu-id="a70cf-133">名称</span><span class="sxs-lookup"><span data-stu-id="a70cf-133">Name</span></span>          | <span data-ttu-id="a70cf-134">说明</span><span class="sxs-lookup"><span data-stu-id="a70cf-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a70cf-135">授权</span><span class="sxs-lookup"><span data-stu-id="a70cf-135">Authorization</span></span> | <span data-ttu-id="a70cf-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="a70cf-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a70cf-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a70cf-138">If-None-Match</span></span> | <span data-ttu-id="a70cf-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a70cf-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a70cf-140">可选。</span><span class="sxs-lookup"><span data-stu-id="a70cf-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a70cf-141">响应</span><span class="sxs-lookup"><span data-stu-id="a70cf-141">Response</span></span>

<span data-ttu-id="a70cf-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a70cf-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a70cf-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a70cf-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a70cf-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a70cf-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a70cf-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a70cf-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a70cf-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a70cf-146">Report Refresh Date</span></span>
- <span data-ttu-id="a70cf-147">组显示名称</span><span class="sxs-lookup"><span data-stu-id="a70cf-147">Group Display Name</span></span>
- <span data-ttu-id="a70cf-148">已删除</span><span class="sxs-lookup"><span data-stu-id="a70cf-148">Is Deleted</span></span>
- <span data-ttu-id="a70cf-149">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="a70cf-149">Owner Principal Name</span></span>
- <span data-ttu-id="a70cf-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a70cf-150">Last Activity Date</span></span>
- <span data-ttu-id="a70cf-151">组类型</span><span class="sxs-lookup"><span data-stu-id="a70cf-151">Group Type</span></span>
- <span data-ttu-id="a70cf-152">成员数</span><span class="sxs-lookup"><span data-stu-id="a70cf-152">Member Count</span></span>
- <span data-ttu-id="a70cf-153">外部成员数</span><span class="sxs-lookup"><span data-stu-id="a70cf-153">External Member Count</span></span>
- <span data-ttu-id="a70cf-154">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="a70cf-154">Exchange Received Email Count</span></span>
- <span data-ttu-id="a70cf-155">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="a70cf-155">SharePoint Active File Count</span></span>
- <span data-ttu-id="a70cf-156">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="a70cf-156">Yammer Posted Message Count</span></span>
- <span data-ttu-id="a70cf-157">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="a70cf-157">Yammer Read Message Count</span></span>
- <span data-ttu-id="a70cf-158">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="a70cf-158">Yammer Liked Message Count</span></span>
- <span data-ttu-id="a70cf-159">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="a70cf-159">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="a70cf-160">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="a70cf-160">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="a70cf-161">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="a70cf-161">SharePoint Total File Count</span></span>
- <span data-ttu-id="a70cf-162">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="a70cf-162">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="a70cf-163">报表周期</span><span class="sxs-lookup"><span data-stu-id="a70cf-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a70cf-164">示例</span><span class="sxs-lookup"><span data-stu-id="a70cf-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a70cf-165">请求</span><span class="sxs-lookup"><span data-stu-id="a70cf-165">Request</span></span>

<span data-ttu-id="a70cf-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a70cf-166">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a70cf-167">响应</span><span class="sxs-lookup"><span data-stu-id="a70cf-167">Response</span></span>

<span data-ttu-id="a70cf-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a70cf-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="a70cf-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a70cf-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
