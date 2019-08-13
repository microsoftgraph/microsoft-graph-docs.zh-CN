---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: 获取报表周期内分配和使用的存储趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9db656c2e042b213b10ea2f157bc531d0f6e6264
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349355"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="32d24-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="32d24-103">reportRoot: getSharePointSiteUsageStorage</span></span>

<span data-ttu-id="32d24-104">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="32d24-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="32d24-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="32d24-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="32d24-106">权限</span><span class="sxs-lookup"><span data-stu-id="32d24-106">Permissions</span></span>

<span data-ttu-id="32d24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32d24-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32d24-109">Permission type</span></span>                        | <span data-ttu-id="32d24-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32d24-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32d24-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32d24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32d24-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32d24-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32d24-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32d24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d24-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="32d24-114">Not supported.</span></span>                           |
| <span data-ttu-id="32d24-115">应用</span><span class="sxs-lookup"><span data-stu-id="32d24-115">Application</span></span>                            | <span data-ttu-id="32d24-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32d24-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32d24-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32d24-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="32d24-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="32d24-118">Function parameters</span></span>

<span data-ttu-id="32d24-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="32d24-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="32d24-120">参数</span><span class="sxs-lookup"><span data-stu-id="32d24-120">Parameter</span></span> | <span data-ttu-id="32d24-121">类型</span><span class="sxs-lookup"><span data-stu-id="32d24-121">Type</span></span>   | <span data-ttu-id="32d24-122">说明</span><span class="sxs-lookup"><span data-stu-id="32d24-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="32d24-123">period</span><span class="sxs-lookup"><span data-stu-id="32d24-123">period</span></span>    | <span data-ttu-id="32d24-124">string</span><span class="sxs-lookup"><span data-stu-id="32d24-124">string</span></span> | <span data-ttu-id="32d24-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="32d24-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="32d24-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="32d24-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="32d24-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="32d24-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="32d24-128">必需。</span><span class="sxs-lookup"><span data-stu-id="32d24-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="32d24-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="32d24-129">Request headers</span></span>

| <span data-ttu-id="32d24-130">名称</span><span class="sxs-lookup"><span data-stu-id="32d24-130">Name</span></span>          | <span data-ttu-id="32d24-131">说明</span><span class="sxs-lookup"><span data-stu-id="32d24-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="32d24-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="32d24-132">Authorization</span></span> | <span data-ttu-id="32d24-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="32d24-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="32d24-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="32d24-135">If-None-Match</span></span> | <span data-ttu-id="32d24-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="32d24-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="32d24-137">可选。</span><span class="sxs-lookup"><span data-stu-id="32d24-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="32d24-138">响应</span><span class="sxs-lookup"><span data-stu-id="32d24-138">Response</span></span>

<span data-ttu-id="32d24-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="32d24-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32d24-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="32d24-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32d24-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="32d24-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32d24-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="32d24-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="32d24-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="32d24-143">Report Refresh Date</span></span>
- <span data-ttu-id="32d24-144">网站类型</span><span class="sxs-lookup"><span data-stu-id="32d24-144">Site Type</span></span>
- <span data-ttu-id="32d24-145">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="32d24-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="32d24-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="32d24-146">Report Date</span></span>
- <span data-ttu-id="32d24-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="32d24-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="32d24-148">示例</span><span class="sxs-lookup"><span data-stu-id="32d24-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32d24-149">请求</span><span class="sxs-lookup"><span data-stu-id="32d24-149">Request</span></span>

<span data-ttu-id="32d24-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32d24-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32d24-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="32d24-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageStorage(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32d24-152">C#</span><span class="sxs-lookup"><span data-stu-id="32d24-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32d24-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32d24-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32d24-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="32d24-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32d24-155">Java</span><span class="sxs-lookup"><span data-stu-id="32d24-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagestorage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32d24-156">响应</span><span class="sxs-lookup"><span data-stu-id="32d24-156">Response</span></span>

<span data-ttu-id="32d24-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32d24-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="32d24-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="32d24-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
