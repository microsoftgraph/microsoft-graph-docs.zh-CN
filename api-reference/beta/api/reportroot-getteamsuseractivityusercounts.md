---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c64ada41cdc1bf766e3944c97c8026785bb9a73f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868921"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="298fe-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="298fe-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="298fe-105">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="298fe-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="298fe-106">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="298fe-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="298fe-107">权限</span><span class="sxs-lookup"><span data-stu-id="298fe-107">Permissions</span></span>

<span data-ttu-id="298fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="298fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="298fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="298fe-110">Permission type</span></span>                        | <span data-ttu-id="298fe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="298fe-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="298fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="298fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="298fe-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="298fe-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="298fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="298fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="298fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="298fe-115">Not supported.</span></span>                           |
| <span data-ttu-id="298fe-116">应用</span><span class="sxs-lookup"><span data-stu-id="298fe-116">Application</span></span>                            | <span data-ttu-id="298fe-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="298fe-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="298fe-118">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="298fe-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="298fe-119">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="298fe-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="298fe-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="298fe-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="298fe-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="298fe-121">Function parameters</span></span>

<span data-ttu-id="298fe-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="298fe-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="298fe-123">参数</span><span class="sxs-lookup"><span data-stu-id="298fe-123">Parameter</span></span> | <span data-ttu-id="298fe-124">类型</span><span class="sxs-lookup"><span data-stu-id="298fe-124">Type</span></span>   | <span data-ttu-id="298fe-125">说明</span><span class="sxs-lookup"><span data-stu-id="298fe-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="298fe-126">period</span><span class="sxs-lookup"><span data-stu-id="298fe-126">period</span></span>    | <span data-ttu-id="298fe-127">string</span><span class="sxs-lookup"><span data-stu-id="298fe-127">string</span></span> | <span data-ttu-id="298fe-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="298fe-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="298fe-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="298fe-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="298fe-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="298fe-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="298fe-131">必需。</span><span class="sxs-lookup"><span data-stu-id="298fe-131">Required.</span></span> |

<span data-ttu-id="298fe-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="298fe-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="298fe-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="298fe-133">The default output type is text/csv.</span></span> <span data-ttu-id="298fe-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="298fe-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="298fe-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="298fe-135">Request headers</span></span>

| <span data-ttu-id="298fe-136">名称</span><span class="sxs-lookup"><span data-stu-id="298fe-136">Name</span></span>          | <span data-ttu-id="298fe-137">说明</span><span class="sxs-lookup"><span data-stu-id="298fe-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="298fe-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="298fe-138">Authorization</span></span> | <span data-ttu-id="298fe-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="298fe-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="298fe-141">响应</span><span class="sxs-lookup"><span data-stu-id="298fe-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="298fe-142">CSV</span><span class="sxs-lookup"><span data-stu-id="298fe-142">CSV</span></span>

<span data-ttu-id="298fe-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="298fe-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="298fe-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="298fe-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="298fe-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="298fe-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="298fe-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="298fe-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="298fe-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="298fe-147">Report Refresh Date</span></span>
- <span data-ttu-id="298fe-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="298fe-148">Report Date</span></span>
- <span data-ttu-id="298fe-149">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="298fe-149">Team Chat Messages</span></span>
- <span data-ttu-id="298fe-150">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="298fe-150">Private Chat Messages</span></span>
- <span data-ttu-id="298fe-151">呼叫</span><span class="sxs-lookup"><span data-stu-id="298fe-151">Calls</span></span>
- <span data-ttu-id="298fe-152">会议</span><span class="sxs-lookup"><span data-stu-id="298fe-152">Meetings</span></span>
- <span data-ttu-id="298fe-153">其他操作</span><span class="sxs-lookup"><span data-stu-id="298fe-153">Other Actions</span></span>
- <span data-ttu-id="298fe-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="298fe-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="298fe-155">JSON</span><span class="sxs-lookup"><span data-stu-id="298fe-155">JSON</span></span>

<span data-ttu-id="298fe-156">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="298fe-156">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="298fe-157">示例</span><span class="sxs-lookup"><span data-stu-id="298fe-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="298fe-158">CSV</span><span class="sxs-lookup"><span data-stu-id="298fe-158">CSV</span></span>

<span data-ttu-id="298fe-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="298fe-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="298fe-160">请求</span><span class="sxs-lookup"><span data-stu-id="298fe-160">Request</span></span>

<span data-ttu-id="298fe-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="298fe-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="298fe-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="298fe-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="298fe-163">C#</span><span class="sxs-lookup"><span data-stu-id="298fe-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="298fe-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="298fe-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="298fe-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="298fe-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="298fe-166">响应</span><span class="sxs-lookup"><span data-stu-id="298fe-166">Response</span></span>

<span data-ttu-id="298fe-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="298fe-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="298fe-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="298fe-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="298fe-169">JSON</span><span class="sxs-lookup"><span data-stu-id="298fe-169">JSON</span></span>

<span data-ttu-id="298fe-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="298fe-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="298fe-171">请求</span><span class="sxs-lookup"><span data-stu-id="298fe-171">Request</span></span>

<span data-ttu-id="298fe-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="298fe-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="298fe-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="298fe-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="298fe-174">C#</span><span class="sxs-lookup"><span data-stu-id="298fe-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="298fe-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="298fe-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="298fe-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="298fe-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="298fe-177">响应</span><span class="sxs-lookup"><span data-stu-id="298fe-177">Response</span></span>

<span data-ttu-id="298fe-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="298fe-178">The following is an example of the response.</span></span>

> <span data-ttu-id="298fe-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="298fe-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
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
