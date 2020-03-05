---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8a90f597ecc52ab34478c596b6d141d084623623
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454197"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="79cc8-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="79cc8-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="79cc8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="79cc8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cc8-106">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="79cc8-106">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="79cc8-107">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="79cc8-107">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="79cc8-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="79cc8-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="79cc8-109">权限</span><span class="sxs-lookup"><span data-stu-id="79cc8-109">Permissions</span></span>

<span data-ttu-id="79cc8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79cc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79cc8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="79cc8-112">Permission type</span></span>                        | <span data-ttu-id="79cc8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79cc8-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="79cc8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79cc8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="79cc8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79cc8-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="79cc8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79cc8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79cc8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79cc8-117">Not supported.</span></span>                           |
| <span data-ttu-id="79cc8-118">应用</span><span class="sxs-lookup"><span data-stu-id="79cc8-118">Application</span></span>                            | <span data-ttu-id="79cc8-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79cc8-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="79cc8-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="79cc8-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="79cc8-121">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="79cc8-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="79cc8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79cc8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="79cc8-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="79cc8-123">Function parameters</span></span>

<span data-ttu-id="79cc8-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="79cc8-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="79cc8-125">参数</span><span class="sxs-lookup"><span data-stu-id="79cc8-125">Parameter</span></span> | <span data-ttu-id="79cc8-126">类型</span><span class="sxs-lookup"><span data-stu-id="79cc8-126">Type</span></span>   | <span data-ttu-id="79cc8-127">说明</span><span class="sxs-lookup"><span data-stu-id="79cc8-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="79cc8-128">period</span><span class="sxs-lookup"><span data-stu-id="79cc8-128">period</span></span>    | <span data-ttu-id="79cc8-129">string</span><span class="sxs-lookup"><span data-stu-id="79cc8-129">string</span></span> | <span data-ttu-id="79cc8-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="79cc8-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="79cc8-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="79cc8-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="79cc8-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="79cc8-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="79cc8-133">必需。</span><span class="sxs-lookup"><span data-stu-id="79cc8-133">Required.</span></span> |

<span data-ttu-id="79cc8-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79cc8-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="79cc8-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="79cc8-135">The default output type is text/csv.</span></span> <span data-ttu-id="79cc8-136">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="79cc8-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79cc8-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="79cc8-137">Request headers</span></span>

| <span data-ttu-id="79cc8-138">名称</span><span class="sxs-lookup"><span data-stu-id="79cc8-138">Name</span></span>          | <span data-ttu-id="79cc8-139">说明</span><span class="sxs-lookup"><span data-stu-id="79cc8-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="79cc8-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="79cc8-140">Authorization</span></span> | <span data-ttu-id="79cc8-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79cc8-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="79cc8-143">响应</span><span class="sxs-lookup"><span data-stu-id="79cc8-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="79cc8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="79cc8-144">CSV</span></span>

<span data-ttu-id="79cc8-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="79cc8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="79cc8-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="79cc8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="79cc8-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="79cc8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="79cc8-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="79cc8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="79cc8-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="79cc8-149">Report Refresh Date</span></span>
- <span data-ttu-id="79cc8-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="79cc8-150">Report Date</span></span>
- <span data-ttu-id="79cc8-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="79cc8-151">Report Period</span></span>
- <span data-ttu-id="79cc8-152">对等</span><span class="sxs-lookup"><span data-stu-id="79cc8-152">Peer-to-peer</span></span>
- <span data-ttu-id="79cc8-153">组织</span><span class="sxs-lookup"><span data-stu-id="79cc8-153">Organized</span></span>
- <span data-ttu-id="79cc8-154">参与</span><span class="sxs-lookup"><span data-stu-id="79cc8-154">Participated</span></span>

### <a name="json"></a><span data-ttu-id="79cc8-155">JSON</span><span class="sxs-lookup"><span data-stu-id="79cc8-155">JSON</span></span>

<span data-ttu-id="79cc8-156">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="79cc8-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79cc8-157">示例</span><span class="sxs-lookup"><span data-stu-id="79cc8-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="79cc8-158">CSV</span><span class="sxs-lookup"><span data-stu-id="79cc8-158">CSV</span></span>

<span data-ttu-id="79cc8-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="79cc8-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="79cc8-160">请求</span><span class="sxs-lookup"><span data-stu-id="79cc8-160">Request</span></span>

<span data-ttu-id="79cc8-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79cc8-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79cc8-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="79cc8-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="79cc8-163">C#</span><span class="sxs-lookup"><span data-stu-id="79cc8-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79cc8-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79cc8-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79cc8-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79cc8-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79cc8-166">响应</span><span class="sxs-lookup"><span data-stu-id="79cc8-166">Response</span></span>

<span data-ttu-id="79cc8-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79cc8-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="79cc8-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="79cc8-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="79cc8-169">JSON</span><span class="sxs-lookup"><span data-stu-id="79cc8-169">JSON</span></span>

<span data-ttu-id="79cc8-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="79cc8-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="79cc8-171">请求</span><span class="sxs-lookup"><span data-stu-id="79cc8-171">Request</span></span>

<span data-ttu-id="79cc8-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79cc8-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79cc8-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="79cc8-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="79cc8-174">C#</span><span class="sxs-lookup"><span data-stu-id="79cc8-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79cc8-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79cc8-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79cc8-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79cc8-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79cc8-177">响应</span><span class="sxs-lookup"><span data-stu-id="79cc8-177">Response</span></span>

<span data-ttu-id="79cc8-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="79cc8-178">The following is an example of the response.</span></span>

> <span data-ttu-id="79cc8-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="79cc8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
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
