---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4cefc989469532bb184beda8db2b1165dc171bf4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461391"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="364a8-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="364a8-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="364a8-104">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="364a8-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="364a8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="364a8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="364a8-106">权限</span><span class="sxs-lookup"><span data-stu-id="364a8-106">Permissions</span></span>

<span data-ttu-id="364a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="364a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="364a8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="364a8-109">Permission type</span></span>                        | <span data-ttu-id="364a8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="364a8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="364a8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="364a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="364a8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="364a8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="364a8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="364a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="364a8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="364a8-114">Not supported.</span></span>                           |
| <span data-ttu-id="364a8-115">应用</span><span class="sxs-lookup"><span data-stu-id="364a8-115">Application</span></span>                            | <span data-ttu-id="364a8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="364a8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="364a8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="364a8-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="364a8-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="364a8-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="364a8-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="364a8-119">Function parameters</span></span>

<span data-ttu-id="364a8-120">在请求 URL 中，提供查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="364a8-120">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="364a8-121">参数</span><span class="sxs-lookup"><span data-stu-id="364a8-121">Parameter</span></span> | <span data-ttu-id="364a8-122">类型</span><span class="sxs-lookup"><span data-stu-id="364a8-122">Type</span></span>   | <span data-ttu-id="364a8-123">说明</span><span class="sxs-lookup"><span data-stu-id="364a8-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="364a8-124">period</span><span class="sxs-lookup"><span data-stu-id="364a8-124">period</span></span>    | <span data-ttu-id="364a8-125">string</span><span class="sxs-lookup"><span data-stu-id="364a8-125">string</span></span> | <span data-ttu-id="364a8-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="364a8-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="364a8-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="364a8-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="364a8-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="364a8-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="364a8-129">date</span><span class="sxs-lookup"><span data-stu-id="364a8-129">date</span></span>      | <span data-ttu-id="364a8-130">Date</span><span class="sxs-lookup"><span data-stu-id="364a8-130">Date</span></span>   | <span data-ttu-id="364a8-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="364a8-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="364a8-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="364a8-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="364a8-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="364a8-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="364a8-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="364a8-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="364a8-135">请求头</span><span class="sxs-lookup"><span data-stu-id="364a8-135">Request headers</span></span>

| <span data-ttu-id="364a8-136">名称</span><span class="sxs-lookup"><span data-stu-id="364a8-136">Name</span></span>          | <span data-ttu-id="364a8-137">说明</span><span class="sxs-lookup"><span data-stu-id="364a8-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="364a8-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="364a8-138">Authorization</span></span> | <span data-ttu-id="364a8-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="364a8-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="364a8-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="364a8-141">If-None-Match</span></span> | <span data-ttu-id="364a8-142">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="364a8-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="364a8-143">可选。</span><span class="sxs-lookup"><span data-stu-id="364a8-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="364a8-144">响应</span><span class="sxs-lookup"><span data-stu-id="364a8-144">Response</span></span>

<span data-ttu-id="364a8-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="364a8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="364a8-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="364a8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="364a8-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="364a8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="364a8-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="364a8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="364a8-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="364a8-149">Report Refresh Date</span></span>
- <span data-ttu-id="364a8-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="364a8-150">User Principal Name</span></span>
- <span data-ttu-id="364a8-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="364a8-151">Display Name</span></span>
- <span data-ttu-id="364a8-152">用户状态</span><span class="sxs-lookup"><span data-stu-id="364a8-152">User State</span></span>
- <span data-ttu-id="364a8-153">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="364a8-153">State Change Date</span></span>
- <span data-ttu-id="364a8-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="364a8-154">Last Activity Date</span></span>
- <span data-ttu-id="364a8-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="364a8-155">Used Web</span></span>
- <span data-ttu-id="364a8-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="364a8-156">Used Windows Phone</span></span>
- <span data-ttu-id="364a8-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="364a8-157">Used Android Phone</span></span>
- <span data-ttu-id="364a8-158">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="364a8-158">Used iPhone</span></span>
- <span data-ttu-id="364a8-159">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="364a8-159">Used iPad</span></span>
- <span data-ttu-id="364a8-160">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="364a8-160">Used Others</span></span>
- <span data-ttu-id="364a8-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="364a8-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="364a8-162">示例</span><span class="sxs-lookup"><span data-stu-id="364a8-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="364a8-163">请求</span><span class="sxs-lookup"><span data-stu-id="364a8-163">Request</span></span>

<span data-ttu-id="364a8-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="364a8-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="364a8-165">C#</span><span class="sxs-lookup"><span data-stu-id="364a8-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="364a8-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="364a8-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="364a8-167">目标-C</span><span class="sxs-lookup"><span data-stu-id="364a8-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="364a8-168">响应</span><span class="sxs-lookup"><span data-stu-id="364a8-168">Response</span></span>

<span data-ttu-id="364a8-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="364a8-169">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="364a8-170">请求</span><span class="sxs-lookup"><span data-stu-id="364a8-170">Request</span></span>

<span data-ttu-id="364a8-171">如果使用`date`参数调用, 则报告的作用范围为给定日期的使用情况。</span><span class="sxs-lookup"><span data-stu-id="364a8-171">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="364a8-172">响应</span><span class="sxs-lookup"><span data-stu-id="364a8-172">Response</span></span>

<span data-ttu-id="364a8-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="364a8-173">The following is an example of the response.</span></span>

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

<span data-ttu-id="364a8-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="364a8-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
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
