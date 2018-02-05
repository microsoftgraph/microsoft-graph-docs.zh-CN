# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="7e7f9-101">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="7e7f9-101">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="7e7f9-102">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-102">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="7e7f9-103">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-103">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="7e7f9-104">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-104">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e7f9-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e7f9-105">Permissions</span></span>

<span data-ttu-id="7e7f9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7e7f9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e7f9-108">Permission type</span></span>                        | <span data-ttu-id="7e7f9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e7f9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7e7f9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e7f9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e7f9-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-111">Not supported.</span></span>                           |
| <span data-ttu-id="7e7f9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e7f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e7f9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-113">Not supported.</span></span>                           |
| <span data-ttu-id="7e7f9-114">应用</span><span class="sxs-lookup"><span data-stu-id="7e7f9-114">Application</span></span>                            | <span data-ttu-id="7e7f9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e7f9-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7e7f9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e7f9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="7e7f9-117">请求参数</span><span class="sxs-lookup"><span data-stu-id="7e7f9-117">Request parameters</span></span>

<span data-ttu-id="7e7f9-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="7e7f9-119">参数</span><span class="sxs-lookup"><span data-stu-id="7e7f9-119">Parameter</span></span> | <span data-ttu-id="7e7f9-120">类型</span><span class="sxs-lookup"><span data-stu-id="7e7f9-120">Type</span></span>   | <span data-ttu-id="7e7f9-121">说明</span><span class="sxs-lookup"><span data-stu-id="7e7f9-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7e7f9-122">period</span><span class="sxs-lookup"><span data-stu-id="7e7f9-122">period</span></span>    | <span data-ttu-id="7e7f9-123">string</span><span class="sxs-lookup"><span data-stu-id="7e7f9-123">string</span></span> | <span data-ttu-id="7e7f9-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7e7f9-125">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7e7f9-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7e7f9-127">必需。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7e7f9-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e7f9-128">Request headers</span></span>

| <span data-ttu-id="7e7f9-129">名称</span><span class="sxs-lookup"><span data-stu-id="7e7f9-129">Name</span></span>          | <span data-ttu-id="7e7f9-130">说明</span><span class="sxs-lookup"><span data-stu-id="7e7f9-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7e7f9-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e7f9-131">Authorization</span></span> | <span data-ttu-id="7e7f9-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e7f9-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7e7f9-134">If-None-Match</span></span> | <span data-ttu-id="7e7f9-135">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7e7f9-136">可选。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7e7f9-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e7f9-137">Response</span></span>

<span data-ttu-id="7e7f9-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7e7f9-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7e7f9-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7e7f9-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7e7f9-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7e7f9-142">Report Refresh Date</span></span>
- <span data-ttu-id="7e7f9-143">网站类型</span><span class="sxs-lookup"><span data-stu-id="7e7f9-143">Site Type</span></span>
- <span data-ttu-id="7e7f9-144">总计</span><span class="sxs-lookup"><span data-stu-id="7e7f9-144">Total</span></span>
- <span data-ttu-id="7e7f9-145">活跃</span><span class="sxs-lookup"><span data-stu-id="7e7f9-145">Active</span></span>
- <span data-ttu-id="7e7f9-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="7e7f9-146">Report Date</span></span>
- <span data-ttu-id="7e7f9-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="7e7f9-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7e7f9-148">示例</span><span class="sxs-lookup"><span data-stu-id="7e7f9-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e7f9-149">请求</span><span class="sxs-lookup"><span data-stu-id="7e7f9-149">Request</span></span>

<span data-ttu-id="7e7f9-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7e7f9-151">响应</span><span class="sxs-lookup"><span data-stu-id="7e7f9-151">Response</span></span>

<span data-ttu-id="7e7f9-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7e7f9-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7e7f9-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
