---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4dd07f0401adfc03856bfebb8aa1894f6ffb7a2e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639143"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="045ff-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="045ff-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="045ff-104">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="045ff-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="045ff-105">权限</span><span class="sxs-lookup"><span data-stu-id="045ff-105">Permissions</span></span>

<span data-ttu-id="045ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="045ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="045ff-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="045ff-108">Permission type</span></span>                        | <span data-ttu-id="045ff-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="045ff-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="045ff-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="045ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="045ff-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="045ff-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="045ff-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="045ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="045ff-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="045ff-113">Not supported.</span></span>                           |
| <span data-ttu-id="045ff-114">应用</span><span class="sxs-lookup"><span data-stu-id="045ff-114">Application</span></span>                            | <span data-ttu-id="045ff-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="045ff-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="045ff-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="045ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="045ff-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="045ff-117">Function parameters</span></span>

<span data-ttu-id="045ff-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="045ff-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="045ff-119">参数</span><span class="sxs-lookup"><span data-stu-id="045ff-119">Parameter</span></span> | <span data-ttu-id="045ff-120">类型</span><span class="sxs-lookup"><span data-stu-id="045ff-120">Type</span></span>   | <span data-ttu-id="045ff-121">说明</span><span class="sxs-lookup"><span data-stu-id="045ff-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="045ff-122">period</span><span class="sxs-lookup"><span data-stu-id="045ff-122">period</span></span>    | <span data-ttu-id="045ff-123">string</span><span class="sxs-lookup"><span data-stu-id="045ff-123">string</span></span> | <span data-ttu-id="045ff-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="045ff-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="045ff-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="045ff-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="045ff-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="045ff-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="045ff-127">必需。</span><span class="sxs-lookup"><span data-stu-id="045ff-127">Required.</span></span> |

<span data-ttu-id="045ff-128">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="045ff-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="045ff-129">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="045ff-129">The default output type is text/csv.</span></span> <span data-ttu-id="045ff-130">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="045ff-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="045ff-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="045ff-131">Request headers</span></span>

| <span data-ttu-id="045ff-132">名称</span><span class="sxs-lookup"><span data-stu-id="045ff-132">Name</span></span>          | <span data-ttu-id="045ff-133">说明</span><span class="sxs-lookup"><span data-stu-id="045ff-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="045ff-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="045ff-134">Authorization</span></span> | <span data-ttu-id="045ff-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="045ff-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="045ff-137">响应</span><span class="sxs-lookup"><span data-stu-id="045ff-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="045ff-138">CSV</span><span class="sxs-lookup"><span data-stu-id="045ff-138">CSV</span></span>

<span data-ttu-id="045ff-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="045ff-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="045ff-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="045ff-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="045ff-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="045ff-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="045ff-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="045ff-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="045ff-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="045ff-143">Report Refresh Date</span></span>
- <span data-ttu-id="045ff-144">Web</span><span class="sxs-lookup"><span data-stu-id="045ff-144">Web</span></span>
- <span data-ttu-id="045ff-145">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="045ff-145">Windows Phone</span></span>
- <span data-ttu-id="045ff-146">Android 手机</span><span class="sxs-lookup"><span data-stu-id="045ff-146">Android Phone</span></span>
- <span data-ttu-id="045ff-147">iOS</span><span class="sxs-lookup"><span data-stu-id="045ff-147">iOS</span></span>
- <span data-ttu-id="045ff-148">Mac</span><span class="sxs-lookup"><span data-stu-id="045ff-148">Mac</span></span>
- <span data-ttu-id="045ff-149">Windows</span><span class="sxs-lookup"><span data-stu-id="045ff-149">Windows</span></span>
- <span data-ttu-id="045ff-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="045ff-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="045ff-151">JSON</span><span class="sxs-lookup"><span data-stu-id="045ff-151">JSON</span></span>

<span data-ttu-id="045ff-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="045ff-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="045ff-153">示例</span><span class="sxs-lookup"><span data-stu-id="045ff-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="045ff-154">CSV</span><span class="sxs-lookup"><span data-stu-id="045ff-154">CSV</span></span>

<span data-ttu-id="045ff-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="045ff-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="045ff-156">请求</span><span class="sxs-lookup"><span data-stu-id="045ff-156">Request</span></span>

<span data-ttu-id="045ff-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="045ff-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="045ff-158">响应</span><span class="sxs-lookup"><span data-stu-id="045ff-158">Response</span></span>

<span data-ttu-id="045ff-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="045ff-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="045ff-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="045ff-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="045ff-161">语言</span><span class="sxs-lookup"><span data-stu-id="045ff-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="045ff-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="045ff-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="045ff-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="045ff-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="045ff-164">JSON</span><span class="sxs-lookup"><span data-stu-id="045ff-164">JSON</span></span>

<span data-ttu-id="045ff-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="045ff-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="045ff-166">请求</span><span class="sxs-lookup"><span data-stu-id="045ff-166">Request</span></span>

<span data-ttu-id="045ff-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="045ff-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="045ff-168">响应</span><span class="sxs-lookup"><span data-stu-id="045ff-168">Response</span></span>

<span data-ttu-id="045ff-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="045ff-169">The following is an example of the response.</span></span>

> <span data-ttu-id="045ff-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="045ff-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="045ff-172">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="045ff-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="045ff-173">语言</span><span class="sxs-lookup"><span data-stu-id="045ff-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="045ff-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="045ff-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
