---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8dfd26bbc7de0806c7f41286800a9872d3eb9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639018"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="a2cc0-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a2cc0-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2cc0-104">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="a2cc0-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2cc0-106">权限</span><span class="sxs-lookup"><span data-stu-id="a2cc0-106">Permissions</span></span>

<span data-ttu-id="a2cc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2cc0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2cc0-109">Permission type</span></span>                        | <span data-ttu-id="a2cc0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2cc0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2cc0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2cc0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2cc0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2cc0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2cc0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2cc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2cc0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-114">Not supported.</span></span>                           |
| <span data-ttu-id="a2cc0-115">应用</span><span class="sxs-lookup"><span data-stu-id="a2cc0-115">Application</span></span>                            | <span data-ttu-id="a2cc0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2cc0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a2cc0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2cc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a2cc0-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-118">Function parameters</span></span>

<span data-ttu-id="a2cc0-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a2cc0-120">参数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-120">Parameter</span></span> | <span data-ttu-id="a2cc0-121">类型</span><span class="sxs-lookup"><span data-stu-id="a2cc0-121">Type</span></span>   | <span data-ttu-id="a2cc0-122">说明</span><span class="sxs-lookup"><span data-stu-id="a2cc0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2cc0-123">period</span><span class="sxs-lookup"><span data-stu-id="a2cc0-123">period</span></span>    | <span data-ttu-id="a2cc0-124">string</span><span class="sxs-lookup"><span data-stu-id="a2cc0-124">string</span></span> | <span data-ttu-id="a2cc0-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2cc0-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2cc0-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a2cc0-128">date</span><span class="sxs-lookup"><span data-stu-id="a2cc0-128">date</span></span>      | <span data-ttu-id="a2cc0-129">Date</span><span class="sxs-lookup"><span data-stu-id="a2cc0-129">Date</span></span>   | <span data-ttu-id="a2cc0-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a2cc0-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a2cc0-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a2cc0-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a2cc0-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2cc0-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-135">The default output type is text/csv.</span></span> <span data-ttu-id="a2cc0-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2cc0-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2cc0-137">Request headers</span></span>

| <span data-ttu-id="a2cc0-138">名称</span><span class="sxs-lookup"><span data-stu-id="a2cc0-138">Name</span></span>          | <span data-ttu-id="a2cc0-139">说明</span><span class="sxs-lookup"><span data-stu-id="a2cc0-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2cc0-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2cc0-140">Authorization</span></span> | <span data-ttu-id="a2cc0-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2cc0-143">响应</span><span class="sxs-lookup"><span data-stu-id="a2cc0-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2cc0-144">CSV</span><span class="sxs-lookup"><span data-stu-id="a2cc0-144">CSV</span></span>

<span data-ttu-id="a2cc0-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2cc0-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2cc0-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2cc0-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2cc0-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a2cc0-149">Report Refresh Date</span></span>
- <span data-ttu-id="a2cc0-150">组显示名称</span><span class="sxs-lookup"><span data-stu-id="a2cc0-150">Group Display Name</span></span>
- <span data-ttu-id="a2cc0-151">已删除</span><span class="sxs-lookup"><span data-stu-id="a2cc0-151">Is Deleted</span></span>
- <span data-ttu-id="a2cc0-152">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="a2cc0-152">Owner Principal Name</span></span>
- <span data-ttu-id="a2cc0-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a2cc0-153">Last Activity Date</span></span>
- <span data-ttu-id="a2cc0-154">组类型</span><span class="sxs-lookup"><span data-stu-id="a2cc0-154">Group Type</span></span>
- <span data-ttu-id="a2cc0-155">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="a2cc0-155">Office 365 Connected</span></span>
- <span data-ttu-id="a2cc0-156">成员数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-156">Member Count</span></span>
- <span data-ttu-id="a2cc0-157">已发布数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-157">Posted Count</span></span>
- <span data-ttu-id="a2cc0-158">已阅读数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-158">Read Count</span></span>
- <span data-ttu-id="a2cc0-159">已赞数</span><span class="sxs-lookup"><span data-stu-id="a2cc0-159">Liked Count</span></span>
- <span data-ttu-id="a2cc0-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="a2cc0-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a2cc0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="a2cc0-161">JSON</span></span>

<span data-ttu-id="a2cc0-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="a2cc0-163">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a2cc0-164">示例</span><span class="sxs-lookup"><span data-stu-id="a2cc0-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2cc0-165">CSV</span><span class="sxs-lookup"><span data-stu-id="a2cc0-165">CSV</span></span>

<span data-ttu-id="a2cc0-166">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2cc0-167">请求</span><span class="sxs-lookup"><span data-stu-id="a2cc0-167">Request</span></span>

<span data-ttu-id="a2cc0-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a2cc0-169">响应</span><span class="sxs-lookup"><span data-stu-id="a2cc0-169">Response</span></span>

<span data-ttu-id="a2cc0-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2cc0-171">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a2cc0-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2cc0-172">语言</span><span class="sxs-lookup"><span data-stu-id="a2cc0-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2cc0-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2cc0-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="a2cc0-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="a2cc0-175">JSON</span><span class="sxs-lookup"><span data-stu-id="a2cc0-175">JSON</span></span>

<span data-ttu-id="a2cc0-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2cc0-177">请求</span><span class="sxs-lookup"><span data-stu-id="a2cc0-177">Request</span></span>

<span data-ttu-id="a2cc0-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a2cc0-179">响应</span><span class="sxs-lookup"><span data-stu-id="a2cc0-179">Response</span></span>

<span data-ttu-id="a2cc0-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-180">The following is an example of the response.</span></span>

> <span data-ttu-id="a2cc0-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a2cc0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2cc0-183">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a2cc0-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2cc0-184">语言</span><span class="sxs-lookup"><span data-stu-id="a2cc0-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2cc0-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2cc0-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
