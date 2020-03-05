---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d50a7f359d6f0b3987bfb9c863f750018d73012a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454057"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="3dfce-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3dfce-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="3dfce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3dfce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfce-105">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="3dfce-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dfce-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dfce-106">Permissions</span></span>

<span data-ttu-id="3dfce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dfce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dfce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dfce-109">Permission type</span></span>                        | <span data-ttu-id="3dfce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dfce-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3dfce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dfce-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dfce-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3dfce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dfce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfce-114">Not supported.</span></span>                           |
| <span data-ttu-id="3dfce-115">应用</span><span class="sxs-lookup"><span data-stu-id="3dfce-115">Application</span></span>                            | <span data-ttu-id="3dfce-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dfce-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3dfce-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3dfce-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3dfce-118">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3dfce-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3dfce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dfce-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="3dfce-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="3dfce-120">Function parameters</span></span>

<span data-ttu-id="3dfce-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3dfce-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3dfce-122">参数</span><span class="sxs-lookup"><span data-stu-id="3dfce-122">Parameter</span></span> | <span data-ttu-id="3dfce-123">类型</span><span class="sxs-lookup"><span data-stu-id="3dfce-123">Type</span></span>   | <span data-ttu-id="3dfce-124">说明</span><span class="sxs-lookup"><span data-stu-id="3dfce-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3dfce-125">period</span><span class="sxs-lookup"><span data-stu-id="3dfce-125">period</span></span>    | <span data-ttu-id="3dfce-126">string</span><span class="sxs-lookup"><span data-stu-id="3dfce-126">string</span></span> | <span data-ttu-id="3dfce-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3dfce-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3dfce-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3dfce-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3dfce-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3dfce-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3dfce-130">必需。</span><span class="sxs-lookup"><span data-stu-id="3dfce-130">Required.</span></span> |

<span data-ttu-id="3dfce-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3dfce-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3dfce-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3dfce-132">The default output type is text/csv.</span></span> <span data-ttu-id="3dfce-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3dfce-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dfce-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dfce-134">Request headers</span></span>

| <span data-ttu-id="3dfce-135">名称</span><span class="sxs-lookup"><span data-stu-id="3dfce-135">Name</span></span>          | <span data-ttu-id="3dfce-136">说明</span><span class="sxs-lookup"><span data-stu-id="3dfce-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3dfce-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dfce-137">Authorization</span></span> | <span data-ttu-id="3dfce-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dfce-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3dfce-140">响应</span><span class="sxs-lookup"><span data-stu-id="3dfce-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3dfce-141">CSV</span><span class="sxs-lookup"><span data-stu-id="3dfce-141">CSV</span></span>

<span data-ttu-id="3dfce-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3dfce-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3dfce-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3dfce-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3dfce-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="3dfce-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3dfce-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="3dfce-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3dfce-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3dfce-146">Report Refresh Date</span></span>
- <span data-ttu-id="3dfce-147">Web</span><span class="sxs-lookup"><span data-stu-id="3dfce-147">Web</span></span>
- <span data-ttu-id="3dfce-148">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="3dfce-148">Windows Phone</span></span>
- <span data-ttu-id="3dfce-149">Android 手机</span><span class="sxs-lookup"><span data-stu-id="3dfce-149">Android Phone</span></span>
- <span data-ttu-id="3dfce-150">iOS</span><span class="sxs-lookup"><span data-stu-id="3dfce-150">iOS</span></span>
- <span data-ttu-id="3dfce-151">Mac</span><span class="sxs-lookup"><span data-stu-id="3dfce-151">Mac</span></span>
- <span data-ttu-id="3dfce-152">Windows</span><span class="sxs-lookup"><span data-stu-id="3dfce-152">Windows</span></span>
- <span data-ttu-id="3dfce-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="3dfce-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3dfce-154">JSON</span><span class="sxs-lookup"><span data-stu-id="3dfce-154">JSON</span></span>

<span data-ttu-id="3dfce-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3dfce-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfce-156">示例</span><span class="sxs-lookup"><span data-stu-id="3dfce-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3dfce-157">CSV</span><span class="sxs-lookup"><span data-stu-id="3dfce-157">CSV</span></span>

<span data-ttu-id="3dfce-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3dfce-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3dfce-159">请求</span><span class="sxs-lookup"><span data-stu-id="3dfce-159">Request</span></span>

<span data-ttu-id="3dfce-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dfce-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3dfce-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfce-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="3dfce-162">C#</span><span class="sxs-lookup"><span data-stu-id="3dfce-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dfce-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dfce-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dfce-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dfce-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3dfce-165">响应</span><span class="sxs-lookup"><span data-stu-id="3dfce-165">Response</span></span>

<span data-ttu-id="3dfce-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3dfce-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3dfce-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3dfce-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3dfce-168">JSON</span><span class="sxs-lookup"><span data-stu-id="3dfce-168">JSON</span></span>

<span data-ttu-id="3dfce-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3dfce-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3dfce-170">请求</span><span class="sxs-lookup"><span data-stu-id="3dfce-170">Request</span></span>

<span data-ttu-id="3dfce-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dfce-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3dfce-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dfce-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="3dfce-173">C#</span><span class="sxs-lookup"><span data-stu-id="3dfce-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dfce-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dfce-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dfce-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dfce-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3dfce-176">响应</span><span class="sxs-lookup"><span data-stu-id="3dfce-176">Response</span></span>

<span data-ttu-id="3dfce-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3dfce-177">The following is an example of the response.</span></span>

> <span data-ttu-id="3dfce-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3dfce-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
