---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: 获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c32e4c280cad6f52eba72a0dacaf98638219c55b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268668"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="e8a32-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e8a32-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="e8a32-104">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="e8a32-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="e8a32-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="e8a32-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a32-106">权限</span><span class="sxs-lookup"><span data-stu-id="e8a32-106">Permissions</span></span>

<span data-ttu-id="e8a32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8a32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8a32-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8a32-109">Permission type</span></span>                        | <span data-ttu-id="e8a32-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8a32-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e8a32-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8a32-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8a32-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e8a32-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8a32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a32-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8a32-114">Not supported.</span></span>                           |
| <span data-ttu-id="e8a32-115">应用</span><span class="sxs-lookup"><span data-stu-id="e8a32-115">Application</span></span>                            | <span data-ttu-id="e8a32-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8a32-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e8a32-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8a32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e8a32-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="e8a32-118">Function parameters</span></span>

<span data-ttu-id="e8a32-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e8a32-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e8a32-120">参数</span><span class="sxs-lookup"><span data-stu-id="e8a32-120">Parameter</span></span> | <span data-ttu-id="e8a32-121">类型</span><span class="sxs-lookup"><span data-stu-id="e8a32-121">Type</span></span>   | <span data-ttu-id="e8a32-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8a32-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e8a32-123">period</span><span class="sxs-lookup"><span data-stu-id="e8a32-123">period</span></span>    | <span data-ttu-id="e8a32-124">string</span><span class="sxs-lookup"><span data-stu-id="e8a32-124">string</span></span> | <span data-ttu-id="e8a32-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e8a32-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e8a32-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e8a32-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e8a32-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e8a32-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e8a32-128">必需。</span><span class="sxs-lookup"><span data-stu-id="e8a32-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e8a32-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8a32-129">Request headers</span></span>

| <span data-ttu-id="e8a32-130">名称</span><span class="sxs-lookup"><span data-stu-id="e8a32-130">Name</span></span>          | <span data-ttu-id="e8a32-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8a32-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e8a32-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a32-132">Authorization</span></span> | <span data-ttu-id="e8a32-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8a32-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e8a32-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e8a32-135">If-None-Match</span></span> | <span data-ttu-id="e8a32-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8a32-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e8a32-137">可选。</span><span class="sxs-lookup"><span data-stu-id="e8a32-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e8a32-138">响应</span><span class="sxs-lookup"><span data-stu-id="e8a32-138">Response</span></span>

<span data-ttu-id="e8a32-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e8a32-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e8a32-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e8a32-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e8a32-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e8a32-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e8a32-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e8a32-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e8a32-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e8a32-143">Report Refresh Date</span></span>
- <span data-ttu-id="e8a32-144">总计</span><span class="sxs-lookup"><span data-stu-id="e8a32-144">Total</span></span>
- <span data-ttu-id="e8a32-145">活跃</span><span class="sxs-lookup"><span data-stu-id="e8a32-145">Active</span></span>
- <span data-ttu-id="e8a32-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="e8a32-146">Report Date</span></span>
- <span data-ttu-id="e8a32-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="e8a32-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e8a32-148">示例</span><span class="sxs-lookup"><span data-stu-id="e8a32-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e8a32-149">请求</span><span class="sxs-lookup"><span data-stu-id="e8a32-149">Request</span></span>

<span data-ttu-id="e8a32-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8a32-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e8a32-151">响应</span><span class="sxs-lookup"><span data-stu-id="e8a32-151">Response</span></span>

<span data-ttu-id="e8a32-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8a32-152">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8a32-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e8a32-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8a32-154">C#</span><span class="sxs-lookup"><span data-stu-id="e8a32-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityfilecounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8a32-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8a32-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityfilecounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8a32-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8a32-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityfilecounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e8a32-157">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e8a32-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
