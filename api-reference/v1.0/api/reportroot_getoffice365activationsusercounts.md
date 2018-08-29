# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="6ee8d-101">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="6ee8d-101">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="6ee8d-102">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-102">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span>

> <span data-ttu-id="6ee8d-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ee8d-104">权限</span><span class="sxs-lookup"><span data-stu-id="6ee8d-104">Permissions</span></span>

<span data-ttu-id="6ee8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6ee8d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ee8d-107">Permission type</span></span>                        | <span data-ttu-id="6ee8d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ee8d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6ee8d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ee8d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ee8d-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ee8d-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6ee8d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ee8d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ee8d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-112">Not supported.</span></span>                           |
| <span data-ttu-id="6ee8d-113">应用</span><span class="sxs-lookup"><span data-stu-id="6ee8d-113">Application</span></span>                            | <span data-ttu-id="6ee8d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ee8d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6ee8d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ee8d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="6ee8d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ee8d-116">Request headers</span></span>

| <span data-ttu-id="6ee8d-117">名称</span><span class="sxs-lookup"><span data-stu-id="6ee8d-117">Name</span></span>          | <span data-ttu-id="6ee8d-118">说明</span><span class="sxs-lookup"><span data-stu-id="6ee8d-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6ee8d-119">授权</span><span class="sxs-lookup"><span data-stu-id="6ee8d-119">Authorization</span></span> | <span data-ttu-id="6ee8d-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6ee8d-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6ee8d-122">If-None-Match</span></span> | <span data-ttu-id="6ee8d-123">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6ee8d-124">可选。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6ee8d-125">响应</span><span class="sxs-lookup"><span data-stu-id="6ee8d-125">Response</span></span>

<span data-ttu-id="6ee8d-126">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6ee8d-127">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6ee8d-128">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6ee8d-129">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6ee8d-130">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6ee8d-130">Report Refresh Date</span></span>
- <span data-ttu-id="6ee8d-131">产品类型</span><span class="sxs-lookup"><span data-stu-id="6ee8d-131">Product Type</span></span>
- <span data-ttu-id="6ee8d-132">已分配</span><span class="sxs-lookup"><span data-stu-id="6ee8d-132">Assigned</span></span>
- <span data-ttu-id="6ee8d-133">已激活</span><span class="sxs-lookup"><span data-stu-id="6ee8d-133">Activated</span></span>

## <a name="example"></a><span data-ttu-id="6ee8d-134">示例</span><span class="sxs-lookup"><span data-stu-id="6ee8d-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6ee8d-135">请求</span><span class="sxs-lookup"><span data-stu-id="6ee8d-135">Request</span></span>

<span data-ttu-id="6ee8d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-136">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="6ee8d-137">响应</span><span class="sxs-lookup"><span data-stu-id="6ee8d-137">Response</span></span>

<span data-ttu-id="6ee8d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-138">The following is an example of the response.</span></span>

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

<span data-ttu-id="6ee8d-139">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6ee8d-139">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated
```
