# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="eebeb-101">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="eebeb-101">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="eebeb-102">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="eebeb-102">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="eebeb-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="eebeb-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="eebeb-104">权限</span><span class="sxs-lookup"><span data-stu-id="eebeb-104">Permissions</span></span>

<span data-ttu-id="eebeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eebeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="eebeb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="eebeb-107">Permission type</span></span>                        | <span data-ttu-id="eebeb-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eebeb-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eebeb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eebeb-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="eebeb-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eebeb-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eebeb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eebeb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eebeb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="eebeb-112">Not supported.</span></span>                           |
| <span data-ttu-id="eebeb-113">应用</span><span class="sxs-lookup"><span data-stu-id="eebeb-113">Application</span></span>                            | <span data-ttu-id="eebeb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eebeb-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eebeb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eebeb-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="eebeb-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="eebeb-116">Request parameters</span></span>

<span data-ttu-id="eebeb-117">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="eebeb-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eebeb-118">参数</span><span class="sxs-lookup"><span data-stu-id="eebeb-118">Parameter</span></span> | <span data-ttu-id="eebeb-119">类型</span><span class="sxs-lookup"><span data-stu-id="eebeb-119">Type</span></span>   | <span data-ttu-id="eebeb-120">说明</span><span class="sxs-lookup"><span data-stu-id="eebeb-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eebeb-121">period</span><span class="sxs-lookup"><span data-stu-id="eebeb-121">period</span></span>    | <span data-ttu-id="eebeb-122">string</span><span class="sxs-lookup"><span data-stu-id="eebeb-122">string</span></span> | <span data-ttu-id="eebeb-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="eebeb-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eebeb-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="eebeb-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eebeb-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="eebeb-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eebeb-126">必需。</span><span class="sxs-lookup"><span data-stu-id="eebeb-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="eebeb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="eebeb-127">Request headers</span></span>

| <span data-ttu-id="eebeb-128">名称</span><span class="sxs-lookup"><span data-stu-id="eebeb-128">Name</span></span>          | <span data-ttu-id="eebeb-129">说明</span><span class="sxs-lookup"><span data-stu-id="eebeb-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eebeb-130">授权</span><span class="sxs-lookup"><span data-stu-id="eebeb-130">Authorization</span></span> | <span data-ttu-id="eebeb-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="eebeb-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eebeb-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eebeb-133">If-None-Match</span></span> | <span data-ttu-id="eebeb-134">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eebeb-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eebeb-135">可选。</span><span class="sxs-lookup"><span data-stu-id="eebeb-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eebeb-136">响应</span><span class="sxs-lookup"><span data-stu-id="eebeb-136">Response</span></span>

<span data-ttu-id="eebeb-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="eebeb-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eebeb-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="eebeb-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eebeb-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="eebeb-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eebeb-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="eebeb-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eebeb-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="eebeb-141">Report Refresh Date</span></span>
- <span data-ttu-id="eebeb-142">总计</span><span class="sxs-lookup"><span data-stu-id="eebeb-142">Total</span></span>
- <span data-ttu-id="eebeb-143">活跃</span><span class="sxs-lookup"><span data-stu-id="eebeb-143">Active</span></span>
- <span data-ttu-id="eebeb-144">报表日期</span><span class="sxs-lookup"><span data-stu-id="eebeb-144">Report Date</span></span>
- <span data-ttu-id="eebeb-145">报表周期</span><span class="sxs-lookup"><span data-stu-id="eebeb-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="eebeb-146">示例</span><span class="sxs-lookup"><span data-stu-id="eebeb-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eebeb-147">请求</span><span class="sxs-lookup"><span data-stu-id="eebeb-147">Request</span></span>

<span data-ttu-id="eebeb-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eebeb-148">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="eebeb-149">响应</span><span class="sxs-lookup"><span data-stu-id="eebeb-149">Response</span></span>

<span data-ttu-id="eebeb-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eebeb-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="eebeb-151">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="eebeb-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
