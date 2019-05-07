---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: 获取使用情况趋势，即组织中召开的会话的次数和类型。 会话类型包括 IM、音频、视频、应用共享和文件传输。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d903b1b77e481e84f564e7de61c31a08723b857b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639129"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="d591a-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d591a-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d591a-105">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="d591a-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="d591a-106">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="d591a-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="d591a-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="d591a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="d591a-108">权限</span><span class="sxs-lookup"><span data-stu-id="d591a-108">Permissions</span></span>

<span data-ttu-id="d591a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d591a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d591a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d591a-111">Permission type</span></span>                        | <span data-ttu-id="d591a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d591a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d591a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d591a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d591a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d591a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d591a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d591a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d591a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d591a-116">Not supported.</span></span>                           |
| <span data-ttu-id="d591a-117">应用</span><span class="sxs-lookup"><span data-stu-id="d591a-117">Application</span></span>                            | <span data-ttu-id="d591a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d591a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d591a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d591a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d591a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d591a-120">Function parameters</span></span>

<span data-ttu-id="d591a-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d591a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d591a-122">参数</span><span class="sxs-lookup"><span data-stu-id="d591a-122">Parameter</span></span> | <span data-ttu-id="d591a-123">类型</span><span class="sxs-lookup"><span data-stu-id="d591a-123">Type</span></span>   | <span data-ttu-id="d591a-124">说明</span><span class="sxs-lookup"><span data-stu-id="d591a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d591a-125">period</span><span class="sxs-lookup"><span data-stu-id="d591a-125">period</span></span>    | <span data-ttu-id="d591a-126">string</span><span class="sxs-lookup"><span data-stu-id="d591a-126">string</span></span> | <span data-ttu-id="d591a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d591a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d591a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d591a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d591a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d591a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d591a-130">必需。</span><span class="sxs-lookup"><span data-stu-id="d591a-130">Required.</span></span> |

<span data-ttu-id="d591a-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d591a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d591a-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d591a-132">The default output type is text/csv.</span></span> <span data-ttu-id="d591a-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d591a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d591a-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="d591a-134">Request headers</span></span>

| <span data-ttu-id="d591a-135">名称</span><span class="sxs-lookup"><span data-stu-id="d591a-135">Name</span></span>          | <span data-ttu-id="d591a-136">说明</span><span class="sxs-lookup"><span data-stu-id="d591a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d591a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d591a-137">Authorization</span></span> | <span data-ttu-id="d591a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d591a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d591a-140">响应</span><span class="sxs-lookup"><span data-stu-id="d591a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d591a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d591a-141">CSV</span></span>

<span data-ttu-id="d591a-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d591a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d591a-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d591a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d591a-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d591a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d591a-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d591a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d591a-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d591a-146">Report Refresh Date</span></span>
- <span data-ttu-id="d591a-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="d591a-147">Report Date</span></span>
- <span data-ttu-id="d591a-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="d591a-148">Report Period</span></span>
- <span data-ttu-id="d591a-149">IM</span><span class="sxs-lookup"><span data-stu-id="d591a-149">IM</span></span>
- <span data-ttu-id="d591a-150">音频</span><span class="sxs-lookup"><span data-stu-id="d591a-150">Audio</span></span>
- <span data-ttu-id="d591a-151">视频</span><span class="sxs-lookup"><span data-stu-id="d591a-151">Video</span></span>
- <span data-ttu-id="d591a-152">应用共享</span><span class="sxs-lookup"><span data-stu-id="d591a-152">App Sharing</span></span>
- <span data-ttu-id="d591a-153">文件传输</span><span class="sxs-lookup"><span data-stu-id="d591a-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="d591a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="d591a-154">JSON</span></span>

<span data-ttu-id="d591a-155">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d591a-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d591a-156">示例</span><span class="sxs-lookup"><span data-stu-id="d591a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d591a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="d591a-157">CSV</span></span>

<span data-ttu-id="d591a-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d591a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d591a-159">请求</span><span class="sxs-lookup"><span data-stu-id="d591a-159">Request</span></span>

<span data-ttu-id="d591a-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d591a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d591a-161">响应</span><span class="sxs-lookup"><span data-stu-id="d591a-161">Response</span></span>

<span data-ttu-id="d591a-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d591a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d591a-163">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d591a-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d591a-164">语言</span><span class="sxs-lookup"><span data-stu-id="d591a-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d591a-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="d591a-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d591a-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d591a-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="d591a-167">JSON</span><span class="sxs-lookup"><span data-stu-id="d591a-167">JSON</span></span>

<span data-ttu-id="d591a-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d591a-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d591a-169">请求</span><span class="sxs-lookup"><span data-stu-id="d591a-169">Request</span></span>

<span data-ttu-id="d591a-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d591a-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d591a-171">响应</span><span class="sxs-lookup"><span data-stu-id="d591a-171">Response</span></span>

<span data-ttu-id="d591a-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d591a-172">The following is an example of the response.</span></span>

> <span data-ttu-id="d591a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d591a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d591a-175">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d591a-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d591a-176">语言</span><span class="sxs-lookup"><span data-stu-id="d591a-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d591a-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="d591a-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinesspeertopeeractivitycounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
