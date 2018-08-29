# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="ed8f7-101">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ed8f7-101">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="ed8f7-102">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-102">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="ed8f7-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed8f7-104">权限</span><span class="sxs-lookup"><span data-stu-id="ed8f7-104">Permissions</span></span>

<span data-ttu-id="ed8f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ed8f7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed8f7-107">Permission type</span></span>                        | <span data-ttu-id="ed8f7-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed8f7-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ed8f7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8f7-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed8f7-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8f7-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ed8f7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed8f7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed8f7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-112">Not supported.</span></span>                           |
| <span data-ttu-id="ed8f7-113">应用</span><span class="sxs-lookup"><span data-stu-id="ed8f7-113">Application</span></span>                            | <span data-ttu-id="ed8f7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8f7-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ed8f7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed8f7-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="ed8f7-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="ed8f7-116">Request parameters</span></span>

<span data-ttu-id="ed8f7-117">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ed8f7-118">参数</span><span class="sxs-lookup"><span data-stu-id="ed8f7-118">Parameter</span></span> | <span data-ttu-id="ed8f7-119">类型</span><span class="sxs-lookup"><span data-stu-id="ed8f7-119">Type</span></span>   | <span data-ttu-id="ed8f7-120">说明</span><span class="sxs-lookup"><span data-stu-id="ed8f7-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ed8f7-121">period</span><span class="sxs-lookup"><span data-stu-id="ed8f7-121">period</span></span>    | <span data-ttu-id="ed8f7-122">string</span><span class="sxs-lookup"><span data-stu-id="ed8f7-122">string</span></span> | <span data-ttu-id="ed8f7-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ed8f7-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ed8f7-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ed8f7-126">必需。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ed8f7-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed8f7-127">Request headers</span></span>

| <span data-ttu-id="ed8f7-128">名称</span><span class="sxs-lookup"><span data-stu-id="ed8f7-128">Name</span></span>          | <span data-ttu-id="ed8f7-129">说明</span><span class="sxs-lookup"><span data-stu-id="ed8f7-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ed8f7-130">授权</span><span class="sxs-lookup"><span data-stu-id="ed8f7-130">Authorization</span></span> | <span data-ttu-id="ed8f7-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ed8f7-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ed8f7-133">If-None-Match</span></span> | <span data-ttu-id="ed8f7-134">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ed8f7-135">可选。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ed8f7-136">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f7-136">Response</span></span>

<span data-ttu-id="ed8f7-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ed8f7-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ed8f7-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ed8f7-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ed8f7-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ed8f7-141">Report Refresh Date</span></span>
- <span data-ttu-id="ed8f7-142">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="ed8f7-142">Viewed Or Edited</span></span>
- <span data-ttu-id="ed8f7-143">已同步</span><span class="sxs-lookup"><span data-stu-id="ed8f7-143">Synced</span></span>
- <span data-ttu-id="ed8f7-144">已内部共享</span><span class="sxs-lookup"><span data-stu-id="ed8f7-144">Shared Internally</span></span>
- <span data-ttu-id="ed8f7-145">已外部共享</span><span class="sxs-lookup"><span data-stu-id="ed8f7-145">Shared Externally</span></span>
- <span data-ttu-id="ed8f7-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="ed8f7-146">Report Date</span></span>
- <span data-ttu-id="ed8f7-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="ed8f7-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ed8f7-148">示例</span><span class="sxs-lookup"><span data-stu-id="ed8f7-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ed8f7-149">请求</span><span class="sxs-lookup"><span data-stu-id="ed8f7-149">Request</span></span>

<span data-ttu-id="ed8f7-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ed8f7-151">响应</span><span class="sxs-lookup"><span data-stu-id="ed8f7-151">Response</span></span>

<span data-ttu-id="ed8f7-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="ed8f7-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ed8f7-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
