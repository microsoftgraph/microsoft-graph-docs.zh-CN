# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="fece3-101">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fece3-101">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="fece3-102">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="fece3-102">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="fece3-103">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="fece3-103">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="fece3-104">权限</span><span class="sxs-lookup"><span data-stu-id="fece3-104">Permissions</span></span>

<span data-ttu-id="fece3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fece3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fece3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fece3-107">Permission type</span></span>                        | <span data-ttu-id="fece3-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fece3-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fece3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fece3-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fece3-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece3-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fece3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fece3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fece3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fece3-112">Not supported.</span></span>                           |
| <span data-ttu-id="fece3-113">应用</span><span class="sxs-lookup"><span data-stu-id="fece3-113">Application</span></span>                            | <span data-ttu-id="fece3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece3-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fece3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fece3-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="fece3-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="fece3-116">Request parameters</span></span>

<span data-ttu-id="fece3-117">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fece3-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fece3-118">参数</span><span class="sxs-lookup"><span data-stu-id="fece3-118">Parameter</span></span> | <span data-ttu-id="fece3-119">类型</span><span class="sxs-lookup"><span data-stu-id="fece3-119">Type</span></span>   | <span data-ttu-id="fece3-120">说明</span><span class="sxs-lookup"><span data-stu-id="fece3-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fece3-121">period</span><span class="sxs-lookup"><span data-stu-id="fece3-121">period</span></span>    | <span data-ttu-id="fece3-122">string</span><span class="sxs-lookup"><span data-stu-id="fece3-122">string</span></span> | <span data-ttu-id="fece3-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fece3-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fece3-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fece3-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fece3-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fece3-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fece3-126">必需。</span><span class="sxs-lookup"><span data-stu-id="fece3-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fece3-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="fece3-127">Request headers</span></span>

| <span data-ttu-id="fece3-128">名称</span><span class="sxs-lookup"><span data-stu-id="fece3-128">Name</span></span>          | <span data-ttu-id="fece3-129">说明</span><span class="sxs-lookup"><span data-stu-id="fece3-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fece3-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fece3-130">Authorization</span></span> | <span data-ttu-id="fece3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fece3-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fece3-133">响应</span><span class="sxs-lookup"><span data-stu-id="fece3-133">Response</span></span>

<span data-ttu-id="fece3-134">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fece3-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fece3-135">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fece3-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fece3-136">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="fece3-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fece3-137">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="fece3-137">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="fece3-138">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fece3-138">Report Refresh Date</span></span>
- <span data-ttu-id="fece3-139">报表日期</span><span class="sxs-lookup"><span data-stu-id="fece3-139">Report Date</span></span>
- <span data-ttu-id="fece3-140">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="fece3-140">Team Chat Messages</span></span>
- <span data-ttu-id="fece3-141">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="fece3-141">Private Chat Messages</span></span>
- <span data-ttu-id="fece3-142">呼叫</span><span class="sxs-lookup"><span data-stu-id="fece3-142">Calls</span></span>
- <span data-ttu-id="fece3-143">会议</span><span class="sxs-lookup"><span data-stu-id="fece3-143">Meetings</span></span>
- <span data-ttu-id="fece3-144">其他操作</span><span class="sxs-lookup"><span data-stu-id="fece3-144">Other Actions</span></span>
- <span data-ttu-id="fece3-145">报表周期</span><span class="sxs-lookup"><span data-stu-id="fece3-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fece3-146">示例</span><span class="sxs-lookup"><span data-stu-id="fece3-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fece3-147">请求</span><span class="sxs-lookup"><span data-stu-id="fece3-147">Request</span></span>

<span data-ttu-id="fece3-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fece3-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fece3-149">响应</span><span class="sxs-lookup"><span data-stu-id="fece3-149">Response</span></span>

<span data-ttu-id="fece3-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fece3-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fece3-151">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fece3-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
