# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="5f69d-101">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5f69d-101">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="5f69d-102">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="5f69d-102">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="5f69d-103">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="5f69d-103">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="5f69d-104">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="5f69d-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f69d-105">权限</span><span class="sxs-lookup"><span data-stu-id="5f69d-105">Permissions</span></span>

<span data-ttu-id="5f69d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f69d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5f69d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f69d-108">Permission type</span></span>                        | <span data-ttu-id="5f69d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f69d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f69d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f69d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f69d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f69d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f69d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f69d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f69d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f69d-113">Not supported.</span></span>                           |
| <span data-ttu-id="5f69d-114">应用</span><span class="sxs-lookup"><span data-stu-id="5f69d-114">Application</span></span>                            | <span data-ttu-id="5f69d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f69d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5f69d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f69d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="5f69d-117">请求参数</span><span class="sxs-lookup"><span data-stu-id="5f69d-117">Request parameters</span></span>

<span data-ttu-id="5f69d-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5f69d-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5f69d-119">参数</span><span class="sxs-lookup"><span data-stu-id="5f69d-119">Parameter</span></span> | <span data-ttu-id="5f69d-120">类型</span><span class="sxs-lookup"><span data-stu-id="5f69d-120">Type</span></span>   | <span data-ttu-id="5f69d-121">说明</span><span class="sxs-lookup"><span data-stu-id="5f69d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f69d-122">period</span><span class="sxs-lookup"><span data-stu-id="5f69d-122">period</span></span>    | <span data-ttu-id="5f69d-123">string</span><span class="sxs-lookup"><span data-stu-id="5f69d-123">string</span></span> | <span data-ttu-id="5f69d-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5f69d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f69d-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5f69d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f69d-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5f69d-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5f69d-127">必需。</span><span class="sxs-lookup"><span data-stu-id="5f69d-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5f69d-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f69d-128">Request headers</span></span>

| <span data-ttu-id="5f69d-129">名称</span><span class="sxs-lookup"><span data-stu-id="5f69d-129">Name</span></span>          | <span data-ttu-id="5f69d-130">说明</span><span class="sxs-lookup"><span data-stu-id="5f69d-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5f69d-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f69d-131">Authorization</span></span> | <span data-ttu-id="5f69d-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f69d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5f69d-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5f69d-134">If-None-Match</span></span> | <span data-ttu-id="5f69d-135">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5f69d-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5f69d-136">可选。</span><span class="sxs-lookup"><span data-stu-id="5f69d-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5f69d-137">响应</span><span class="sxs-lookup"><span data-stu-id="5f69d-137">Response</span></span>

<span data-ttu-id="5f69d-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5f69d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f69d-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5f69d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f69d-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5f69d-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f69d-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5f69d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f69d-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5f69d-142">Report Refresh Date</span></span>
- <span data-ttu-id="5f69d-143">报表日期</span><span class="sxs-lookup"><span data-stu-id="5f69d-143">Report Date</span></span>
- <span data-ttu-id="5f69d-144">报表周期</span><span class="sxs-lookup"><span data-stu-id="5f69d-144">Report Period</span></span>
- <span data-ttu-id="5f69d-145">IM</span><span class="sxs-lookup"><span data-stu-id="5f69d-145">IM</span></span>
- <span data-ttu-id="5f69d-146">音频</span><span class="sxs-lookup"><span data-stu-id="5f69d-146">Audio</span></span>
- <span data-ttu-id="5f69d-147">视频</span><span class="sxs-lookup"><span data-stu-id="5f69d-147">Video</span></span>
- <span data-ttu-id="5f69d-148">应用共享</span><span class="sxs-lookup"><span data-stu-id="5f69d-148">App Sharing</span></span>
- <span data-ttu-id="5f69d-149">文件传输</span><span class="sxs-lookup"><span data-stu-id="5f69d-149">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="5f69d-150">示例</span><span class="sxs-lookup"><span data-stu-id="5f69d-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f69d-151">请求</span><span class="sxs-lookup"><span data-stu-id="5f69d-151">Request</span></span>

<span data-ttu-id="5f69d-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5f69d-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5f69d-153">响应</span><span class="sxs-lookup"><span data-stu-id="5f69d-153">Response</span></span>

<span data-ttu-id="5f69d-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5f69d-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5f69d-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5f69d-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
