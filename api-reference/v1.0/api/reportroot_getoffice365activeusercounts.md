# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="fb669-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="fb669-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="fb669-102">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="fb669-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="fb669-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="fb669-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb669-104">权限</span><span class="sxs-lookup"><span data-stu-id="fb669-104">Permissions</span></span>

<span data-ttu-id="fb669-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fb669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fb669-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb669-107">Permission type</span></span>                        | <span data-ttu-id="fb669-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb669-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fb669-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb669-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb669-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb669-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fb669-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb669-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb669-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb669-112">Not supported.</span></span>                           |
| <span data-ttu-id="fb669-113">应用</span><span class="sxs-lookup"><span data-stu-id="fb669-113">Application</span></span>                            | <span data-ttu-id="fb669-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb669-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fb669-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb669-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="fb669-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="fb669-116">Request parameters</span></span>

<span data-ttu-id="fb669-117">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fb669-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fb669-118">参数</span><span class="sxs-lookup"><span data-stu-id="fb669-118">Parameter</span></span> | <span data-ttu-id="fb669-119">类型</span><span class="sxs-lookup"><span data-stu-id="fb669-119">Type</span></span>   | <span data-ttu-id="fb669-120">说明</span><span class="sxs-lookup"><span data-stu-id="fb669-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fb669-121">period</span><span class="sxs-lookup"><span data-stu-id="fb669-121">period</span></span>    | <span data-ttu-id="fb669-122">string</span><span class="sxs-lookup"><span data-stu-id="fb669-122">string</span></span> | <span data-ttu-id="fb669-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fb669-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fb669-124">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fb669-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fb669-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fb669-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fb669-126">必需。</span><span class="sxs-lookup"><span data-stu-id="fb669-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fb669-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb669-127">Request headers</span></span>

| <span data-ttu-id="fb669-128">名称</span><span class="sxs-lookup"><span data-stu-id="fb669-128">Name</span></span>          | <span data-ttu-id="fb669-129">说明</span><span class="sxs-lookup"><span data-stu-id="fb669-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fb669-130">授权</span><span class="sxs-lookup"><span data-stu-id="fb669-130">Authorization</span></span> | <span data-ttu-id="fb669-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb669-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fb669-133">响应</span><span class="sxs-lookup"><span data-stu-id="fb669-133">Response</span></span>

<span data-ttu-id="fb669-134">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fb669-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fb669-135">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fb669-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fb669-136">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fb669-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fb669-137">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fb669-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fb669-138">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fb669-138">Report Refresh Date</span></span>
- <span data-ttu-id="fb669-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="fb669-139">Office 365</span></span>
- <span data-ttu-id="fb669-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="fb669-140">Exchange</span></span>
- <span data-ttu-id="fb669-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="fb669-141">OneDrive</span></span>
- <span data-ttu-id="fb669-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb669-142">SharePoint</span></span>
- <span data-ttu-id="fb669-143">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="fb669-143">Skype For Business</span></span> 
- <span data-ttu-id="fb669-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="fb669-144">Yammer</span></span>
- <span data-ttu-id="fb669-145">Teams</span><span class="sxs-lookup"><span data-stu-id="fb669-145">Teams</span></span>
- <span data-ttu-id="fb669-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="fb669-146">Report Date</span></span>
- <span data-ttu-id="fb669-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="fb669-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fb669-148">示例</span><span class="sxs-lookup"><span data-stu-id="fb669-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fb669-149">请求</span><span class="sxs-lookup"><span data-stu-id="fb669-149">Request</span></span>

<span data-ttu-id="fb669-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb669-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fb669-151">响应</span><span class="sxs-lookup"><span data-stu-id="fb669-151">Response</span></span>

<span data-ttu-id="fb669-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb669-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="fb669-153">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fb669-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
