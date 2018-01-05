# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="89476-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="89476-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="89476-102">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="89476-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="89476-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60))。</span><span class="sxs-lookup"><span data-stu-id="89476-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)).</span></span>

## <a name="permissions"></a><span data-ttu-id="89476-104">权限</span><span class="sxs-lookup"><span data-stu-id="89476-104">Permissions</span></span>

<span data-ttu-id="89476-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="89476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="89476-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="89476-107">Permission type</span></span>                        | <span data-ttu-id="89476-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89476-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="89476-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89476-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="89476-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="89476-110">Not supported.</span></span>                           |
| <span data-ttu-id="89476-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89476-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89476-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="89476-112">Not supported.</span></span>                           |
| <span data-ttu-id="89476-113">应用</span><span class="sxs-lookup"><span data-stu-id="89476-113">Application</span></span>                            | <span data-ttu-id="89476-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89476-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="89476-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89476-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="89476-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="89476-116">Request headers</span></span>

| <span data-ttu-id="89476-117">名称</span><span class="sxs-lookup"><span data-stu-id="89476-117">Name</span></span>          | <span data-ttu-id="89476-118">说明</span><span class="sxs-lookup"><span data-stu-id="89476-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="89476-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="89476-119">Authorization</span></span> | <span data-ttu-id="89476-p102">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="89476-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="89476-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="89476-122">if-none-match</span></span> | <span data-ttu-id="89476-123">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="89476-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="89476-124">可选。</span><span class="sxs-lookup"><span data-stu-id="89476-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="89476-125">响应</span><span class="sxs-lookup"><span data-stu-id="89476-125">Response</span></span>

<span data-ttu-id="89476-126">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="89476-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="89476-127">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="89476-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="89476-128">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="89476-128">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="89476-129">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="89476-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="89476-130">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="89476-130">Report Refresh Date</span></span>
- <span data-ttu-id="89476-131">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="89476-131">User Principal Name</span></span>
- <span data-ttu-id="89476-132">显示名称</span><span class="sxs-lookup"><span data-stu-id="89476-132">Display Name</span></span>
- <span data-ttu-id="89476-133">产品类型</span><span class="sxs-lookup"><span data-stu-id="89476-133">Product External Content Type</span></span>
- <span data-ttu-id="89476-134">上次激活日期</span><span class="sxs-lookup"><span data-stu-id="89476-134">Last Activated Date</span></span>
- <span data-ttu-id="89476-135">Windows</span><span class="sxs-lookup"><span data-stu-id="89476-135">Windows</span></span>
- <span data-ttu-id="89476-136">Mac</span><span class="sxs-lookup"><span data-stu-id="89476-136">"mac"</span></span>
- <span data-ttu-id="89476-137">Windows 10 移动版</span><span class="sxs-lookup"><span data-stu-id="89476-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="89476-138">iOS</span><span class="sxs-lookup"><span data-stu-id="89476-138">iOS</span></span>
- <span data-ttu-id="89476-139">Android</span><span class="sxs-lookup"><span data-stu-id="89476-139">Android</span></span>

## <a name="example"></a><span data-ttu-id="89476-140">示例</span><span class="sxs-lookup"><span data-stu-id="89476-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="89476-141">请求</span><span class="sxs-lookup"><span data-stu-id="89476-141">Request</span></span>

<span data-ttu-id="89476-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89476-142">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="89476-143">响应</span><span class="sxs-lookup"><span data-stu-id="89476-143">Response</span></span>

<span data-ttu-id="89476-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89476-144">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="89476-145">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="89476-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android
```
