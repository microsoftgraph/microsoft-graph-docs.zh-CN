# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="aa1b4-101">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="aa1b4-101">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="aa1b4-102">按设备类型获取 Microsoft Teams 每日唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-102">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa1b4-103">权限</span><span class="sxs-lookup"><span data-stu-id="aa1b4-103">Permissions</span></span>

<span data-ttu-id="aa1b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="aa1b4-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa1b4-106">Permission type</span></span>                        | <span data-ttu-id="aa1b4-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa1b4-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aa1b4-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa1b4-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa1b4-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa1b4-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aa1b4-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa1b4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa1b4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-111">Not supported.</span></span>                           |
| <span data-ttu-id="aa1b4-112">应用</span><span class="sxs-lookup"><span data-stu-id="aa1b4-112">Application</span></span>                            | <span data-ttu-id="aa1b4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa1b4-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aa1b4-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa1b4-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="aa1b4-115">请求参数</span><span class="sxs-lookup"><span data-stu-id="aa1b4-115">Request parameters</span></span>

<span data-ttu-id="aa1b4-116">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-116">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aa1b4-117">参数</span><span class="sxs-lookup"><span data-stu-id="aa1b4-117">Parameter</span></span> | <span data-ttu-id="aa1b4-118">类型</span><span class="sxs-lookup"><span data-stu-id="aa1b4-118">Type</span></span>   | <span data-ttu-id="aa1b4-119">说明</span><span class="sxs-lookup"><span data-stu-id="aa1b4-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aa1b4-120">period</span><span class="sxs-lookup"><span data-stu-id="aa1b4-120">period</span></span>    | <span data-ttu-id="aa1b4-121">string</span><span class="sxs-lookup"><span data-stu-id="aa1b4-121">string</span></span> | <span data-ttu-id="aa1b4-122">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aa1b4-123">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aa1b4-124">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aa1b4-125">必需。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="aa1b4-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa1b4-126">Request headers</span></span>

| <span data-ttu-id="aa1b4-127">名称</span><span class="sxs-lookup"><span data-stu-id="aa1b4-127">Name</span></span>          | <span data-ttu-id="aa1b4-128">说明</span><span class="sxs-lookup"><span data-stu-id="aa1b4-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aa1b4-129">授权</span><span class="sxs-lookup"><span data-stu-id="aa1b4-129">Authorization</span></span> | <span data-ttu-id="aa1b4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aa1b4-132">响应</span><span class="sxs-lookup"><span data-stu-id="aa1b4-132">Response</span></span>

<span data-ttu-id="aa1b4-133">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aa1b4-134">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aa1b4-135">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aa1b4-136">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="aa1b4-136">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="aa1b4-137">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="aa1b4-137">Report Refresh Date</span></span>
- <span data-ttu-id="aa1b4-138">Web</span><span class="sxs-lookup"><span data-stu-id="aa1b4-138">Web</span></span>
- <span data-ttu-id="aa1b4-139">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="aa1b4-139">Windows Phone</span></span>
- <span data-ttu-id="aa1b4-140">Android 手机</span><span class="sxs-lookup"><span data-stu-id="aa1b4-140">Android Phone</span></span>
- <span data-ttu-id="aa1b4-141">iOS</span><span class="sxs-lookup"><span data-stu-id="aa1b4-141">iOS</span></span>
- <span data-ttu-id="aa1b4-142">Mac</span><span class="sxs-lookup"><span data-stu-id="aa1b4-142">Mac</span></span>
- <span data-ttu-id="aa1b4-143">Windows</span><span class="sxs-lookup"><span data-stu-id="aa1b4-143">Windows</span></span>
- <span data-ttu-id="aa1b4-144">报表日期</span><span class="sxs-lookup"><span data-stu-id="aa1b4-144">Report Date</span></span>
- <span data-ttu-id="aa1b4-145">报表周期</span><span class="sxs-lookup"><span data-stu-id="aa1b4-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="aa1b4-146">示例</span><span class="sxs-lookup"><span data-stu-id="aa1b4-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aa1b4-147">请求</span><span class="sxs-lookup"><span data-stu-id="aa1b4-147">Request</span></span>

<span data-ttu-id="aa1b4-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="aa1b4-149">响应</span><span class="sxs-lookup"><span data-stu-id="aa1b4-149">Response</span></span>

<span data-ttu-id="aa1b4-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="aa1b4-151">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="aa1b4-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```
