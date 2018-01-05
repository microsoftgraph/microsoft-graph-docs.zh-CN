# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="99d1d-101">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="99d1d-101">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="99d1d-102">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="99d1d-102">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="99d1d-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况]((https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d))。</span><span class="sxs-lookup"><span data-stu-id="99d1d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage]((https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)).</span></span>

## <a name="permissions"></a><span data-ttu-id="99d1d-104">权限</span><span class="sxs-lookup"><span data-stu-id="99d1d-104">Permissions</span></span>

<span data-ttu-id="99d1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="99d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="99d1d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="99d1d-107">Permission type</span></span>                        | <span data-ttu-id="99d1d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99d1d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="99d1d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99d1d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="99d1d-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="99d1d-110">Not supported.</span></span>                           |
| <span data-ttu-id="99d1d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99d1d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99d1d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="99d1d-112">Not supported.</span></span>                           |
| <span data-ttu-id="99d1d-113">应用</span><span class="sxs-lookup"><span data-stu-id="99d1d-113">Application</span></span>                            | <span data-ttu-id="99d1d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="99d1d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="99d1d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99d1d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="99d1d-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="99d1d-116">Request parameters</span></span>

<span data-ttu-id="99d1d-117">在请求 URL 中，提供以下查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="99d1d-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="99d1d-118">参数</span><span class="sxs-lookup"><span data-stu-id="99d1d-118">Parameter</span></span> | <span data-ttu-id="99d1d-119">类型</span><span class="sxs-lookup"><span data-stu-id="99d1d-119">Type</span></span>   | <span data-ttu-id="99d1d-120">说明</span><span class="sxs-lookup"><span data-stu-id="99d1d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="99d1d-121">period</span><span class="sxs-lookup"><span data-stu-id="99d1d-121">Period</span></span>    | <span data-ttu-id="99d1d-122">string</span><span class="sxs-lookup"><span data-stu-id="99d1d-122">string</span></span> | <span data-ttu-id="99d1d-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="99d1d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="99d1d-124">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="99d1d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="99d1d-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="99d1d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="99d1d-126">必需。</span><span class="sxs-lookup"><span data-stu-id="99d1d-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="99d1d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="99d1d-127">Request headers</span></span>

| <span data-ttu-id="99d1d-128">名称</span><span class="sxs-lookup"><span data-stu-id="99d1d-128">Name</span></span>          | <span data-ttu-id="99d1d-129">说明</span><span class="sxs-lookup"><span data-stu-id="99d1d-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="99d1d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="99d1d-130">Authorization</span></span> | <span data-ttu-id="99d1d-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="99d1d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="99d1d-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="99d1d-133">if-none-match</span></span> | <span data-ttu-id="99d1d-134">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99d1d-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="99d1d-135">可选。</span><span class="sxs-lookup"><span data-stu-id="99d1d-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="99d1d-136">响应</span><span class="sxs-lookup"><span data-stu-id="99d1d-136">Response</span></span>

<span data-ttu-id="99d1d-137">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="99d1d-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="99d1d-138">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="99d1d-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="99d1d-139">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="99d1d-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="99d1d-140">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="99d1d-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="99d1d-141">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="99d1d-141">Report Refresh Date</span></span>
- <span data-ttu-id="99d1d-142">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="99d1d-142">Mail For Mac</span></span>
- <span data-ttu-id="99d1d-143">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="99d1d-143">Outlook for Mac</span></span>
- <span data-ttu-id="99d1d-144">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="99d1d-144">Outlook for Windows</span></span>
- <span data-ttu-id="99d1d-145">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="99d1d-145">Outlook For Mobile</span></span>
- <span data-ttu-id="99d1d-146">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="99d1d-146">Other For Mobile</span></span>
- <span data-ttu-id="99d1d-147">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="99d1d-147">Outlook for web</span></span>
- <span data-ttu-id="99d1d-148">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="99d1d-148">POP3 App</span></span>
- <span data-ttu-id="99d1d-149">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="99d1d-149">IMAP4 App</span></span>
- <span data-ttu-id="99d1d-150">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="99d1d-150">SMTP App</span></span>
- <span data-ttu-id="99d1d-151">报表日期</span><span class="sxs-lookup"><span data-stu-id="99d1d-151">Report Date</span></span>
- <span data-ttu-id="99d1d-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="99d1d-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="99d1d-153">示例</span><span class="sxs-lookup"><span data-stu-id="99d1d-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="99d1d-154">请求</span><span class="sxs-lookup"><span data-stu-id="99d1d-154">Request</span></span>

<span data-ttu-id="99d1d-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99d1d-155">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="99d1d-156">响应</span><span class="sxs-lookup"><span data-stu-id="99d1d-156">Response</span></span>

<span data-ttu-id="99d1d-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99d1d-157">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="99d1d-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="99d1d-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```
