# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="6fbb1-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="6fbb1-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="6fbb1-102">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="6fbb1-103">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fbb1-104">权限</span><span class="sxs-lookup"><span data-stu-id="6fbb1-104">Permissions</span></span>

<span data-ttu-id="6fbb1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6fbb1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fbb1-107">Permission type</span></span>                        | <span data-ttu-id="6fbb1-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fbb1-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6fbb1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fbb1-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fbb1-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fbb1-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6fbb1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fbb1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fbb1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-112">Not supported.</span></span>                           |
| <span data-ttu-id="6fbb1-113">应用</span><span class="sxs-lookup"><span data-stu-id="6fbb1-113">Application</span></span>                            | <span data-ttu-id="6fbb1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fbb1-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6fbb1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fbb1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="6fbb1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fbb1-116">Request headers</span></span>

| <span data-ttu-id="6fbb1-117">名称</span><span class="sxs-lookup"><span data-stu-id="6fbb1-117">Name</span></span>          | <span data-ttu-id="6fbb1-118">说明</span><span class="sxs-lookup"><span data-stu-id="6fbb1-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6fbb1-119">授权</span><span class="sxs-lookup"><span data-stu-id="6fbb1-119">Authorization</span></span> | <span data-ttu-id="6fbb1-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6fbb1-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6fbb1-122">If-None-Match</span></span> | <span data-ttu-id="6fbb1-123">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6fbb1-124">可选。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6fbb1-125">响应</span><span class="sxs-lookup"><span data-stu-id="6fbb1-125">Response</span></span>

<span data-ttu-id="6fbb1-126">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6fbb1-127">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6fbb1-128">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6fbb1-129">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6fbb1-130">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6fbb1-130">Report Refresh Date</span></span>
- <span data-ttu-id="6fbb1-131">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6fbb1-131">User Principal Name</span></span>
- <span data-ttu-id="6fbb1-132">显示名称</span><span class="sxs-lookup"><span data-stu-id="6fbb1-132">Display Name</span></span>
- <span data-ttu-id="6fbb1-133">产品类型</span><span class="sxs-lookup"><span data-stu-id="6fbb1-133">Product Type</span></span>
- <span data-ttu-id="6fbb1-134">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="6fbb1-134">Last Activated Date</span></span>
- <span data-ttu-id="6fbb1-135">Windows</span><span class="sxs-lookup"><span data-stu-id="6fbb1-135">Windows</span></span>
- <span data-ttu-id="6fbb1-136">Mac</span><span class="sxs-lookup"><span data-stu-id="6fbb1-136">Mac</span></span>
- <span data-ttu-id="6fbb1-137">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="6fbb1-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="6fbb1-138">iOS</span><span class="sxs-lookup"><span data-stu-id="6fbb1-138">iOS</span></span>
- <span data-ttu-id="6fbb1-139">Android</span><span class="sxs-lookup"><span data-stu-id="6fbb1-139">Android</span></span>

## <a name="example"></a><span data-ttu-id="6fbb1-140">示例</span><span class="sxs-lookup"><span data-stu-id="6fbb1-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6fbb1-141">请求</span><span class="sxs-lookup"><span data-stu-id="6fbb1-141">Request</span></span>

<span data-ttu-id="6fbb1-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-142">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="6fbb1-143">响应</span><span class="sxs-lookup"><span data-stu-id="6fbb1-143">Response</span></span>

<span data-ttu-id="6fbb1-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-144">The following is an example of the response.</span></span>

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

<span data-ttu-id="6fbb1-145">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6fbb1-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android
```
