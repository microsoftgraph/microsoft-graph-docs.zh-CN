---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: 获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。 还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b6f228913fe8ba552bec36d7381e2931247cfec0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869027"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="28403-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="28403-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28403-105">获取使用情况趋势，即组织中有多少用户已使用 Skype for Business 应用进行了连接。</span><span class="sxs-lookup"><span data-stu-id="28403-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="28403-106">还可以按设备类型（Windows、Windows 手机、Android 手机、iPhone 或 iPad）进一步了解整个组织中安装和使用的 Skype for Business 客户端应用。</span><span class="sxs-lookup"><span data-stu-id="28403-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="28403-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="28403-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="28403-108">权限</span><span class="sxs-lookup"><span data-stu-id="28403-108">Permissions</span></span>

<span data-ttu-id="28403-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28403-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28403-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="28403-111">Permission type</span></span>                        | <span data-ttu-id="28403-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28403-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="28403-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28403-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="28403-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28403-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="28403-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28403-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28403-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="28403-116">Not supported.</span></span>                           |
| <span data-ttu-id="28403-117">应用</span><span class="sxs-lookup"><span data-stu-id="28403-117">Application</span></span>                            | <span data-ttu-id="28403-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28403-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="28403-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="28403-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="28403-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="28403-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="28403-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28403-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="28403-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="28403-122">Function parameters</span></span>

<span data-ttu-id="28403-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="28403-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="28403-124">参数</span><span class="sxs-lookup"><span data-stu-id="28403-124">Parameter</span></span> | <span data-ttu-id="28403-125">类型</span><span class="sxs-lookup"><span data-stu-id="28403-125">Type</span></span>   | <span data-ttu-id="28403-126">说明</span><span class="sxs-lookup"><span data-stu-id="28403-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="28403-127">period</span><span class="sxs-lookup"><span data-stu-id="28403-127">period</span></span>    | <span data-ttu-id="28403-128">string</span><span class="sxs-lookup"><span data-stu-id="28403-128">string</span></span> | <span data-ttu-id="28403-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="28403-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="28403-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="28403-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="28403-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="28403-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="28403-132">必需。</span><span class="sxs-lookup"><span data-stu-id="28403-132">Required.</span></span> |

<span data-ttu-id="28403-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="28403-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="28403-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="28403-134">The default output type is text/csv.</span></span> <span data-ttu-id="28403-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="28403-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28403-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="28403-136">Request headers</span></span>

| <span data-ttu-id="28403-137">名称</span><span class="sxs-lookup"><span data-stu-id="28403-137">Name</span></span>          | <span data-ttu-id="28403-138">说明</span><span class="sxs-lookup"><span data-stu-id="28403-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="28403-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="28403-139">Authorization</span></span> | <span data-ttu-id="28403-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28403-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="28403-142">响应</span><span class="sxs-lookup"><span data-stu-id="28403-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="28403-143">CSV</span><span class="sxs-lookup"><span data-stu-id="28403-143">CSV</span></span>

<span data-ttu-id="28403-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="28403-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="28403-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="28403-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="28403-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="28403-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="28403-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="28403-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="28403-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="28403-148">Report Refresh Date</span></span>
- <span data-ttu-id="28403-149">Windows</span><span class="sxs-lookup"><span data-stu-id="28403-149">Windows</span></span>
- <span data-ttu-id="28403-150">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="28403-150">Windows Phone</span></span>
- <span data-ttu-id="28403-151">Android 手机</span><span class="sxs-lookup"><span data-stu-id="28403-151">Android Phone</span></span>
- <span data-ttu-id="28403-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="28403-152">iPhone</span></span>
- <span data-ttu-id="28403-153">iPad</span><span class="sxs-lookup"><span data-stu-id="28403-153">iPad</span></span>
- <span data-ttu-id="28403-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="28403-154">Report Date</span></span>
- <span data-ttu-id="28403-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="28403-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="28403-156">JSON</span><span class="sxs-lookup"><span data-stu-id="28403-156">JSON</span></span>

<span data-ttu-id="28403-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="28403-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28403-158">示例</span><span class="sxs-lookup"><span data-stu-id="28403-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="28403-159">CSV</span><span class="sxs-lookup"><span data-stu-id="28403-159">CSV</span></span>

<span data-ttu-id="28403-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="28403-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="28403-161">请求</span><span class="sxs-lookup"><span data-stu-id="28403-161">Request</span></span>

<span data-ttu-id="28403-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28403-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="28403-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="28403-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28403-164">C#</span><span class="sxs-lookup"><span data-stu-id="28403-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28403-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28403-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28403-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28403-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28403-167">响应</span><span class="sxs-lookup"><span data-stu-id="28403-167">Response</span></span>

<span data-ttu-id="28403-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28403-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="28403-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="28403-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="28403-170">JSON</span><span class="sxs-lookup"><span data-stu-id="28403-170">JSON</span></span>

<span data-ttu-id="28403-171">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="28403-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="28403-172">请求</span><span class="sxs-lookup"><span data-stu-id="28403-172">Request</span></span>

<span data-ttu-id="28403-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28403-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="28403-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="28403-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28403-175">C#</span><span class="sxs-lookup"><span data-stu-id="28403-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28403-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28403-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28403-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28403-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28403-178">响应</span><span class="sxs-lookup"><span data-stu-id="28403-178">Response</span></span>

<span data-ttu-id="28403-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="28403-179">The following is an example of the response.</span></span>

> <span data-ttu-id="28403-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28403-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
      "reportDate": "2017-09-01", 
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
