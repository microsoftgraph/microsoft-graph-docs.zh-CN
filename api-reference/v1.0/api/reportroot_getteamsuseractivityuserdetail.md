# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="b9940-101">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b9940-101">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="b9940-102">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9940-102">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9940-103">权限</span><span class="sxs-lookup"><span data-stu-id="b9940-103">Permissions</span></span>

<span data-ttu-id="b9940-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b9940-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9940-106">Permission type</span></span>                        | <span data-ttu-id="b9940-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9940-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b9940-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9940-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9940-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9940-109">Not supported.</span></span>                           |
| <span data-ttu-id="b9940-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9940-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9940-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9940-111">Not supported.</span></span>                           |
| <span data-ttu-id="b9940-112">应用</span><span class="sxs-lookup"><span data-stu-id="b9940-112">Application</span></span>                            | <span data-ttu-id="b9940-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9940-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b9940-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9940-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b9940-115">请求参数</span><span class="sxs-lookup"><span data-stu-id="b9940-115">Request parameters</span></span>

<span data-ttu-id="b9940-116">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="b9940-116">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="b9940-117">参数</span><span class="sxs-lookup"><span data-stu-id="b9940-117">Parameter</span></span> | <span data-ttu-id="b9940-118">类型</span><span class="sxs-lookup"><span data-stu-id="b9940-118">Type</span></span>   | <span data-ttu-id="b9940-119">说明</span><span class="sxs-lookup"><span data-stu-id="b9940-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b9940-120">period</span><span class="sxs-lookup"><span data-stu-id="b9940-120">period</span></span>    | <span data-ttu-id="b9940-121">string</span><span class="sxs-lookup"><span data-stu-id="b9940-121">string</span></span> | <span data-ttu-id="b9940-122">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b9940-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b9940-123">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b9940-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b9940-124">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b9940-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b9940-125">date</span><span class="sxs-lookup"><span data-stu-id="b9940-125">date</span></span>      | <span data-ttu-id="b9940-126">Date</span><span class="sxs-lookup"><span data-stu-id="b9940-126">Date</span></span>   | <span data-ttu-id="b9940-127">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b9940-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b9940-128">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b9940-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b9940-129">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b9940-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b9940-130">**注意：**需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b9940-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9940-131">请求头</span><span class="sxs-lookup"><span data-stu-id="b9940-131">Request headers</span></span>

| <span data-ttu-id="b9940-132">名称</span><span class="sxs-lookup"><span data-stu-id="b9940-132">Name</span></span>          | <span data-ttu-id="b9940-133">说明</span><span class="sxs-lookup"><span data-stu-id="b9940-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b9940-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9940-134">Authorization</span></span> | <span data-ttu-id="b9940-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9940-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b9940-137">响应</span><span class="sxs-lookup"><span data-stu-id="b9940-137">Response</span></span>

<span data-ttu-id="b9940-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b9940-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b9940-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b9940-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b9940-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b9940-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b9940-141">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="b9940-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b9940-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b9940-142">Report Refresh Date</span></span>
- <span data-ttu-id="b9940-143">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b9940-143">User Principal Name</span></span>
- <span data-ttu-id="b9940-144">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b9940-144">Last Activity Date</span></span>
- <span data-ttu-id="b9940-145">已删除</span><span class="sxs-lookup"><span data-stu-id="b9940-145">Is Deleted</span></span>
- <span data-ttu-id="b9940-146">删除日期</span><span class="sxs-lookup"><span data-stu-id="b9940-146">Deleted Date</span></span>
- <span data-ttu-id="b9940-147">分配的产品</span><span class="sxs-lookup"><span data-stu-id="b9940-147">Assigned Products</span></span>
- <span data-ttu-id="b9940-148">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="b9940-148">Team Chat Message Count</span></span>
- <span data-ttu-id="b9940-149">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="b9940-149">Private Chat Message Count</span></span>
- <span data-ttu-id="b9940-150">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="b9940-150">Call Count</span></span>
- <span data-ttu-id="b9940-151">会议计数</span><span class="sxs-lookup"><span data-stu-id="b9940-151">Meeting Count</span></span>
- <span data-ttu-id="b9940-152">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="b9940-152">Has Other Action</span></span>
- <span data-ttu-id="b9940-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="b9940-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b9940-154">示例</span><span class="sxs-lookup"><span data-stu-id="b9940-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9940-155">请求</span><span class="sxs-lookup"><span data-stu-id="b9940-155">Request</span></span>

<span data-ttu-id="b9940-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9940-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b9940-157">响应</span><span class="sxs-lookup"><span data-stu-id="b9940-157">Response</span></span>

<span data-ttu-id="b9940-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9940-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b9940-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b9940-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
