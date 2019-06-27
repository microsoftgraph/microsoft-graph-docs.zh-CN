---
title: 'reportRoot: getYammerActivityCounts'
description: 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fc2f58f316bd3b06c6a9625e6e95399415a750c8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274688"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="4a405-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4a405-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="4a405-104">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="4a405-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="4a405-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="4a405-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a405-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a405-106">Permissions</span></span>

<span data-ttu-id="4a405-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a405-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a405-109">Permission type</span></span>                        | <span data-ttu-id="4a405-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a405-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a405-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a405-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a405-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a405-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a405-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a405-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a405-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a405-114">Not supported.</span></span>                           |
| <span data-ttu-id="4a405-115">应用</span><span class="sxs-lookup"><span data-stu-id="4a405-115">Application</span></span>                            | <span data-ttu-id="4a405-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a405-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a405-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a405-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a405-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="4a405-118">Function parameters</span></span>

<span data-ttu-id="4a405-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4a405-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a405-120">参数</span><span class="sxs-lookup"><span data-stu-id="4a405-120">Parameter</span></span> | <span data-ttu-id="4a405-121">类型</span><span class="sxs-lookup"><span data-stu-id="4a405-121">Type</span></span>   | <span data-ttu-id="4a405-122">说明</span><span class="sxs-lookup"><span data-stu-id="4a405-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a405-123">period</span><span class="sxs-lookup"><span data-stu-id="4a405-123">period</span></span>    | <span data-ttu-id="4a405-124">string</span><span class="sxs-lookup"><span data-stu-id="4a405-124">string</span></span> | <span data-ttu-id="4a405-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4a405-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a405-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4a405-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a405-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4a405-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a405-128">必需。</span><span class="sxs-lookup"><span data-stu-id="4a405-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4a405-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a405-129">Request headers</span></span>

| <span data-ttu-id="4a405-130">名称</span><span class="sxs-lookup"><span data-stu-id="4a405-130">Name</span></span>          | <span data-ttu-id="4a405-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a405-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4a405-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a405-132">Authorization</span></span> | <span data-ttu-id="4a405-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a405-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4a405-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4a405-135">If-None-Match</span></span> | <span data-ttu-id="4a405-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a405-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4a405-137">可选。</span><span class="sxs-lookup"><span data-stu-id="4a405-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4a405-138">响应</span><span class="sxs-lookup"><span data-stu-id="4a405-138">Response</span></span>

<span data-ttu-id="4a405-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4a405-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a405-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4a405-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a405-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4a405-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a405-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4a405-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a405-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4a405-143">Report Refresh Date</span></span>
- <span data-ttu-id="4a405-144">已赞</span><span class="sxs-lookup"><span data-stu-id="4a405-144">Liked</span></span>
- <span data-ttu-id="4a405-145">已发布</span><span class="sxs-lookup"><span data-stu-id="4a405-145">Posted</span></span>
- <span data-ttu-id="4a405-146">已阅读</span><span class="sxs-lookup"><span data-stu-id="4a405-146">Read</span></span>
- <span data-ttu-id="4a405-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="4a405-147">Report Date</span></span>
- <span data-ttu-id="4a405-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="4a405-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4a405-149">示例</span><span class="sxs-lookup"><span data-stu-id="4a405-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4a405-150">请求</span><span class="sxs-lookup"><span data-stu-id="4a405-150">Request</span></span>

<span data-ttu-id="4a405-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4a405-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4a405-152">响应</span><span class="sxs-lookup"><span data-stu-id="4a405-152">Response</span></span>

<span data-ttu-id="4a405-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4a405-153">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a405-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4a405-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a405-155">C#</span><span class="sxs-lookup"><span data-stu-id="4a405-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a405-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a405-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4a405-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="4a405-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="4a405-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4a405-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
