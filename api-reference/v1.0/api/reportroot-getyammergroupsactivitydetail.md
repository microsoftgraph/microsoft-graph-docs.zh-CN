---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d7d34a42129ee948c6a49e184421844b9b0c2797
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893872"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="bb981-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bb981-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="bb981-104">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bb981-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="bb981-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="bb981-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb981-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb981-106">Permissions</span></span>

<span data-ttu-id="bb981-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb981-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb981-109">Permission type</span></span>                        | <span data-ttu-id="bb981-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb981-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb981-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb981-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb981-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb981-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb981-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb981-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb981-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb981-114">Not supported.</span></span>                           |
| <span data-ttu-id="bb981-115">应用</span><span class="sxs-lookup"><span data-stu-id="bb981-115">Application</span></span>                            | <span data-ttu-id="bb981-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb981-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb981-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb981-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb981-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bb981-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bb981-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="bb981-119">Function parameters</span></span>

<span data-ttu-id="bb981-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bb981-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bb981-121">参数</span><span class="sxs-lookup"><span data-stu-id="bb981-121">Parameter</span></span> | <span data-ttu-id="bb981-122">类型</span><span class="sxs-lookup"><span data-stu-id="bb981-122">Type</span></span>   | <span data-ttu-id="bb981-123">说明</span><span class="sxs-lookup"><span data-stu-id="bb981-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb981-124">period</span><span class="sxs-lookup"><span data-stu-id="bb981-124">period</span></span>    | <span data-ttu-id="bb981-125">string</span><span class="sxs-lookup"><span data-stu-id="bb981-125">string</span></span> | <span data-ttu-id="bb981-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bb981-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb981-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bb981-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb981-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bb981-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bb981-129">date</span><span class="sxs-lookup"><span data-stu-id="bb981-129">date</span></span>      | <span data-ttu-id="bb981-130">Date</span><span class="sxs-lookup"><span data-stu-id="bb981-130">Date</span></span>   | <span data-ttu-id="bb981-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="bb981-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bb981-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="bb981-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bb981-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="bb981-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bb981-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="bb981-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb981-135">请求头</span><span class="sxs-lookup"><span data-stu-id="bb981-135">Request headers</span></span>

| <span data-ttu-id="bb981-136">名称</span><span class="sxs-lookup"><span data-stu-id="bb981-136">Name</span></span>          | <span data-ttu-id="bb981-137">说明</span><span class="sxs-lookup"><span data-stu-id="bb981-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bb981-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb981-138">Authorization</span></span> | <span data-ttu-id="bb981-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb981-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bb981-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bb981-141">If-None-Match</span></span> | <span data-ttu-id="bb981-142">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb981-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bb981-143">可选。</span><span class="sxs-lookup"><span data-stu-id="bb981-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bb981-144">响应</span><span class="sxs-lookup"><span data-stu-id="bb981-144">Response</span></span>

<span data-ttu-id="bb981-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bb981-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb981-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bb981-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb981-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bb981-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb981-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bb981-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bb981-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bb981-149">Report Refresh Date</span></span>
- <span data-ttu-id="bb981-150">组显示名称</span><span class="sxs-lookup"><span data-stu-id="bb981-150">Group Display Name</span></span>
- <span data-ttu-id="bb981-151">已删除</span><span class="sxs-lookup"><span data-stu-id="bb981-151">Is Deleted</span></span>
- <span data-ttu-id="bb981-152">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="bb981-152">Owner Principal Name</span></span>
- <span data-ttu-id="bb981-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="bb981-153">Last Activity Date</span></span>
- <span data-ttu-id="bb981-154">组类型</span><span class="sxs-lookup"><span data-stu-id="bb981-154">Group Type</span></span>
- <span data-ttu-id="bb981-155">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="bb981-155">Office 365 Connected</span></span>
- <span data-ttu-id="bb981-156">成员数</span><span class="sxs-lookup"><span data-stu-id="bb981-156">Member Count</span></span>
- <span data-ttu-id="bb981-157">已发布数</span><span class="sxs-lookup"><span data-stu-id="bb981-157">Posted Count</span></span>
- <span data-ttu-id="bb981-158">已阅读数</span><span class="sxs-lookup"><span data-stu-id="bb981-158">Read Count</span></span>
- <span data-ttu-id="bb981-159">已赞数</span><span class="sxs-lookup"><span data-stu-id="bb981-159">Liked Count</span></span>
- <span data-ttu-id="bb981-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="bb981-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb981-161">示例</span><span class="sxs-lookup"><span data-stu-id="bb981-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb981-162">请求</span><span class="sxs-lookup"><span data-stu-id="bb981-162">Request</span></span>

<span data-ttu-id="bb981-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb981-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb981-164">C#</span><span class="sxs-lookup"><span data-stu-id="bb981-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb981-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb981-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb981-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="bb981-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb981-167">Java</span><span class="sxs-lookup"><span data-stu-id="bb981-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb981-168">响应</span><span class="sxs-lookup"><span data-stu-id="bb981-168">Response</span></span>

<span data-ttu-id="bb981-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb981-169">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="bb981-170">请求</span><span class="sxs-lookup"><span data-stu-id="bb981-170">Request</span></span>
<span data-ttu-id="bb981-171">如果通过调用`date`, 则报告将作用域限定为给定日期的活动。</span><span class="sxs-lookup"><span data-stu-id="bb981-171">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="bb981-172">响应</span><span class="sxs-lookup"><span data-stu-id="bb981-172">Response</span></span>

<span data-ttu-id="bb981-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb981-173">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bb981-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bb981-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
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
