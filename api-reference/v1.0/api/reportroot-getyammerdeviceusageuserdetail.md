---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fc9cc937278889242acca1efab49ca58d642ad23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975723"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="f4e46-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="f4e46-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="f4e46-104">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4e46-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="f4e46-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="f4e46-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4e46-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4e46-106">Permissions</span></span>

<span data-ttu-id="f4e46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4e46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4e46-109">Permission type</span></span>                        | <span data-ttu-id="f4e46-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4e46-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f4e46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4e46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4e46-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4e46-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f4e46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4e46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e46-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4e46-114">Not supported.</span></span>                           |
| <span data-ttu-id="f4e46-115">应用</span><span class="sxs-lookup"><span data-stu-id="f4e46-115">Application</span></span>                            | <span data-ttu-id="f4e46-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4e46-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f4e46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4e46-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f4e46-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f4e46-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f4e46-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="f4e46-119">Function parameters</span></span>

<span data-ttu-id="f4e46-120">在请求 URL 中，提供查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f4e46-120">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="f4e46-121">参数</span><span class="sxs-lookup"><span data-stu-id="f4e46-121">Parameter</span></span> | <span data-ttu-id="f4e46-122">类型</span><span class="sxs-lookup"><span data-stu-id="f4e46-122">Type</span></span>   | <span data-ttu-id="f4e46-123">说明</span><span class="sxs-lookup"><span data-stu-id="f4e46-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f4e46-124">period</span><span class="sxs-lookup"><span data-stu-id="f4e46-124">period</span></span>    | <span data-ttu-id="f4e46-125">string</span><span class="sxs-lookup"><span data-stu-id="f4e46-125">string</span></span> | <span data-ttu-id="f4e46-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f4e46-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f4e46-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f4e46-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f4e46-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f4e46-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f4e46-129">date</span><span class="sxs-lookup"><span data-stu-id="f4e46-129">date</span></span>      | <span data-ttu-id="f4e46-130">Date</span><span class="sxs-lookup"><span data-stu-id="f4e46-130">Date</span></span>   | <span data-ttu-id="f4e46-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="f4e46-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f4e46-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="f4e46-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f4e46-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="f4e46-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f4e46-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="f4e46-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4e46-135">请求头</span><span class="sxs-lookup"><span data-stu-id="f4e46-135">Request headers</span></span>

| <span data-ttu-id="f4e46-136">名称</span><span class="sxs-lookup"><span data-stu-id="f4e46-136">Name</span></span>          | <span data-ttu-id="f4e46-137">说明</span><span class="sxs-lookup"><span data-stu-id="f4e46-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f4e46-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e46-138">Authorization</span></span> | <span data-ttu-id="f4e46-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4e46-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f4e46-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f4e46-141">If-None-Match</span></span> | <span data-ttu-id="f4e46-142">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f4e46-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f4e46-143">可选。</span><span class="sxs-lookup"><span data-stu-id="f4e46-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f4e46-144">响应</span><span class="sxs-lookup"><span data-stu-id="f4e46-144">Response</span></span>

<span data-ttu-id="f4e46-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f4e46-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f4e46-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f4e46-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f4e46-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f4e46-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f4e46-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f4e46-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f4e46-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f4e46-149">Report Refresh Date</span></span>
- <span data-ttu-id="f4e46-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f4e46-150">User Principal Name</span></span>
- <span data-ttu-id="f4e46-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="f4e46-151">Display Name</span></span>
- <span data-ttu-id="f4e46-152">用户状态</span><span class="sxs-lookup"><span data-stu-id="f4e46-152">User State</span></span>
- <span data-ttu-id="f4e46-153">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="f4e46-153">State Change Date</span></span>
- <span data-ttu-id="f4e46-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="f4e46-154">Last Activity Date</span></span>
- <span data-ttu-id="f4e46-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="f4e46-155">Used Web</span></span>
- <span data-ttu-id="f4e46-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="f4e46-156">Used Windows Phone</span></span>
- <span data-ttu-id="f4e46-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="f4e46-157">Used Android Phone</span></span>
- <span data-ttu-id="f4e46-158">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="f4e46-158">Used iPhone</span></span>
- <span data-ttu-id="f4e46-159">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="f4e46-159">Used iPad</span></span>
- <span data-ttu-id="f4e46-160">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="f4e46-160">Used Others</span></span>
- <span data-ttu-id="f4e46-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="f4e46-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f4e46-162">示例</span><span class="sxs-lookup"><span data-stu-id="f4e46-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f4e46-163">请求</span><span class="sxs-lookup"><span data-stu-id="f4e46-163">Request</span></span>

<span data-ttu-id="f4e46-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4e46-164">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4e46-165">C#</span><span class="sxs-lookup"><span data-stu-id="f4e46-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4e46-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4e46-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4e46-167">目标-C</span><span class="sxs-lookup"><span data-stu-id="f4e46-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f4e46-168">Java</span><span class="sxs-lookup"><span data-stu-id="f4e46-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4e46-169">响应</span><span class="sxs-lookup"><span data-stu-id="f4e46-169">Response</span></span>

<span data-ttu-id="f4e46-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4e46-170">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="f4e46-171">请求</span><span class="sxs-lookup"><span data-stu-id="f4e46-171">Request</span></span>

<span data-ttu-id="f4e46-172">如果使用`date`参数调用, 则报告的作用范围为给定日期的使用情况。</span><span class="sxs-lookup"><span data-stu-id="f4e46-172">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="f4e46-173">响应</span><span class="sxs-lookup"><span data-stu-id="f4e46-173">Response</span></span>

<span data-ttu-id="f4e46-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4e46-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="f4e46-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f4e46-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
