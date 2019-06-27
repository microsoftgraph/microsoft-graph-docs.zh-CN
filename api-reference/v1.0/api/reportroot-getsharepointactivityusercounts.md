---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c64a87e51bd3f3ee140aa5e125f38be3c3594a80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273351"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="6cf13-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6cf13-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="6cf13-105">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="6cf13-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="6cf13-106">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="6cf13-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="6cf13-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="6cf13-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf13-108">权限</span><span class="sxs-lookup"><span data-stu-id="6cf13-108">Permissions</span></span>

<span data-ttu-id="6cf13-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cf13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cf13-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cf13-111">Permission type</span></span>                        | <span data-ttu-id="6cf13-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cf13-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6cf13-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf13-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cf13-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cf13-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6cf13-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cf13-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cf13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cf13-116">Not supported.</span></span>                           |
| <span data-ttu-id="6cf13-117">应用</span><span class="sxs-lookup"><span data-stu-id="6cf13-117">Application</span></span>                            | <span data-ttu-id="6cf13-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cf13-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6cf13-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cf13-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6cf13-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="6cf13-120">Function parameters</span></span>

<span data-ttu-id="6cf13-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6cf13-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6cf13-122">参数</span><span class="sxs-lookup"><span data-stu-id="6cf13-122">Parameter</span></span> | <span data-ttu-id="6cf13-123">类型</span><span class="sxs-lookup"><span data-stu-id="6cf13-123">Type</span></span>   | <span data-ttu-id="6cf13-124">说明</span><span class="sxs-lookup"><span data-stu-id="6cf13-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6cf13-125">period</span><span class="sxs-lookup"><span data-stu-id="6cf13-125">period</span></span>    | <span data-ttu-id="6cf13-126">string</span><span class="sxs-lookup"><span data-stu-id="6cf13-126">string</span></span> | <span data-ttu-id="6cf13-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6cf13-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6cf13-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6cf13-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6cf13-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6cf13-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6cf13-130">必需。</span><span class="sxs-lookup"><span data-stu-id="6cf13-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6cf13-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cf13-131">Request headers</span></span>

| <span data-ttu-id="6cf13-132">名称</span><span class="sxs-lookup"><span data-stu-id="6cf13-132">Name</span></span>          | <span data-ttu-id="6cf13-133">说明</span><span class="sxs-lookup"><span data-stu-id="6cf13-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6cf13-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cf13-134">Authorization</span></span> | <span data-ttu-id="6cf13-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cf13-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6cf13-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6cf13-137">If-None-Match</span></span> | <span data-ttu-id="6cf13-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cf13-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6cf13-139">可选。</span><span class="sxs-lookup"><span data-stu-id="6cf13-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6cf13-140">响应</span><span class="sxs-lookup"><span data-stu-id="6cf13-140">Response</span></span>

<span data-ttu-id="6cf13-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6cf13-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6cf13-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6cf13-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6cf13-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6cf13-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6cf13-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6cf13-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6cf13-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6cf13-145">Report Refresh Date</span></span>
- <span data-ttu-id="6cf13-146">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="6cf13-146">Visited Page</span></span>
- <span data-ttu-id="6cf13-147">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="6cf13-147">Viewed Or Edited</span></span>
- <span data-ttu-id="6cf13-148">已同步</span><span class="sxs-lookup"><span data-stu-id="6cf13-148">Synced</span></span>
- <span data-ttu-id="6cf13-149">已内部共享</span><span class="sxs-lookup"><span data-stu-id="6cf13-149">Shared Internally</span></span>
- <span data-ttu-id="6cf13-150">已外部共享</span><span class="sxs-lookup"><span data-stu-id="6cf13-150">Shared Externally</span></span>
- <span data-ttu-id="6cf13-151">报表日期</span><span class="sxs-lookup"><span data-stu-id="6cf13-151">Report Date</span></span>
- <span data-ttu-id="6cf13-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="6cf13-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6cf13-153">示例</span><span class="sxs-lookup"><span data-stu-id="6cf13-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6cf13-154">请求</span><span class="sxs-lookup"><span data-stu-id="6cf13-154">Request</span></span>

<span data-ttu-id="6cf13-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cf13-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6cf13-156">响应</span><span class="sxs-lookup"><span data-stu-id="6cf13-156">Response</span></span>

<span data-ttu-id="6cf13-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6cf13-157">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6cf13-158">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6cf13-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6cf13-159">C#</span><span class="sxs-lookup"><span data-stu-id="6cf13-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cf13-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="6cf13-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6cf13-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="6cf13-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6cf13-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6cf13-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
