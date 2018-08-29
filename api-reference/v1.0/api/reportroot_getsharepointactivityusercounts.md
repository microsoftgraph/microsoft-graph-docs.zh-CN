# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="b7294-101">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b7294-101">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="b7294-102">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="b7294-102">Get the trend in the number of active users.</span></span> <span data-ttu-id="b7294-103">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="b7294-103">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="b7294-104">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="b7294-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7294-105">权限</span><span class="sxs-lookup"><span data-stu-id="b7294-105">Permissions</span></span>

<span data-ttu-id="b7294-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b7294-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b7294-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7294-108">Permission type</span></span>                        | <span data-ttu-id="b7294-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7294-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7294-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7294-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7294-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7294-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7294-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7294-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7294-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7294-113">Not supported.</span></span>                           |
| <span data-ttu-id="b7294-114">应用</span><span class="sxs-lookup"><span data-stu-id="b7294-114">Application</span></span>                            | <span data-ttu-id="b7294-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7294-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7294-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7294-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="b7294-117">请求参数</span><span class="sxs-lookup"><span data-stu-id="b7294-117">Request parameters</span></span>

<span data-ttu-id="b7294-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b7294-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b7294-119">参数</span><span class="sxs-lookup"><span data-stu-id="b7294-119">Parameter</span></span> | <span data-ttu-id="b7294-120">类型</span><span class="sxs-lookup"><span data-stu-id="b7294-120">Type</span></span>   | <span data-ttu-id="b7294-121">说明</span><span class="sxs-lookup"><span data-stu-id="b7294-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7294-122">period</span><span class="sxs-lookup"><span data-stu-id="b7294-122">period</span></span>    | <span data-ttu-id="b7294-123">string</span><span class="sxs-lookup"><span data-stu-id="b7294-123">string</span></span> | <span data-ttu-id="b7294-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b7294-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7294-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b7294-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7294-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b7294-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b7294-127">必需。</span><span class="sxs-lookup"><span data-stu-id="b7294-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b7294-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7294-128">Request headers</span></span>

| <span data-ttu-id="b7294-129">名称</span><span class="sxs-lookup"><span data-stu-id="b7294-129">Name</span></span>          | <span data-ttu-id="b7294-130">说明</span><span class="sxs-lookup"><span data-stu-id="b7294-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b7294-131">授权</span><span class="sxs-lookup"><span data-stu-id="b7294-131">Authorization</span></span> | <span data-ttu-id="b7294-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7294-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b7294-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b7294-134">If-None-Match</span></span> | <span data-ttu-id="b7294-135">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b7294-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b7294-136">可选。</span><span class="sxs-lookup"><span data-stu-id="b7294-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b7294-137">响应</span><span class="sxs-lookup"><span data-stu-id="b7294-137">Response</span></span>

<span data-ttu-id="b7294-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b7294-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7294-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b7294-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7294-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b7294-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7294-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b7294-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7294-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b7294-142">Report Refresh Date</span></span>
- <span data-ttu-id="b7294-143">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="b7294-143">Visited Page</span></span>
- <span data-ttu-id="b7294-144">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="b7294-144">Viewed Or Edited</span></span>
- <span data-ttu-id="b7294-145">已同步</span><span class="sxs-lookup"><span data-stu-id="b7294-145">Synced</span></span>
- <span data-ttu-id="b7294-146">已内部共享</span><span class="sxs-lookup"><span data-stu-id="b7294-146">Shared Internally</span></span>
- <span data-ttu-id="b7294-147">已外部共享</span><span class="sxs-lookup"><span data-stu-id="b7294-147">Shared Externally</span></span>
- <span data-ttu-id="b7294-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="b7294-148">Report Date</span></span>
- <span data-ttu-id="b7294-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="b7294-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b7294-150">示例</span><span class="sxs-lookup"><span data-stu-id="b7294-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7294-151">请求</span><span class="sxs-lookup"><span data-stu-id="b7294-151">Request</span></span>

<span data-ttu-id="b7294-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7294-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b7294-153">响应</span><span class="sxs-lookup"><span data-stu-id="b7294-153">Response</span></span>

<span data-ttu-id="b7294-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7294-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="b7294-155">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b7294-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
