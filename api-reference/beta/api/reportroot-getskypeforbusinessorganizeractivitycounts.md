---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c3a325628803b3062263076dd24338eafd557dd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868990"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="46c08-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="46c08-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46c08-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="46c08-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="46c08-106">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="46c08-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="46c08-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="46c08-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="46c08-108">权限</span><span class="sxs-lookup"><span data-stu-id="46c08-108">Permissions</span></span>

<span data-ttu-id="46c08-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46c08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46c08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46c08-111">Permission type</span></span>                        | <span data-ttu-id="46c08-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46c08-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="46c08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46c08-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="46c08-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c08-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="46c08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46c08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46c08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c08-116">Not supported.</span></span>                           |
| <span data-ttu-id="46c08-117">应用</span><span class="sxs-lookup"><span data-stu-id="46c08-117">Application</span></span>                            | <span data-ttu-id="46c08-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c08-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="46c08-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="46c08-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="46c08-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="46c08-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="46c08-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46c08-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="46c08-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="46c08-122">Function parameters</span></span>

<span data-ttu-id="46c08-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="46c08-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="46c08-124">参数</span><span class="sxs-lookup"><span data-stu-id="46c08-124">Parameter</span></span> | <span data-ttu-id="46c08-125">类型</span><span class="sxs-lookup"><span data-stu-id="46c08-125">Type</span></span>   | <span data-ttu-id="46c08-126">说明</span><span class="sxs-lookup"><span data-stu-id="46c08-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="46c08-127">period</span><span class="sxs-lookup"><span data-stu-id="46c08-127">period</span></span>    | <span data-ttu-id="46c08-128">string</span><span class="sxs-lookup"><span data-stu-id="46c08-128">string</span></span> | <span data-ttu-id="46c08-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="46c08-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="46c08-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="46c08-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="46c08-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="46c08-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="46c08-132">必需。</span><span class="sxs-lookup"><span data-stu-id="46c08-132">Required.</span></span> |

<span data-ttu-id="46c08-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46c08-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="46c08-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="46c08-134">The default output type is text/csv.</span></span> <span data-ttu-id="46c08-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="46c08-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46c08-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="46c08-136">Request headers</span></span>

| <span data-ttu-id="46c08-137">名称</span><span class="sxs-lookup"><span data-stu-id="46c08-137">Name</span></span>          | <span data-ttu-id="46c08-138">说明</span><span class="sxs-lookup"><span data-stu-id="46c08-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="46c08-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="46c08-139">Authorization</span></span> | <span data-ttu-id="46c08-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46c08-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46c08-142">响应</span><span class="sxs-lookup"><span data-stu-id="46c08-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="46c08-143">CSV</span><span class="sxs-lookup"><span data-stu-id="46c08-143">CSV</span></span>

<span data-ttu-id="46c08-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="46c08-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="46c08-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="46c08-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="46c08-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="46c08-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="46c08-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="46c08-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="46c08-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="46c08-148">Report Refresh Date</span></span>
- <span data-ttu-id="46c08-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="46c08-149">Report Date</span></span>
- <span data-ttu-id="46c08-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="46c08-150">Report Period</span></span>
- <span data-ttu-id="46c08-151">IM</span><span class="sxs-lookup"><span data-stu-id="46c08-151">IM</span></span>
- <span data-ttu-id="46c08-152">音频/视频</span><span class="sxs-lookup"><span data-stu-id="46c08-152">Audio/Video</span></span>
- <span data-ttu-id="46c08-153">应用共享</span><span class="sxs-lookup"><span data-stu-id="46c08-153">App Sharing</span></span>
- <span data-ttu-id="46c08-154">Web</span><span class="sxs-lookup"><span data-stu-id="46c08-154">Web</span></span>
- <span data-ttu-id="46c08-155">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="46c08-155">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="46c08-156">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="46c08-156">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="46c08-157">JSON</span><span class="sxs-lookup"><span data-stu-id="46c08-157">JSON</span></span>

<span data-ttu-id="46c08-158">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="46c08-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c08-159">示例</span><span class="sxs-lookup"><span data-stu-id="46c08-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="46c08-160">CSV</span><span class="sxs-lookup"><span data-stu-id="46c08-160">CSV</span></span>

<span data-ttu-id="46c08-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="46c08-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="46c08-162">请求</span><span class="sxs-lookup"><span data-stu-id="46c08-162">Request</span></span>

<span data-ttu-id="46c08-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46c08-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46c08-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="46c08-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46c08-165">C#</span><span class="sxs-lookup"><span data-stu-id="46c08-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46c08-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46c08-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46c08-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46c08-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46c08-168">响应</span><span class="sxs-lookup"><span data-stu-id="46c08-168">Response</span></span>

<span data-ttu-id="46c08-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="46c08-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="46c08-170">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="46c08-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="46c08-171">JSON</span><span class="sxs-lookup"><span data-stu-id="46c08-171">JSON</span></span>

<span data-ttu-id="46c08-172">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="46c08-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="46c08-173">请求</span><span class="sxs-lookup"><span data-stu-id="46c08-173">Request</span></span>

<span data-ttu-id="46c08-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46c08-174">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46c08-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="46c08-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46c08-176">C#</span><span class="sxs-lookup"><span data-stu-id="46c08-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46c08-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46c08-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46c08-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46c08-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46c08-179">响应</span><span class="sxs-lookup"><span data-stu-id="46c08-179">Response</span></span>

<span data-ttu-id="46c08-180">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="46c08-180">The following is an example of the response.</span></span>

> <span data-ttu-id="46c08-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="46c08-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
