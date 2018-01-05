# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="82dff-101">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="82dff-101">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="82dff-102">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="82dff-102">Get details about mailbox usage.</span></span>

> <span data-ttu-id="82dff-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况]((https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729))。</span><span class="sxs-lookup"><span data-stu-id="82dff-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage]((https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)).</span></span>

## <a name="permissions"></a><span data-ttu-id="82dff-104">权限</span><span class="sxs-lookup"><span data-stu-id="82dff-104">Permissions</span></span>

<span data-ttu-id="82dff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="82dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="82dff-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="82dff-107">Permission type</span></span>                        | <span data-ttu-id="82dff-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82dff-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="82dff-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82dff-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="82dff-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="82dff-110">Not supported.</span></span>                           |
| <span data-ttu-id="82dff-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82dff-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82dff-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="82dff-112">Not supported.</span></span>                           |
| <span data-ttu-id="82dff-113">应用</span><span class="sxs-lookup"><span data-stu-id="82dff-113">Application</span></span>                            | <span data-ttu-id="82dff-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82dff-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="82dff-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82dff-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="82dff-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="82dff-116">Request parameters</span></span>

<span data-ttu-id="82dff-117">在请求 URL 中，提供以下查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="82dff-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="82dff-118">参数</span><span class="sxs-lookup"><span data-stu-id="82dff-118">Parameter</span></span> | <span data-ttu-id="82dff-119">类型</span><span class="sxs-lookup"><span data-stu-id="82dff-119">Type</span></span>   | <span data-ttu-id="82dff-120">说明</span><span class="sxs-lookup"><span data-stu-id="82dff-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="82dff-121">period</span><span class="sxs-lookup"><span data-stu-id="82dff-121">Period</span></span>    | <span data-ttu-id="82dff-122">string</span><span class="sxs-lookup"><span data-stu-id="82dff-122">string</span></span> | <span data-ttu-id="82dff-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="82dff-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="82dff-124">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="82dff-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="82dff-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="82dff-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="82dff-126">必需。</span><span class="sxs-lookup"><span data-stu-id="82dff-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="82dff-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="82dff-127">Request headers</span></span>

| <span data-ttu-id="82dff-128">名称</span><span class="sxs-lookup"><span data-stu-id="82dff-128">Name</span></span>          | <span data-ttu-id="82dff-129">说明</span><span class="sxs-lookup"><span data-stu-id="82dff-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="82dff-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="82dff-130">Authorization</span></span> | <span data-ttu-id="82dff-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="82dff-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="82dff-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="82dff-133">if-none-match</span></span> | <span data-ttu-id="82dff-134">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="82dff-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="82dff-135">可选。</span><span class="sxs-lookup"><span data-stu-id="82dff-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="82dff-136">响应</span><span class="sxs-lookup"><span data-stu-id="82dff-136">Response</span></span>

<span data-ttu-id="82dff-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="82dff-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="82dff-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="82dff-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="82dff-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="82dff-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="82dff-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="82dff-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="82dff-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="82dff-141">Report Refresh Date</span></span>
- <span data-ttu-id="82dff-142">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="82dff-142">User Principal Name</span></span>
- <span data-ttu-id="82dff-143">显示名称</span><span class="sxs-lookup"><span data-stu-id="82dff-143">Display Name</span></span>
- <span data-ttu-id="82dff-144">已删除</span><span class="sxs-lookup"><span data-stu-id="82dff-144">Is Deleted</span></span>
- <span data-ttu-id="82dff-145">删除日期</span><span class="sxs-lookup"><span data-stu-id="82dff-145">Deleted Date</span></span>
- <span data-ttu-id="82dff-146">创建日期</span><span class="sxs-lookup"><span data-stu-id="82dff-146">Created Date</span></span>
- <span data-ttu-id="82dff-147">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="82dff-147">Last Activity Date</span></span>
- <span data-ttu-id="82dff-148">项数</span><span class="sxs-lookup"><span data-stu-id="82dff-148">Item Count</span></span>
- <span data-ttu-id="82dff-149">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="82dff-149">Storage Used (Byte)</span></span>
- <span data-ttu-id="82dff-150">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="82dff-150">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="82dff-151">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="82dff-151">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="82dff-152">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="82dff-152">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="82dff-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="82dff-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="82dff-154">示例</span><span class="sxs-lookup"><span data-stu-id="82dff-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="82dff-155">请求</span><span class="sxs-lookup"><span data-stu-id="82dff-155">Request</span></span>

<span data-ttu-id="82dff-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82dff-156">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="82dff-157">响应</span><span class="sxs-lookup"><span data-stu-id="82dff-157">Response</span></span>

<span data-ttu-id="82dff-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="82dff-158">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="82dff-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="82dff-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
