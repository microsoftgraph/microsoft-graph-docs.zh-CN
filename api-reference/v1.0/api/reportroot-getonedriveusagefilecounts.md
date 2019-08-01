---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0aca7eec4c4991484a3ec4ab6a3a301b704e2144
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021906"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="f463b-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="f463b-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="f463b-105">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="f463b-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="f463b-106">如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。</span><span class="sxs-lookup"><span data-stu-id="f463b-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="f463b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="f463b-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="f463b-108">权限</span><span class="sxs-lookup"><span data-stu-id="f463b-108">Permissions</span></span>

<span data-ttu-id="f463b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f463b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f463b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f463b-111">Permission type</span></span>                        | <span data-ttu-id="f463b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f463b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f463b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f463b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f463b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f463b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f463b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f463b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f463b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f463b-116">Not supported.</span></span>                           |
| <span data-ttu-id="f463b-117">应用</span><span class="sxs-lookup"><span data-stu-id="f463b-117">Application</span></span>                            | <span data-ttu-id="f463b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f463b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f463b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f463b-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f463b-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f463b-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f463b-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="f463b-121">Function parameters</span></span>

<span data-ttu-id="f463b-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f463b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f463b-123">参数</span><span class="sxs-lookup"><span data-stu-id="f463b-123">Parameter</span></span> | <span data-ttu-id="f463b-124">类型</span><span class="sxs-lookup"><span data-stu-id="f463b-124">Type</span></span>   | <span data-ttu-id="f463b-125">说明</span><span class="sxs-lookup"><span data-stu-id="f463b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f463b-126">period</span><span class="sxs-lookup"><span data-stu-id="f463b-126">period</span></span>    | <span data-ttu-id="f463b-127">string</span><span class="sxs-lookup"><span data-stu-id="f463b-127">string</span></span> | <span data-ttu-id="f463b-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f463b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f463b-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f463b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f463b-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f463b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f463b-131">必需。</span><span class="sxs-lookup"><span data-stu-id="f463b-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f463b-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f463b-132">Request headers</span></span>

| <span data-ttu-id="f463b-133">名称</span><span class="sxs-lookup"><span data-stu-id="f463b-133">Name</span></span>          | <span data-ttu-id="f463b-134">说明</span><span class="sxs-lookup"><span data-stu-id="f463b-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f463b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f463b-135">Authorization</span></span> | <span data-ttu-id="f463b-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="f463b-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f463b-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f463b-138">If-None-Match</span></span> | <span data-ttu-id="f463b-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f463b-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f463b-140">可选。</span><span class="sxs-lookup"><span data-stu-id="f463b-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f463b-141">响应</span><span class="sxs-lookup"><span data-stu-id="f463b-141">Response</span></span>

<span data-ttu-id="f463b-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f463b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f463b-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f463b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f463b-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f463b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f463b-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f463b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f463b-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f463b-146">Report Refresh Date</span></span>
- <span data-ttu-id="f463b-147">网站类型</span><span class="sxs-lookup"><span data-stu-id="f463b-147">Site Type</span></span>
- <span data-ttu-id="f463b-148">总计</span><span class="sxs-lookup"><span data-stu-id="f463b-148">Total</span></span>
- <span data-ttu-id="f463b-149">活跃</span><span class="sxs-lookup"><span data-stu-id="f463b-149">Active</span></span>
- <span data-ttu-id="f463b-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="f463b-150">Report Date</span></span>
- <span data-ttu-id="f463b-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="f463b-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f463b-152">示例</span><span class="sxs-lookup"><span data-stu-id="f463b-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f463b-153">请求</span><span class="sxs-lookup"><span data-stu-id="f463b-153">Request</span></span>

<span data-ttu-id="f463b-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f463b-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f463b-155">C#</span><span class="sxs-lookup"><span data-stu-id="f463b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f463b-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="f463b-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f463b-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="f463b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f463b-158">Java</span><span class="sxs-lookup"><span data-stu-id="f463b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagefilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f463b-159">响应</span><span class="sxs-lookup"><span data-stu-id="f463b-159">Response</span></span>

<span data-ttu-id="f463b-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f463b-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="f463b-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f463b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
