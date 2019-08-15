---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ff546a159d7ca25d72739da9512f7cce6e66742a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411331"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="519cc-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="519cc-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="519cc-105">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="519cc-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="519cc-106">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="519cc-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="519cc-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="519cc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="519cc-108">权限</span><span class="sxs-lookup"><span data-stu-id="519cc-108">Permissions</span></span>

<span data-ttu-id="519cc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="519cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="519cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="519cc-111">Permission type</span></span>                        | <span data-ttu-id="519cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="519cc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="519cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="519cc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="519cc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="519cc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="519cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="519cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="519cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="519cc-116">Not supported.</span></span>                           |
| <span data-ttu-id="519cc-117">应用</span><span class="sxs-lookup"><span data-stu-id="519cc-117">Application</span></span>                            | <span data-ttu-id="519cc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="519cc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="519cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="519cc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="519cc-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="519cc-120">Function parameters</span></span>

<span data-ttu-id="519cc-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="519cc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="519cc-122">参数</span><span class="sxs-lookup"><span data-stu-id="519cc-122">Parameter</span></span> | <span data-ttu-id="519cc-123">类型</span><span class="sxs-lookup"><span data-stu-id="519cc-123">Type</span></span>   | <span data-ttu-id="519cc-124">说明</span><span class="sxs-lookup"><span data-stu-id="519cc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="519cc-125">period</span><span class="sxs-lookup"><span data-stu-id="519cc-125">period</span></span>    | <span data-ttu-id="519cc-126">string</span><span class="sxs-lookup"><span data-stu-id="519cc-126">string</span></span> | <span data-ttu-id="519cc-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="519cc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="519cc-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="519cc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="519cc-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="519cc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="519cc-130">必需。</span><span class="sxs-lookup"><span data-stu-id="519cc-130">Required.</span></span> |

<span data-ttu-id="519cc-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="519cc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="519cc-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="519cc-132">The default output type is text/csv.</span></span> <span data-ttu-id="519cc-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="519cc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="519cc-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="519cc-134">Request headers</span></span>

| <span data-ttu-id="519cc-135">名称</span><span class="sxs-lookup"><span data-stu-id="519cc-135">Name</span></span>          | <span data-ttu-id="519cc-136">说明</span><span class="sxs-lookup"><span data-stu-id="519cc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="519cc-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="519cc-137">Authorization</span></span> | <span data-ttu-id="519cc-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="519cc-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="519cc-140">响应</span><span class="sxs-lookup"><span data-stu-id="519cc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="519cc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="519cc-141">CSV</span></span>

<span data-ttu-id="519cc-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="519cc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="519cc-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="519cc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="519cc-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="519cc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="519cc-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="519cc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="519cc-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="519cc-146">Report Refresh Date</span></span>
- <span data-ttu-id="519cc-147">Windows</span><span class="sxs-lookup"><span data-stu-id="519cc-147">Windows</span></span>
- <span data-ttu-id="519cc-148">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="519cc-148">Windows Phone</span></span>
- <span data-ttu-id="519cc-149">Android 手机</span><span class="sxs-lookup"><span data-stu-id="519cc-149">Android Phone</span></span>
- <span data-ttu-id="519cc-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="519cc-150">iPhone</span></span>
- <span data-ttu-id="519cc-151">iPad</span><span class="sxs-lookup"><span data-stu-id="519cc-151">iPad</span></span>
- <span data-ttu-id="519cc-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="519cc-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="519cc-153">JSON</span><span class="sxs-lookup"><span data-stu-id="519cc-153">JSON</span></span>

<span data-ttu-id="519cc-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="519cc-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="519cc-155">示例</span><span class="sxs-lookup"><span data-stu-id="519cc-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="519cc-156">CSV</span><span class="sxs-lookup"><span data-stu-id="519cc-156">CSV</span></span>

<span data-ttu-id="519cc-157">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="519cc-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="519cc-158">请求</span><span class="sxs-lookup"><span data-stu-id="519cc-158">Request</span></span>

<span data-ttu-id="519cc-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="519cc-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="519cc-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="519cc-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="519cc-161">C#</span><span class="sxs-lookup"><span data-stu-id="519cc-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="519cc-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519cc-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="519cc-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="519cc-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519cc-164">响应</span><span class="sxs-lookup"><span data-stu-id="519cc-164">Response</span></span>

<span data-ttu-id="519cc-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="519cc-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="519cc-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="519cc-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="519cc-167">JSON</span><span class="sxs-lookup"><span data-stu-id="519cc-167">JSON</span></span>

<span data-ttu-id="519cc-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="519cc-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="519cc-169">请求</span><span class="sxs-lookup"><span data-stu-id="519cc-169">Request</span></span>

<span data-ttu-id="519cc-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="519cc-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="519cc-171">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="519cc-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="519cc-172">C#</span><span class="sxs-lookup"><span data-stu-id="519cc-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="519cc-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="519cc-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="519cc-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="519cc-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="519cc-175">响应</span><span class="sxs-lookup"><span data-stu-id="519cc-175">Response</span></span>

<span data-ttu-id="519cc-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="519cc-176">The following is an example of the response.</span></span>

> <span data-ttu-id="519cc-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="519cc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
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
