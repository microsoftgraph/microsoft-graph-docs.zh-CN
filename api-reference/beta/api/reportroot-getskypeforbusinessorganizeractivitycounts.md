---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0194df11740111d93c27929ccaecc550bbbc47c8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639206"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="5281c-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5281c-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5281c-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="5281c-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="5281c-106">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="5281c-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="5281c-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="5281c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="5281c-108">权限</span><span class="sxs-lookup"><span data-stu-id="5281c-108">Permissions</span></span>

<span data-ttu-id="5281c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5281c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5281c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5281c-111">Permission type</span></span>                        | <span data-ttu-id="5281c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5281c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5281c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5281c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5281c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5281c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5281c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5281c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5281c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5281c-116">Not supported.</span></span>                           |
| <span data-ttu-id="5281c-117">应用</span><span class="sxs-lookup"><span data-stu-id="5281c-117">Application</span></span>                            | <span data-ttu-id="5281c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5281c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5281c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5281c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5281c-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="5281c-120">Function parameters</span></span>

<span data-ttu-id="5281c-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5281c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5281c-122">参数</span><span class="sxs-lookup"><span data-stu-id="5281c-122">Parameter</span></span> | <span data-ttu-id="5281c-123">类型</span><span class="sxs-lookup"><span data-stu-id="5281c-123">Type</span></span>   | <span data-ttu-id="5281c-124">说明</span><span class="sxs-lookup"><span data-stu-id="5281c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5281c-125">period</span><span class="sxs-lookup"><span data-stu-id="5281c-125">period</span></span>    | <span data-ttu-id="5281c-126">string</span><span class="sxs-lookup"><span data-stu-id="5281c-126">string</span></span> | <span data-ttu-id="5281c-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5281c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5281c-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5281c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5281c-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5281c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5281c-130">必需。</span><span class="sxs-lookup"><span data-stu-id="5281c-130">Required.</span></span> |

<span data-ttu-id="5281c-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5281c-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5281c-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="5281c-132">The default output type is text/csv.</span></span> <span data-ttu-id="5281c-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="5281c-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5281c-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="5281c-134">Request headers</span></span>

| <span data-ttu-id="5281c-135">名称</span><span class="sxs-lookup"><span data-stu-id="5281c-135">Name</span></span>          | <span data-ttu-id="5281c-136">说明</span><span class="sxs-lookup"><span data-stu-id="5281c-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5281c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5281c-137">Authorization</span></span> | <span data-ttu-id="5281c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5281c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5281c-140">响应</span><span class="sxs-lookup"><span data-stu-id="5281c-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5281c-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5281c-141">CSV</span></span>

<span data-ttu-id="5281c-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5281c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5281c-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5281c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5281c-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5281c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5281c-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5281c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5281c-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5281c-146">Report Refresh Date</span></span>
- <span data-ttu-id="5281c-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="5281c-147">Report Date</span></span>
- <span data-ttu-id="5281c-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="5281c-148">Report Period</span></span>
- <span data-ttu-id="5281c-149">IM</span><span class="sxs-lookup"><span data-stu-id="5281c-149">IM</span></span>
- <span data-ttu-id="5281c-150">音频/视频</span><span class="sxs-lookup"><span data-stu-id="5281c-150">Audio/Video</span></span>
- <span data-ttu-id="5281c-151">应用共享</span><span class="sxs-lookup"><span data-stu-id="5281c-151">App Sharing</span></span>
- <span data-ttu-id="5281c-152">Web</span><span class="sxs-lookup"><span data-stu-id="5281c-152">Web</span></span>
- <span data-ttu-id="5281c-153">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="5281c-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="5281c-154">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="5281c-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="5281c-155">JSON</span><span class="sxs-lookup"><span data-stu-id="5281c-155">JSON</span></span>

<span data-ttu-id="5281c-156">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="5281c-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5281c-157">示例</span><span class="sxs-lookup"><span data-stu-id="5281c-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5281c-158">CSV</span><span class="sxs-lookup"><span data-stu-id="5281c-158">CSV</span></span>

<span data-ttu-id="5281c-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="5281c-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5281c-160">请求</span><span class="sxs-lookup"><span data-stu-id="5281c-160">Request</span></span>

<span data-ttu-id="5281c-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5281c-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5281c-162">响应</span><span class="sxs-lookup"><span data-stu-id="5281c-162">Response</span></span>

<span data-ttu-id="5281c-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5281c-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5281c-164">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5281c-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5281c-165">语言</span><span class="sxs-lookup"><span data-stu-id="5281c-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5281c-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="5281c-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5281c-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5281c-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="5281c-168">JSON</span><span class="sxs-lookup"><span data-stu-id="5281c-168">JSON</span></span>

<span data-ttu-id="5281c-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="5281c-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5281c-170">请求</span><span class="sxs-lookup"><span data-stu-id="5281c-170">Request</span></span>

<span data-ttu-id="5281c-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5281c-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5281c-172">响应</span><span class="sxs-lookup"><span data-stu-id="5281c-172">Response</span></span>

<span data-ttu-id="5281c-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5281c-173">The following is an example of the response.</span></span>

> <span data-ttu-id="5281c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5281c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5281c-176">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5281c-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5281c-177">语言</span><span class="sxs-lookup"><span data-stu-id="5281c-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5281c-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="5281c-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
