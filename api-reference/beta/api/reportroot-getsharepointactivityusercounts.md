---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: dfe07aa6e2f652b4158b76584f1053340d942bb6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265294"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="cf7df-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="cf7df-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf7df-105">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="cf7df-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="cf7df-106">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="cf7df-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="cf7df-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="cf7df-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf7df-108">权限</span><span class="sxs-lookup"><span data-stu-id="cf7df-108">Permissions</span></span>

<span data-ttu-id="cf7df-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf7df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf7df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf7df-111">Permission type</span></span>                        | <span data-ttu-id="cf7df-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf7df-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf7df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7df-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf7df-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf7df-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf7df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf7df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf7df-116">Not supported.</span></span>                           |
| <span data-ttu-id="cf7df-117">应用</span><span class="sxs-lookup"><span data-stu-id="cf7df-117">Application</span></span>                            | <span data-ttu-id="cf7df-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf7df-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cf7df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf7df-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cf7df-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="cf7df-120">Function parameters</span></span>

<span data-ttu-id="cf7df-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="cf7df-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cf7df-122">参数</span><span class="sxs-lookup"><span data-stu-id="cf7df-122">Parameter</span></span> | <span data-ttu-id="cf7df-123">类型</span><span class="sxs-lookup"><span data-stu-id="cf7df-123">Type</span></span>   | <span data-ttu-id="cf7df-124">说明</span><span class="sxs-lookup"><span data-stu-id="cf7df-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf7df-125">period</span><span class="sxs-lookup"><span data-stu-id="cf7df-125">period</span></span>    | <span data-ttu-id="cf7df-126">string</span><span class="sxs-lookup"><span data-stu-id="cf7df-126">string</span></span> | <span data-ttu-id="cf7df-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cf7df-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf7df-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cf7df-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf7df-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cf7df-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cf7df-130">必需。</span><span class="sxs-lookup"><span data-stu-id="cf7df-130">Required.</span></span> |

<span data-ttu-id="cf7df-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf7df-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cf7df-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="cf7df-132">The default output type is text/csv.</span></span> <span data-ttu-id="cf7df-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="cf7df-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf7df-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf7df-134">Request headers</span></span>

| <span data-ttu-id="cf7df-135">名称</span><span class="sxs-lookup"><span data-stu-id="cf7df-135">Name</span></span>          | <span data-ttu-id="cf7df-136">说明</span><span class="sxs-lookup"><span data-stu-id="cf7df-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf7df-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf7df-137">Authorization</span></span> | <span data-ttu-id="cf7df-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf7df-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf7df-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf7df-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cf7df-141">CSV</span><span class="sxs-lookup"><span data-stu-id="cf7df-141">CSV</span></span>

<span data-ttu-id="cf7df-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cf7df-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf7df-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cf7df-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf7df-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cf7df-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf7df-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cf7df-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cf7df-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cf7df-146">Report Refresh Date</span></span>
- <span data-ttu-id="cf7df-147">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="cf7df-147">Visited Page</span></span>
- <span data-ttu-id="cf7df-148">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="cf7df-148">Viewed Or Edited</span></span>
- <span data-ttu-id="cf7df-149">已同步</span><span class="sxs-lookup"><span data-stu-id="cf7df-149">Synced</span></span>
- <span data-ttu-id="cf7df-150">已内部共享</span><span class="sxs-lookup"><span data-stu-id="cf7df-150">Shared Internally</span></span>
- <span data-ttu-id="cf7df-151">已外部共享</span><span class="sxs-lookup"><span data-stu-id="cf7df-151">Shared Externally</span></span>
- <span data-ttu-id="cf7df-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="cf7df-152">Report Date</span></span>
- <span data-ttu-id="cf7df-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="cf7df-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cf7df-154">JSON</span><span class="sxs-lookup"><span data-stu-id="cf7df-154">JSON</span></span>

<span data-ttu-id="cf7df-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="cf7df-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7df-156">示例</span><span class="sxs-lookup"><span data-stu-id="cf7df-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cf7df-157">CSV</span><span class="sxs-lookup"><span data-stu-id="cf7df-157">CSV</span></span>

<span data-ttu-id="cf7df-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="cf7df-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cf7df-159">请求</span><span class="sxs-lookup"><span data-stu-id="cf7df-159">Request</span></span>

<span data-ttu-id="cf7df-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf7df-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cf7df-161">响应</span><span class="sxs-lookup"><span data-stu-id="cf7df-161">Response</span></span>

<span data-ttu-id="cf7df-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cf7df-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf7df-163">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cf7df-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf7df-164">C#</span><span class="sxs-lookup"><span data-stu-id="cf7df-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf7df-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf7df-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cf7df-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="cf7df-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="cf7df-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cf7df-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="cf7df-168">JSON</span><span class="sxs-lookup"><span data-stu-id="cf7df-168">JSON</span></span>

<span data-ttu-id="cf7df-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="cf7df-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cf7df-170">请求</span><span class="sxs-lookup"><span data-stu-id="cf7df-170">Request</span></span>

<span data-ttu-id="cf7df-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf7df-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cf7df-172">响应</span><span class="sxs-lookup"><span data-stu-id="cf7df-172">Response</span></span>

<span data-ttu-id="cf7df-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf7df-173">The following is an example of the response.</span></span>

> <span data-ttu-id="cf7df-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cf7df-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf7df-176">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cf7df-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf7df-177">C#</span><span class="sxs-lookup"><span data-stu-id="cf7df-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf7df-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf7df-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cf7df-179">目标-C</span><span class="sxs-lookup"><span data-stu-id="cf7df-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityusercounts_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
