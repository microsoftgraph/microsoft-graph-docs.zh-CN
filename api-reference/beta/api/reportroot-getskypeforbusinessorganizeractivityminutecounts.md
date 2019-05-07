---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d60e367c3ce7d900aa1d45a4438aaae5b89514cc
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639196"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="d3153-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="d3153-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3153-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="d3153-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="d3153-106">会议会话类型包括音频/视频和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="d3153-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="d3153-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="d3153-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3153-108">权限</span><span class="sxs-lookup"><span data-stu-id="d3153-108">Permissions</span></span>

<span data-ttu-id="d3153-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3153-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3153-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3153-111">Permission type</span></span>                        | <span data-ttu-id="d3153-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3153-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d3153-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3153-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3153-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3153-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d3153-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3153-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3153-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3153-116">Not supported.</span></span>                           |
| <span data-ttu-id="d3153-117">应用</span><span class="sxs-lookup"><span data-stu-id="d3153-117">Application</span></span>                            | <span data-ttu-id="d3153-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3153-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d3153-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3153-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d3153-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d3153-120">Function parameters</span></span>

<span data-ttu-id="d3153-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d3153-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d3153-122">参数</span><span class="sxs-lookup"><span data-stu-id="d3153-122">Parameter</span></span> | <span data-ttu-id="d3153-123">类型</span><span class="sxs-lookup"><span data-stu-id="d3153-123">Type</span></span>   | <span data-ttu-id="d3153-124">说明</span><span class="sxs-lookup"><span data-stu-id="d3153-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d3153-125">period</span><span class="sxs-lookup"><span data-stu-id="d3153-125">period</span></span>    | <span data-ttu-id="d3153-126">string</span><span class="sxs-lookup"><span data-stu-id="d3153-126">string</span></span> | <span data-ttu-id="d3153-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d3153-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d3153-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d3153-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d3153-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d3153-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d3153-130">必需。</span><span class="sxs-lookup"><span data-stu-id="d3153-130">Required.</span></span> |

<span data-ttu-id="d3153-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3153-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d3153-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d3153-132">The default output type is text/csv.</span></span> <span data-ttu-id="d3153-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d3153-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3153-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3153-134">Request headers</span></span>

| <span data-ttu-id="d3153-135">名称</span><span class="sxs-lookup"><span data-stu-id="d3153-135">Name</span></span>          | <span data-ttu-id="d3153-136">说明</span><span class="sxs-lookup"><span data-stu-id="d3153-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d3153-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3153-137">Authorization</span></span> | <span data-ttu-id="d3153-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3153-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d3153-140">响应</span><span class="sxs-lookup"><span data-stu-id="d3153-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d3153-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d3153-141">CSV</span></span>

<span data-ttu-id="d3153-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d3153-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d3153-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d3153-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d3153-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d3153-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d3153-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d3153-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d3153-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d3153-146">Report Refresh Date</span></span>
- <span data-ttu-id="d3153-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="d3153-147">Report Date</span></span>
- <span data-ttu-id="d3153-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="d3153-148">Report Period</span></span>
- <span data-ttu-id="d3153-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="d3153-149">Audio/Video</span></span>
- <span data-ttu-id="d3153-150">Microsoft 拨入</span><span class="sxs-lookup"><span data-stu-id="d3153-150">Dial-in Microsoft</span></span>
- <span data-ttu-id="d3153-151">Microsoft 拨出</span><span class="sxs-lookup"><span data-stu-id="d3153-151">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="d3153-152">JSON</span><span class="sxs-lookup"><span data-stu-id="d3153-152">JSON</span></span>

<span data-ttu-id="d3153-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d3153-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3153-154">示例</span><span class="sxs-lookup"><span data-stu-id="d3153-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d3153-155">CSV</span><span class="sxs-lookup"><span data-stu-id="d3153-155">CSV</span></span>

<span data-ttu-id="d3153-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d3153-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d3153-157">请求</span><span class="sxs-lookup"><span data-stu-id="d3153-157">Request</span></span>

<span data-ttu-id="d3153-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3153-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d3153-159">响应</span><span class="sxs-lookup"><span data-stu-id="d3153-159">Response</span></span>

<span data-ttu-id="d3153-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d3153-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3153-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d3153-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3153-162">语言</span><span class="sxs-lookup"><span data-stu-id="d3153-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3153-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3153-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d3153-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d3153-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="d3153-165">JSON</span><span class="sxs-lookup"><span data-stu-id="d3153-165">JSON</span></span>

<span data-ttu-id="d3153-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d3153-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d3153-167">请求</span><span class="sxs-lookup"><span data-stu-id="d3153-167">Request</span></span>

<span data-ttu-id="d3153-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3153-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d3153-169">响应</span><span class="sxs-lookup"><span data-stu-id="d3153-169">Response</span></span>

<span data-ttu-id="d3153-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3153-170">The following is an example of the response.</span></span>

> <span data-ttu-id="d3153-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3153-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3153-173">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d3153-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3153-174">语言</span><span class="sxs-lookup"><span data-stu-id="d3153-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3153-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3153-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityminutecounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
