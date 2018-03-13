# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="2f6c9-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2f6c9-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="2f6c9-102">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-102">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f6c9-103">权限</span><span class="sxs-lookup"><span data-stu-id="2f6c9-103">Permissions</span></span>

<span data-ttu-id="2f6c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2f6c9-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f6c9-106">Permission type</span></span>                        | <span data-ttu-id="2f6c9-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f6c9-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2f6c9-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f6c9-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f6c9-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-109">Not supported.</span></span>                           |
| <span data-ttu-id="2f6c9-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f6c9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f6c9-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-111">Not supported.</span></span>                           |
| <span data-ttu-id="2f6c9-112">应用</span><span class="sxs-lookup"><span data-stu-id="2f6c9-112">Application</span></span>                            | <span data-ttu-id="2f6c9-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f6c9-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2f6c9-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f6c9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="2f6c9-115">请求参数</span><span class="sxs-lookup"><span data-stu-id="2f6c9-115">Request parameters</span></span>

<span data-ttu-id="2f6c9-116">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-116">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="2f6c9-117">参数</span><span class="sxs-lookup"><span data-stu-id="2f6c9-117">Parameter</span></span> | <span data-ttu-id="2f6c9-118">类型</span><span class="sxs-lookup"><span data-stu-id="2f6c9-118">Type</span></span>   | <span data-ttu-id="2f6c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="2f6c9-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2f6c9-120">period</span><span class="sxs-lookup"><span data-stu-id="2f6c9-120">period</span></span>    | <span data-ttu-id="2f6c9-121">string</span><span class="sxs-lookup"><span data-stu-id="2f6c9-121">string</span></span> | <span data-ttu-id="2f6c9-122">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2f6c9-123">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2f6c9-124">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2f6c9-125">必需。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2f6c9-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f6c9-126">Request headers</span></span>

| <span data-ttu-id="2f6c9-127">名称</span><span class="sxs-lookup"><span data-stu-id="2f6c9-127">Name</span></span>          | <span data-ttu-id="2f6c9-128">说明</span><span class="sxs-lookup"><span data-stu-id="2f6c9-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2f6c9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f6c9-129">Authorization</span></span> | <span data-ttu-id="2f6c9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f6c9-132">响应</span><span class="sxs-lookup"><span data-stu-id="2f6c9-132">Response</span></span>

<span data-ttu-id="2f6c9-133">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2f6c9-134">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2f6c9-135">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2f6c9-136">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="2f6c9-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2f6c9-137">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2f6c9-137">Report Refresh Date</span></span>
- <span data-ttu-id="2f6c9-138">Web</span><span class="sxs-lookup"><span data-stu-id="2f6c9-138">Web</span></span>
- <span data-ttu-id="2f6c9-139">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="2f6c9-139">Windows Phone</span></span>
- <span data-ttu-id="2f6c9-140">Android 手机</span><span class="sxs-lookup"><span data-stu-id="2f6c9-140">Android Phone</span></span>
- <span data-ttu-id="2f6c9-141">iOS</span><span class="sxs-lookup"><span data-stu-id="2f6c9-141">iOS</span></span>
- <span data-ttu-id="2f6c9-142">Mac</span><span class="sxs-lookup"><span data-stu-id="2f6c9-142">Mac</span></span>
- <span data-ttu-id="2f6c9-143">Windows</span><span class="sxs-lookup"><span data-stu-id="2f6c9-143">Windows</span></span>
- <span data-ttu-id="2f6c9-144">报表周期</span><span class="sxs-lookup"><span data-stu-id="2f6c9-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2f6c9-145">示例</span><span class="sxs-lookup"><span data-stu-id="2f6c9-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2f6c9-146">请求</span><span class="sxs-lookup"><span data-stu-id="2f6c9-146">Request</span></span>

<span data-ttu-id="2f6c9-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2f6c9-148">响应</span><span class="sxs-lookup"><span data-stu-id="2f6c9-148">Response</span></span>

<span data-ttu-id="2f6c9-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2f6c9-150">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2f6c9-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
