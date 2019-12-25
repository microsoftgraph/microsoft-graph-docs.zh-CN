---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型是团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d7489fe5de57ef8d1b9b3a9f435670333de42f91
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867332"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="9cf2b-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="9cf2b-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf2b-105">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="9cf2b-106">活动类型是团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cf2b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9cf2b-107">Permissions</span></span>

<span data-ttu-id="9cf2b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cf2b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cf2b-110">Permission type</span></span>                        | <span data-ttu-id="9cf2b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cf2b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9cf2b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf2b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cf2b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cf2b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9cf2b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf2b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-115">Not supported.</span></span>                           |
| <span data-ttu-id="9cf2b-116">应用</span><span class="sxs-lookup"><span data-stu-id="9cf2b-116">Application</span></span>                            | <span data-ttu-id="9cf2b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cf2b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="9cf2b-118">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9cf2b-119">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9cf2b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cf2b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="9cf2b-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="9cf2b-121">Function parameters</span></span>

<span data-ttu-id="9cf2b-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9cf2b-123">参数</span><span class="sxs-lookup"><span data-stu-id="9cf2b-123">Parameter</span></span> | <span data-ttu-id="9cf2b-124">类型</span><span class="sxs-lookup"><span data-stu-id="9cf2b-124">Type</span></span>   | <span data-ttu-id="9cf2b-125">说明</span><span class="sxs-lookup"><span data-stu-id="9cf2b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9cf2b-126">period</span><span class="sxs-lookup"><span data-stu-id="9cf2b-126">period</span></span>    | <span data-ttu-id="9cf2b-127">string</span><span class="sxs-lookup"><span data-stu-id="9cf2b-127">string</span></span> | <span data-ttu-id="9cf2b-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9cf2b-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9cf2b-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9cf2b-131">必需。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-131">Required.</span></span> |

<span data-ttu-id="9cf2b-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9cf2b-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-133">The default output type is text/csv.</span></span> <span data-ttu-id="9cf2b-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cf2b-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cf2b-135">Request headers</span></span>

| <span data-ttu-id="9cf2b-136">名称</span><span class="sxs-lookup"><span data-stu-id="9cf2b-136">Name</span></span>          | <span data-ttu-id="9cf2b-137">说明</span><span class="sxs-lookup"><span data-stu-id="9cf2b-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9cf2b-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cf2b-138">Authorization</span></span> | <span data-ttu-id="9cf2b-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9cf2b-141">响应</span><span class="sxs-lookup"><span data-stu-id="9cf2b-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9cf2b-142">CSV</span><span class="sxs-lookup"><span data-stu-id="9cf2b-142">CSV</span></span>

<span data-ttu-id="9cf2b-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9cf2b-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9cf2b-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9cf2b-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9cf2b-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9cf2b-147">Report Refresh Date</span></span>
- <span data-ttu-id="9cf2b-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="9cf2b-148">Report Date</span></span>
- <span data-ttu-id="9cf2b-149">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="9cf2b-149">Team Chat Messages</span></span>
- <span data-ttu-id="9cf2b-150">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="9cf2b-150">Private Chat Messages</span></span>
- <span data-ttu-id="9cf2b-151">呼叫</span><span class="sxs-lookup"><span data-stu-id="9cf2b-151">Calls</span></span>
- <span data-ttu-id="9cf2b-152">会议</span><span class="sxs-lookup"><span data-stu-id="9cf2b-152">Meetings</span></span>
- <span data-ttu-id="9cf2b-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="9cf2b-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9cf2b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="9cf2b-154">JSON</span></span>

<span data-ttu-id="9cf2b-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-155">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf2b-156">示例</span><span class="sxs-lookup"><span data-stu-id="9cf2b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9cf2b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="9cf2b-157">CSV</span></span>

<span data-ttu-id="9cf2b-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9cf2b-159">请求</span><span class="sxs-lookup"><span data-stu-id="9cf2b-159">Request</span></span>

<span data-ttu-id="9cf2b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cf2b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf2b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cf2b-162">C#</span><span class="sxs-lookup"><span data-stu-id="9cf2b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cf2b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf2b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cf2b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf2b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cf2b-165">响应</span><span class="sxs-lookup"><span data-stu-id="9cf2b-165">Response</span></span>

<span data-ttu-id="9cf2b-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="9cf2b-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="9cf2b-168">JSON</span><span class="sxs-lookup"><span data-stu-id="9cf2b-168">JSON</span></span>

<span data-ttu-id="9cf2b-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9cf2b-170">请求</span><span class="sxs-lookup"><span data-stu-id="9cf2b-170">Request</span></span>

<span data-ttu-id="9cf2b-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cf2b-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf2b-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cf2b-173">C#</span><span class="sxs-lookup"><span data-stu-id="9cf2b-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cf2b-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf2b-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cf2b-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf2b-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cf2b-176">响应</span><span class="sxs-lookup"><span data-stu-id="9cf2b-176">Response</span></span>

<span data-ttu-id="9cf2b-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="9cf2b-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cf2b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
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
