---
title: 'reportRoot: getEmailActivityUserDetail'
description: 获取用户执行的电子邮件活动的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ce7a5f71e217b639080b7ae51210a1d2397a717f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607075"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="b5d69-103">reportRoot：getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b5d69-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="b5d69-104">获取用户执行的电子邮件活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b5d69-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="b5d69-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="b5d69-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5d69-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5d69-106">Permissions</span></span>

<span data-ttu-id="b5d69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5d69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5d69-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5d69-109">Permission type</span></span>                        | <span data-ttu-id="b5d69-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5d69-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b5d69-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d69-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5d69-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d69-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b5d69-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5d69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d69-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5d69-114">Not supported.</span></span>                           |
| <span data-ttu-id="b5d69-115">应用</span><span class="sxs-lookup"><span data-stu-id="b5d69-115">Application</span></span>                            | <span data-ttu-id="b5d69-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d69-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b5d69-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5d69-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b5d69-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="b5d69-118">Function parameters</span></span>

<span data-ttu-id="b5d69-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b5d69-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b5d69-120">参数</span><span class="sxs-lookup"><span data-stu-id="b5d69-120">Parameter</span></span> | <span data-ttu-id="b5d69-121">类型</span><span class="sxs-lookup"><span data-stu-id="b5d69-121">Type</span></span>   | <span data-ttu-id="b5d69-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5d69-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b5d69-123">period</span><span class="sxs-lookup"><span data-stu-id="b5d69-123">period</span></span>    | <span data-ttu-id="b5d69-124">string</span><span class="sxs-lookup"><span data-stu-id="b5d69-124">string</span></span> | <span data-ttu-id="b5d69-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b5d69-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b5d69-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b5d69-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b5d69-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b5d69-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b5d69-128">date</span><span class="sxs-lookup"><span data-stu-id="b5d69-128">date</span></span>      | <span data-ttu-id="b5d69-129">Date</span><span class="sxs-lookup"><span data-stu-id="b5d69-129">Date</span></span>   | <span data-ttu-id="b5d69-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b5d69-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b5d69-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b5d69-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b5d69-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b5d69-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b5d69-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b5d69-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5d69-134">请求头</span><span class="sxs-lookup"><span data-stu-id="b5d69-134">Request headers</span></span>

| <span data-ttu-id="b5d69-135">名称</span><span class="sxs-lookup"><span data-stu-id="b5d69-135">Name</span></span>          | <span data-ttu-id="b5d69-136">说明</span><span class="sxs-lookup"><span data-stu-id="b5d69-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b5d69-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d69-137">Authorization</span></span> | <span data-ttu-id="b5d69-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5d69-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b5d69-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b5d69-140">If-None-Match</span></span> | <span data-ttu-id="b5d69-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b5d69-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b5d69-142">可选。</span><span class="sxs-lookup"><span data-stu-id="b5d69-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b5d69-143">响应</span><span class="sxs-lookup"><span data-stu-id="b5d69-143">Response</span></span>

<span data-ttu-id="b5d69-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b5d69-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b5d69-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b5d69-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b5d69-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b5d69-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b5d69-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b5d69-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b5d69-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b5d69-148">Report Refresh Date</span></span>
- <span data-ttu-id="b5d69-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b5d69-149">User Principal Name</span></span>
- <span data-ttu-id="b5d69-150">显示名称</span><span class="sxs-lookup"><span data-stu-id="b5d69-150">Display Name</span></span>
- <span data-ttu-id="b5d69-151">已删除</span><span class="sxs-lookup"><span data-stu-id="b5d69-151">Is Deleted</span></span>
- <span data-ttu-id="b5d69-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="b5d69-152">Deleted Date</span></span>
- <span data-ttu-id="b5d69-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b5d69-153">Last Activity Date</span></span>
- <span data-ttu-id="b5d69-154">已发送数</span><span class="sxs-lookup"><span data-stu-id="b5d69-154">Send Count</span></span>
- <span data-ttu-id="b5d69-155">已接收数</span><span class="sxs-lookup"><span data-stu-id="b5d69-155">Receive Count</span></span>
- <span data-ttu-id="b5d69-156">已阅读数</span><span class="sxs-lookup"><span data-stu-id="b5d69-156">Read Count</span></span>
- <span data-ttu-id="b5d69-157">分配的产品</span><span class="sxs-lookup"><span data-stu-id="b5d69-157">Assigned Products</span></span>
- <span data-ttu-id="b5d69-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="b5d69-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b5d69-159">示例</span><span class="sxs-lookup"><span data-stu-id="b5d69-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b5d69-160">请求</span><span class="sxs-lookup"><span data-stu-id="b5d69-160">Request</span></span>

<span data-ttu-id="b5d69-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5d69-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b5d69-162">响应</span><span class="sxs-lookup"><span data-stu-id="b5d69-162">Response</span></span>

<span data-ttu-id="b5d69-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b5d69-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5d69-164">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b5d69-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5d69-165">C#</span><span class="sxs-lookup"><span data-stu-id="b5d69-165">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5d69-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5d69-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="b5d69-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b5d69-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
