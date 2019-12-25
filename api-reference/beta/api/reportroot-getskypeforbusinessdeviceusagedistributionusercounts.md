---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b92525ca73ea17e35c0de430ca2e141834c6764e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867363"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="fe77c-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="fe77c-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe77c-105">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="fe77c-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="fe77c-106">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="fe77c-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="fe77c-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="fe77c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe77c-108">权限</span><span class="sxs-lookup"><span data-stu-id="fe77c-108">Permissions</span></span>

<span data-ttu-id="fe77c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe77c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe77c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe77c-111">Permission type</span></span>                        | <span data-ttu-id="fe77c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe77c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fe77c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe77c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe77c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe77c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fe77c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe77c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe77c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe77c-116">Not supported.</span></span>                           |
| <span data-ttu-id="fe77c-117">应用</span><span class="sxs-lookup"><span data-stu-id="fe77c-117">Application</span></span>                            | <span data-ttu-id="fe77c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe77c-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="fe77c-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="fe77c-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="fe77c-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="fe77c-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="fe77c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe77c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fe77c-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="fe77c-122">Function parameters</span></span>

<span data-ttu-id="fe77c-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fe77c-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fe77c-124">参数</span><span class="sxs-lookup"><span data-stu-id="fe77c-124">Parameter</span></span> | <span data-ttu-id="fe77c-125">类型</span><span class="sxs-lookup"><span data-stu-id="fe77c-125">Type</span></span>   | <span data-ttu-id="fe77c-126">说明</span><span class="sxs-lookup"><span data-stu-id="fe77c-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fe77c-127">period</span><span class="sxs-lookup"><span data-stu-id="fe77c-127">period</span></span>    | <span data-ttu-id="fe77c-128">string</span><span class="sxs-lookup"><span data-stu-id="fe77c-128">string</span></span> | <span data-ttu-id="fe77c-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fe77c-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fe77c-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fe77c-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fe77c-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fe77c-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fe77c-132">必需。</span><span class="sxs-lookup"><span data-stu-id="fe77c-132">Required.</span></span> |

<span data-ttu-id="fe77c-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe77c-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fe77c-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="fe77c-134">The default output type is text/csv.</span></span> <span data-ttu-id="fe77c-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="fe77c-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe77c-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe77c-136">Request headers</span></span>

| <span data-ttu-id="fe77c-137">名称</span><span class="sxs-lookup"><span data-stu-id="fe77c-137">Name</span></span>          | <span data-ttu-id="fe77c-138">说明</span><span class="sxs-lookup"><span data-stu-id="fe77c-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fe77c-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe77c-139">Authorization</span></span> | <span data-ttu-id="fe77c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe77c-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fe77c-142">响应</span><span class="sxs-lookup"><span data-stu-id="fe77c-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fe77c-143">CSV</span><span class="sxs-lookup"><span data-stu-id="fe77c-143">CSV</span></span>

<span data-ttu-id="fe77c-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fe77c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fe77c-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fe77c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fe77c-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fe77c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fe77c-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fe77c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fe77c-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fe77c-148">Report Refresh Date</span></span>
- <span data-ttu-id="fe77c-149">Windows</span><span class="sxs-lookup"><span data-stu-id="fe77c-149">Windows</span></span>
- <span data-ttu-id="fe77c-150">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="fe77c-150">Windows Phone</span></span>
- <span data-ttu-id="fe77c-151">Android 手机</span><span class="sxs-lookup"><span data-stu-id="fe77c-151">Android Phone</span></span>
- <span data-ttu-id="fe77c-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="fe77c-152">iPhone</span></span>
- <span data-ttu-id="fe77c-153">iPad</span><span class="sxs-lookup"><span data-stu-id="fe77c-153">iPad</span></span>
- <span data-ttu-id="fe77c-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="fe77c-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fe77c-155">JSON</span><span class="sxs-lookup"><span data-stu-id="fe77c-155">JSON</span></span>

<span data-ttu-id="fe77c-156">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fe77c-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe77c-157">示例</span><span class="sxs-lookup"><span data-stu-id="fe77c-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fe77c-158">CSV</span><span class="sxs-lookup"><span data-stu-id="fe77c-158">CSV</span></span>

<span data-ttu-id="fe77c-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="fe77c-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fe77c-160">请求</span><span class="sxs-lookup"><span data-stu-id="fe77c-160">Request</span></span>

<span data-ttu-id="fe77c-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fe77c-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe77c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe77c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe77c-163">C#</span><span class="sxs-lookup"><span data-stu-id="fe77c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe77c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe77c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe77c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe77c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fe77c-166">响应</span><span class="sxs-lookup"><span data-stu-id="fe77c-166">Response</span></span>

<span data-ttu-id="fe77c-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fe77c-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fe77c-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fe77c-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fe77c-169">JSON</span><span class="sxs-lookup"><span data-stu-id="fe77c-169">JSON</span></span>

<span data-ttu-id="fe77c-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fe77c-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fe77c-171">请求</span><span class="sxs-lookup"><span data-stu-id="fe77c-171">Request</span></span>

<span data-ttu-id="fe77c-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fe77c-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe77c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe77c-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe77c-174">C#</span><span class="sxs-lookup"><span data-stu-id="fe77c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe77c-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe77c-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe77c-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe77c-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fe77c-177">响应</span><span class="sxs-lookup"><span data-stu-id="fe77c-177">Response</span></span>

<span data-ttu-id="fe77c-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe77c-178">The following is an example of the response.</span></span>

> <span data-ttu-id="fe77c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fe77c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
