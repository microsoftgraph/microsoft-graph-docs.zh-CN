---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6de7fd82fbd54d6bfdfc1f52fab4fafe1967d6f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603509"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="ffc53-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="ffc53-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="ffc53-104">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ffc53-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="ffc53-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="ffc53-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffc53-106">权限</span><span class="sxs-lookup"><span data-stu-id="ffc53-106">Permissions</span></span>

<span data-ttu-id="ffc53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffc53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffc53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffc53-109">Permission type</span></span>                        | <span data-ttu-id="ffc53-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffc53-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ffc53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffc53-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc53-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ffc53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffc53-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffc53-114">Not supported.</span></span>                           |
| <span data-ttu-id="ffc53-115">应用</span><span class="sxs-lookup"><span data-stu-id="ffc53-115">Application</span></span>                            | <span data-ttu-id="ffc53-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc53-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ffc53-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffc53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ffc53-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="ffc53-118">Function parameters</span></span>

<span data-ttu-id="ffc53-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ffc53-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ffc53-120">参数</span><span class="sxs-lookup"><span data-stu-id="ffc53-120">Parameter</span></span> | <span data-ttu-id="ffc53-121">类型</span><span class="sxs-lookup"><span data-stu-id="ffc53-121">Type</span></span>   | <span data-ttu-id="ffc53-122">说明</span><span class="sxs-lookup"><span data-stu-id="ffc53-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ffc53-123">period</span><span class="sxs-lookup"><span data-stu-id="ffc53-123">period</span></span>    | <span data-ttu-id="ffc53-124">string</span><span class="sxs-lookup"><span data-stu-id="ffc53-124">string</span></span> | <span data-ttu-id="ffc53-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ffc53-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ffc53-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ffc53-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ffc53-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ffc53-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ffc53-128">date</span><span class="sxs-lookup"><span data-stu-id="ffc53-128">date</span></span>      | <span data-ttu-id="ffc53-129">Date</span><span class="sxs-lookup"><span data-stu-id="ffc53-129">Date</span></span>   | <span data-ttu-id="ffc53-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="ffc53-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ffc53-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="ffc53-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ffc53-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="ffc53-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ffc53-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="ffc53-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffc53-134">请求头</span><span class="sxs-lookup"><span data-stu-id="ffc53-134">Request headers</span></span>

| <span data-ttu-id="ffc53-135">名称</span><span class="sxs-lookup"><span data-stu-id="ffc53-135">Name</span></span>          | <span data-ttu-id="ffc53-136">说明</span><span class="sxs-lookup"><span data-stu-id="ffc53-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ffc53-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc53-137">Authorization</span></span> | <span data-ttu-id="ffc53-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ffc53-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ffc53-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ffc53-140">If-None-Match</span></span> | <span data-ttu-id="ffc53-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ffc53-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ffc53-142">可选。</span><span class="sxs-lookup"><span data-stu-id="ffc53-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ffc53-143">响应</span><span class="sxs-lookup"><span data-stu-id="ffc53-143">Response</span></span>

<span data-ttu-id="ffc53-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ffc53-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ffc53-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ffc53-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ffc53-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ffc53-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ffc53-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ffc53-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ffc53-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ffc53-148">Report Refresh Date</span></span>
- <span data-ttu-id="ffc53-149">组显示名称</span><span class="sxs-lookup"><span data-stu-id="ffc53-149">Group Display Name</span></span>
- <span data-ttu-id="ffc53-150">已删除</span><span class="sxs-lookup"><span data-stu-id="ffc53-150">Is Deleted</span></span>
- <span data-ttu-id="ffc53-151">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="ffc53-151">Owner Principal Name</span></span>
- <span data-ttu-id="ffc53-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="ffc53-152">Last Activity Date</span></span>
- <span data-ttu-id="ffc53-153">组类型</span><span class="sxs-lookup"><span data-stu-id="ffc53-153">Group Type</span></span>
- <span data-ttu-id="ffc53-154">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="ffc53-154">Office 365 Connected</span></span>
- <span data-ttu-id="ffc53-155">成员数</span><span class="sxs-lookup"><span data-stu-id="ffc53-155">Member Count</span></span>
- <span data-ttu-id="ffc53-156">已发布数</span><span class="sxs-lookup"><span data-stu-id="ffc53-156">Posted Count</span></span>
- <span data-ttu-id="ffc53-157">已阅读数</span><span class="sxs-lookup"><span data-stu-id="ffc53-157">Read Count</span></span>
- <span data-ttu-id="ffc53-158">已赞数</span><span class="sxs-lookup"><span data-stu-id="ffc53-158">Liked Count</span></span>
- <span data-ttu-id="ffc53-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="ffc53-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ffc53-160">示例</span><span class="sxs-lookup"><span data-stu-id="ffc53-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ffc53-161">请求</span><span class="sxs-lookup"><span data-stu-id="ffc53-161">Request</span></span>

<span data-ttu-id="ffc53-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ffc53-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ffc53-163">响应</span><span class="sxs-lookup"><span data-stu-id="ffc53-163">Response</span></span>

<span data-ttu-id="ffc53-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ffc53-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ffc53-165">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ffc53-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ffc53-166">语言</span><span class="sxs-lookup"><span data-stu-id="ffc53-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffc53-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="ffc53-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivityuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request"></a><span data-ttu-id="ffc53-168">请求</span><span class="sxs-lookup"><span data-stu-id="ffc53-168">Request</span></span>
<span data-ttu-id="ffc53-169">如果通过调用`date`, 则报告将作用域限定为给定日期的活动。</span><span class="sxs-lookup"><span data-stu-id="ffc53-169">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="ffc53-170">响应</span><span class="sxs-lookup"><span data-stu-id="ffc53-170">Response</span></span>

<span data-ttu-id="ffc53-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ffc53-171">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ffc53-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ffc53-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
