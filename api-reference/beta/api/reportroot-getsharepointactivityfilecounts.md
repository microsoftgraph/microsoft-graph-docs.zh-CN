---
title: 'reportRoot: getSharePointActivityFileCounts'
description: 获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e28cc85dfb20f7255a792121208129e4a571834d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265287"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="d6565-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d6565-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6565-104">获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="d6565-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="d6565-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="d6565-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6565-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6565-106">Permissions</span></span>

<span data-ttu-id="d6565-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6565-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6565-109">Permission type</span></span>                        | <span data-ttu-id="d6565-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6565-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d6565-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6565-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6565-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6565-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d6565-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6565-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6565-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6565-114">Not supported.</span></span>                           |
| <span data-ttu-id="d6565-115">应用</span><span class="sxs-lookup"><span data-stu-id="d6565-115">Application</span></span>                            | <span data-ttu-id="d6565-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6565-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d6565-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6565-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d6565-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="d6565-118">Function parameters</span></span>

<span data-ttu-id="d6565-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d6565-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d6565-120">参数</span><span class="sxs-lookup"><span data-stu-id="d6565-120">Parameter</span></span> | <span data-ttu-id="d6565-121">类型</span><span class="sxs-lookup"><span data-stu-id="d6565-121">Type</span></span>   | <span data-ttu-id="d6565-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6565-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d6565-123">period</span><span class="sxs-lookup"><span data-stu-id="d6565-123">period</span></span>    | <span data-ttu-id="d6565-124">string</span><span class="sxs-lookup"><span data-stu-id="d6565-124">string</span></span> | <span data-ttu-id="d6565-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d6565-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d6565-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d6565-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d6565-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d6565-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d6565-128">必需。</span><span class="sxs-lookup"><span data-stu-id="d6565-128">Required.</span></span> |

<span data-ttu-id="d6565-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6565-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d6565-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d6565-130">The default output type is text/csv.</span></span> <span data-ttu-id="d6565-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d6565-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6565-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6565-132">Request headers</span></span>

| <span data-ttu-id="d6565-133">名称</span><span class="sxs-lookup"><span data-stu-id="d6565-133">Name</span></span>          | <span data-ttu-id="d6565-134">说明</span><span class="sxs-lookup"><span data-stu-id="d6565-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d6565-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6565-135">Authorization</span></span> | <span data-ttu-id="d6565-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6565-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d6565-138">响应</span><span class="sxs-lookup"><span data-stu-id="d6565-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d6565-139">CSV</span><span class="sxs-lookup"><span data-stu-id="d6565-139">CSV</span></span>

<span data-ttu-id="d6565-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d6565-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d6565-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d6565-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d6565-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d6565-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d6565-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d6565-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d6565-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d6565-144">Report Refresh Date</span></span>
- <span data-ttu-id="d6565-145">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="d6565-145">Viewed Or Edited</span></span>
- <span data-ttu-id="d6565-146">已同步</span><span class="sxs-lookup"><span data-stu-id="d6565-146">Synced</span></span>
- <span data-ttu-id="d6565-147">已内部共享</span><span class="sxs-lookup"><span data-stu-id="d6565-147">Shared Internally</span></span>
- <span data-ttu-id="d6565-148">已外部共享</span><span class="sxs-lookup"><span data-stu-id="d6565-148">Shared Externally</span></span>
- <span data-ttu-id="d6565-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="d6565-149">Report Date</span></span>
- <span data-ttu-id="d6565-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="d6565-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d6565-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d6565-151">JSON</span></span>

<span data-ttu-id="d6565-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[siteActivitySummary](../resources/siteactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d6565-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6565-153">示例</span><span class="sxs-lookup"><span data-stu-id="d6565-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d6565-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d6565-154">CSV</span></span>

<span data-ttu-id="d6565-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d6565-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d6565-156">请求</span><span class="sxs-lookup"><span data-stu-id="d6565-156">Request</span></span>

<span data-ttu-id="d6565-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6565-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d6565-158">响应</span><span class="sxs-lookup"><span data-stu-id="d6565-158">Response</span></span>

<span data-ttu-id="d6565-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6565-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6565-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d6565-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6565-161">C#</span><span class="sxs-lookup"><span data-stu-id="d6565-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6565-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6565-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d6565-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="d6565-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d6565-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d6565-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="d6565-165">JSON</span><span class="sxs-lookup"><span data-stu-id="d6565-165">JSON</span></span>

<span data-ttu-id="d6565-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d6565-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d6565-167">请求</span><span class="sxs-lookup"><span data-stu-id="d6565-167">Request</span></span>

<span data-ttu-id="d6565-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6565-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d6565-169">响应</span><span class="sxs-lookup"><span data-stu-id="d6565-169">Response</span></span>

<span data-ttu-id="d6565-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d6565-170">The following is an example of the response.</span></span>

> <span data-ttu-id="d6565-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d6565-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d6565-173">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d6565-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d6565-174">C#</span><span class="sxs-lookup"><span data-stu-id="d6565-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6565-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6565-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d6565-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="d6565-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
