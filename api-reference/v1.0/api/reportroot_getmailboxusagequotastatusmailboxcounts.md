# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="8f14e-101">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="8f14e-101">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="8f14e-102">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="8f14e-102">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="8f14e-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="8f14e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f14e-104">权限</span><span class="sxs-lookup"><span data-stu-id="8f14e-104">Permissions</span></span>

<span data-ttu-id="8f14e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8f14e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8f14e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f14e-107">Permission type</span></span>                        | <span data-ttu-id="8f14e-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f14e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f14e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f14e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f14e-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f14e-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f14e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f14e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f14e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f14e-112">Not supported.</span></span>                           |
| <span data-ttu-id="8f14e-113">应用</span><span class="sxs-lookup"><span data-stu-id="8f14e-113">Application</span></span>                            | <span data-ttu-id="8f14e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f14e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f14e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f14e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="8f14e-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="8f14e-116">Request parameters</span></span>

<span data-ttu-id="8f14e-117">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="8f14e-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8f14e-118">参数</span><span class="sxs-lookup"><span data-stu-id="8f14e-118">Parameter</span></span> | <span data-ttu-id="8f14e-119">类型</span><span class="sxs-lookup"><span data-stu-id="8f14e-119">Type</span></span>   | <span data-ttu-id="8f14e-120">说明</span><span class="sxs-lookup"><span data-stu-id="8f14e-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f14e-121">period</span><span class="sxs-lookup"><span data-stu-id="8f14e-121">period</span></span>    | <span data-ttu-id="8f14e-122">string</span><span class="sxs-lookup"><span data-stu-id="8f14e-122">string</span></span> | <span data-ttu-id="8f14e-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8f14e-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f14e-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8f14e-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f14e-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8f14e-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8f14e-126">必需。</span><span class="sxs-lookup"><span data-stu-id="8f14e-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8f14e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f14e-127">Request headers</span></span>

| <span data-ttu-id="8f14e-128">名称</span><span class="sxs-lookup"><span data-stu-id="8f14e-128">Name</span></span>          | <span data-ttu-id="8f14e-129">说明</span><span class="sxs-lookup"><span data-stu-id="8f14e-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8f14e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f14e-130">Authorization</span></span> | <span data-ttu-id="8f14e-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f14e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8f14e-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8f14e-133">If-None-Match</span></span> | <span data-ttu-id="8f14e-134">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8f14e-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8f14e-135">可选。</span><span class="sxs-lookup"><span data-stu-id="8f14e-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8f14e-136">响应</span><span class="sxs-lookup"><span data-stu-id="8f14e-136">Response</span></span>

<span data-ttu-id="8f14e-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8f14e-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f14e-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8f14e-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f14e-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8f14e-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f14e-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="8f14e-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f14e-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8f14e-141">Report Refresh Date</span></span>
- <span data-ttu-id="8f14e-142">未达限制</span><span class="sxs-lookup"><span data-stu-id="8f14e-142">Under Limit</span></span>
- <span data-ttu-id="8f14e-143">已发出警告</span><span class="sxs-lookup"><span data-stu-id="8f14e-143">Warning Issued</span></span>
- <span data-ttu-id="8f14e-144">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="8f14e-144">Send Prohibited</span></span>
- <span data-ttu-id="8f14e-145">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="8f14e-145">Send/Receive Prohibited</span></span>
- <span data-ttu-id="8f14e-146">不确定</span><span class="sxs-lookup"><span data-stu-id="8f14e-146">Indeterminate</span></span>
- <span data-ttu-id="8f14e-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="8f14e-147">Report Date</span></span>
- <span data-ttu-id="8f14e-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="8f14e-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8f14e-149">示例</span><span class="sxs-lookup"><span data-stu-id="8f14e-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8f14e-150">请求</span><span class="sxs-lookup"><span data-stu-id="8f14e-150">Request</span></span>

<span data-ttu-id="8f14e-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8f14e-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8f14e-152">响应</span><span class="sxs-lookup"><span data-stu-id="8f14e-152">Response</span></span>

<span data-ttu-id="8f14e-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8f14e-153">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8f14e-154">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8f14e-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```
