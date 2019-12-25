---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e59c7c82192e287d00ccb1ae4582416955588c47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868945"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="aca4b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="aca4b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aca4b-104">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="aca4b-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="aca4b-105">权限</span><span class="sxs-lookup"><span data-stu-id="aca4b-105">Permissions</span></span>

<span data-ttu-id="aca4b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aca4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aca4b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aca4b-108">Permission type</span></span>                        | <span data-ttu-id="aca4b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aca4b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aca4b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aca4b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aca4b-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca4b-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aca4b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aca4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca4b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="aca4b-113">Not supported.</span></span>                           |
| <span data-ttu-id="aca4b-114">应用</span><span class="sxs-lookup"><span data-stu-id="aca4b-114">Application</span></span>                            | <span data-ttu-id="aca4b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca4b-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="aca4b-116">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="aca4b-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="aca4b-117">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="aca4b-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="aca4b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aca4b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="aca4b-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="aca4b-119">Function parameters</span></span>

<span data-ttu-id="aca4b-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="aca4b-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aca4b-121">参数</span><span class="sxs-lookup"><span data-stu-id="aca4b-121">Parameter</span></span> | <span data-ttu-id="aca4b-122">类型</span><span class="sxs-lookup"><span data-stu-id="aca4b-122">Type</span></span>   | <span data-ttu-id="aca4b-123">说明</span><span class="sxs-lookup"><span data-stu-id="aca4b-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aca4b-124">period</span><span class="sxs-lookup"><span data-stu-id="aca4b-124">period</span></span>    | <span data-ttu-id="aca4b-125">string</span><span class="sxs-lookup"><span data-stu-id="aca4b-125">string</span></span> | <span data-ttu-id="aca4b-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aca4b-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aca4b-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="aca4b-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aca4b-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aca4b-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aca4b-129">必需。</span><span class="sxs-lookup"><span data-stu-id="aca4b-129">Required.</span></span> |

<span data-ttu-id="aca4b-130">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aca4b-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aca4b-131">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="aca4b-131">The default output type is text/csv.</span></span> <span data-ttu-id="aca4b-132">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="aca4b-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aca4b-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="aca4b-133">Request headers</span></span>

| <span data-ttu-id="aca4b-134">名称</span><span class="sxs-lookup"><span data-stu-id="aca4b-134">Name</span></span>          | <span data-ttu-id="aca4b-135">说明</span><span class="sxs-lookup"><span data-stu-id="aca4b-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aca4b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="aca4b-136">Authorization</span></span> | <span data-ttu-id="aca4b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aca4b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aca4b-139">响应</span><span class="sxs-lookup"><span data-stu-id="aca4b-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aca4b-140">CSV</span><span class="sxs-lookup"><span data-stu-id="aca4b-140">CSV</span></span>

<span data-ttu-id="aca4b-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="aca4b-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aca4b-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="aca4b-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aca4b-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="aca4b-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aca4b-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="aca4b-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aca4b-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="aca4b-145">Report Refresh Date</span></span>
- <span data-ttu-id="aca4b-146">Web</span><span class="sxs-lookup"><span data-stu-id="aca4b-146">Web</span></span>
- <span data-ttu-id="aca4b-147">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="aca4b-147">Windows Phone</span></span>
- <span data-ttu-id="aca4b-148">Android 手机</span><span class="sxs-lookup"><span data-stu-id="aca4b-148">Android Phone</span></span>
- <span data-ttu-id="aca4b-149">iOS</span><span class="sxs-lookup"><span data-stu-id="aca4b-149">iOS</span></span>
- <span data-ttu-id="aca4b-150">Mac</span><span class="sxs-lookup"><span data-stu-id="aca4b-150">Mac</span></span>
- <span data-ttu-id="aca4b-151">Windows</span><span class="sxs-lookup"><span data-stu-id="aca4b-151">Windows</span></span>
- <span data-ttu-id="aca4b-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="aca4b-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aca4b-153">JSON</span><span class="sxs-lookup"><span data-stu-id="aca4b-153">JSON</span></span>

<span data-ttu-id="aca4b-154">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="aca4b-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aca4b-155">示例</span><span class="sxs-lookup"><span data-stu-id="aca4b-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aca4b-156">CSV</span><span class="sxs-lookup"><span data-stu-id="aca4b-156">CSV</span></span>

<span data-ttu-id="aca4b-157">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="aca4b-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aca4b-158">请求</span><span class="sxs-lookup"><span data-stu-id="aca4b-158">Request</span></span>

<span data-ttu-id="aca4b-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aca4b-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aca4b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="aca4b-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aca4b-161">C#</span><span class="sxs-lookup"><span data-stu-id="aca4b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aca4b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aca4b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aca4b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aca4b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aca4b-164">响应</span><span class="sxs-lookup"><span data-stu-id="aca4b-164">Response</span></span>

<span data-ttu-id="aca4b-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aca4b-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aca4b-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="aca4b-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="aca4b-167">JSON</span><span class="sxs-lookup"><span data-stu-id="aca4b-167">JSON</span></span>

<span data-ttu-id="aca4b-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="aca4b-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aca4b-169">请求</span><span class="sxs-lookup"><span data-stu-id="aca4b-169">Request</span></span>

<span data-ttu-id="aca4b-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aca4b-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aca4b-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="aca4b-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aca4b-172">C#</span><span class="sxs-lookup"><span data-stu-id="aca4b-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aca4b-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aca4b-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aca4b-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aca4b-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aca4b-175">响应</span><span class="sxs-lookup"><span data-stu-id="aca4b-175">Response</span></span>

<span data-ttu-id="aca4b-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aca4b-176">The following is an example of the response.</span></span>

> <span data-ttu-id="aca4b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aca4b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
