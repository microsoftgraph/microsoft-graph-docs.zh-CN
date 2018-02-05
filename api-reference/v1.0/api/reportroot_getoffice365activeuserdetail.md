# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="818bc-101">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="818bc-101">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="818bc-102">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="818bc-102">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="818bc-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="818bc-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="818bc-104">权限</span><span class="sxs-lookup"><span data-stu-id="818bc-104">Permissions</span></span>

<span data-ttu-id="818bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="818bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="818bc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="818bc-107">Permission type</span></span>                        | <span data-ttu-id="818bc-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="818bc-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="818bc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="818bc-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="818bc-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="818bc-110">Not supported.</span></span>                           |
| <span data-ttu-id="818bc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="818bc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="818bc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="818bc-112">Not supported.</span></span>                           |
| <span data-ttu-id="818bc-113">应用</span><span class="sxs-lookup"><span data-stu-id="818bc-113">Application</span></span>                            | <span data-ttu-id="818bc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="818bc-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="818bc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="818bc-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="818bc-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="818bc-116">Request parameters</span></span>

<span data-ttu-id="818bc-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="818bc-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="818bc-118">参数</span><span class="sxs-lookup"><span data-stu-id="818bc-118">Parameter</span></span> | <span data-ttu-id="818bc-119">类型</span><span class="sxs-lookup"><span data-stu-id="818bc-119">Type</span></span>   | <span data-ttu-id="818bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="818bc-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="818bc-121">period</span><span class="sxs-lookup"><span data-stu-id="818bc-121">period</span></span>    | <span data-ttu-id="818bc-122">string</span><span class="sxs-lookup"><span data-stu-id="818bc-122">string</span></span> | <span data-ttu-id="818bc-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="818bc-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="818bc-124">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="818bc-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="818bc-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="818bc-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="818bc-126">date</span><span class="sxs-lookup"><span data-stu-id="818bc-126">date</span></span>      | <span data-ttu-id="818bc-127">Date</span><span class="sxs-lookup"><span data-stu-id="818bc-127">Date</span></span>   | <span data-ttu-id="818bc-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="818bc-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="818bc-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="818bc-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="818bc-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="818bc-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="818bc-131">**注意：**需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="818bc-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="818bc-132">请求头</span><span class="sxs-lookup"><span data-stu-id="818bc-132">Request headers</span></span>

| <span data-ttu-id="818bc-133">名称</span><span class="sxs-lookup"><span data-stu-id="818bc-133">Name</span></span>          | <span data-ttu-id="818bc-134">说明</span><span class="sxs-lookup"><span data-stu-id="818bc-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="818bc-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="818bc-135">Authorization</span></span> | <span data-ttu-id="818bc-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="818bc-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="818bc-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="818bc-138">If-None-Match</span></span> | <span data-ttu-id="818bc-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="818bc-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="818bc-140">可选。</span><span class="sxs-lookup"><span data-stu-id="818bc-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="818bc-141">响应</span><span class="sxs-lookup"><span data-stu-id="818bc-141">Response</span></span>

<span data-ttu-id="818bc-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="818bc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="818bc-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="818bc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="818bc-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="818bc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="818bc-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="818bc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="818bc-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="818bc-146">Report Refresh Date</span></span>
- <span data-ttu-id="818bc-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="818bc-147">User Principal Name</span></span>
- <span data-ttu-id="818bc-148">显示名称</span><span class="sxs-lookup"><span data-stu-id="818bc-148">Display Name</span></span>
- <span data-ttu-id="818bc-149">已删除</span><span class="sxs-lookup"><span data-stu-id="818bc-149">Is Deleted</span></span>
- <span data-ttu-id="818bc-150">删除日期</span><span class="sxs-lookup"><span data-stu-id="818bc-150">Deleted Date</span></span>
- <span data-ttu-id="818bc-151">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-151">Has Exchange License</span></span>
- <span data-ttu-id="818bc-152">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-152">Has OneDrive License</span></span>
- <span data-ttu-id="818bc-153">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-153">Has SharePoint License</span></span>
- <span data-ttu-id="818bc-154">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-154">Has Skype For Business License</span></span>
- <span data-ttu-id="818bc-155">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-155">Has Yammer License</span></span>
- <span data-ttu-id="818bc-156">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="818bc-156">Has Teams License</span></span>
- <span data-ttu-id="818bc-157">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-157">Exchange Last Activity Date</span></span>
- <span data-ttu-id="818bc-158">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-158">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="818bc-159">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-159">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="818bc-160">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-160">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="818bc-161">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-161">Yammer Last Activity Date</span></span>
- <span data-ttu-id="818bc-162">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="818bc-162">Teams Last Activity Date</span></span>
- <span data-ttu-id="818bc-163">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-163">Exchange License Assign Date</span></span>
- <span data-ttu-id="818bc-164">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-164">OneDrive License Assign Date</span></span>
- <span data-ttu-id="818bc-165">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-165">SharePoint License Assign Date</span></span>
- <span data-ttu-id="818bc-166">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-166">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="818bc-167">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-167">Yammer License Assign Date</span></span>
- <span data-ttu-id="818bc-168">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="818bc-168">Teams License Assign Date</span></span>
- <span data-ttu-id="818bc-169">分配的产品</span><span class="sxs-lookup"><span data-stu-id="818bc-169">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="818bc-170">示例</span><span class="sxs-lookup"><span data-stu-id="818bc-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="818bc-171">请求</span><span class="sxs-lookup"><span data-stu-id="818bc-171">Request</span></span>

<span data-ttu-id="818bc-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="818bc-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="818bc-173">响应</span><span class="sxs-lookup"><span data-stu-id="818bc-173">Response</span></span>

<span data-ttu-id="818bc-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="818bc-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="818bc-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="818bc-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```
