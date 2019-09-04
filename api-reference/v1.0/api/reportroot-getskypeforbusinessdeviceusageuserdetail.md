---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: 获取用户的 Skype for Business 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e4075ae4679850b9f46ba75f0934baa4e5f53ba6
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729526"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="18b13-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="18b13-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="18b13-104">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="18b13-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="18b13-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="18b13-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="18b13-106">权限</span><span class="sxs-lookup"><span data-stu-id="18b13-106">Permissions</span></span>

<span data-ttu-id="18b13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18b13-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18b13-109">Permission type</span></span>                        | <span data-ttu-id="18b13-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18b13-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="18b13-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18b13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18b13-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="18b13-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="18b13-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18b13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18b13-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18b13-114">Not supported.</span></span>                           |
| <span data-ttu-id="18b13-115">应用</span><span class="sxs-lookup"><span data-stu-id="18b13-115">Application</span></span>                            | <span data-ttu-id="18b13-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="18b13-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="18b13-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18b13-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="18b13-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="18b13-118">Function parameters</span></span>

<span data-ttu-id="18b13-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="18b13-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="18b13-120">参数</span><span class="sxs-lookup"><span data-stu-id="18b13-120">Parameter</span></span> | <span data-ttu-id="18b13-121">类型</span><span class="sxs-lookup"><span data-stu-id="18b13-121">Type</span></span>   | <span data-ttu-id="18b13-122">说明</span><span class="sxs-lookup"><span data-stu-id="18b13-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="18b13-123">period</span><span class="sxs-lookup"><span data-stu-id="18b13-123">period</span></span>    | <span data-ttu-id="18b13-124">string</span><span class="sxs-lookup"><span data-stu-id="18b13-124">string</span></span> | <span data-ttu-id="18b13-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="18b13-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="18b13-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="18b13-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="18b13-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="18b13-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="18b13-128">date</span><span class="sxs-lookup"><span data-stu-id="18b13-128">date</span></span>      | <span data-ttu-id="18b13-129">Date</span><span class="sxs-lookup"><span data-stu-id="18b13-129">Date</span></span>   | <span data-ttu-id="18b13-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="18b13-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="18b13-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="18b13-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="18b13-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="18b13-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="18b13-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="18b13-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18b13-134">请求头</span><span class="sxs-lookup"><span data-stu-id="18b13-134">Request headers</span></span>

| <span data-ttu-id="18b13-135">名称</span><span class="sxs-lookup"><span data-stu-id="18b13-135">Name</span></span>          | <span data-ttu-id="18b13-136">说明</span><span class="sxs-lookup"><span data-stu-id="18b13-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="18b13-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b13-137">Authorization</span></span> | <span data-ttu-id="18b13-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="18b13-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="18b13-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="18b13-140">If-None-Match</span></span> | <span data-ttu-id="18b13-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18b13-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="18b13-142">可选。</span><span class="sxs-lookup"><span data-stu-id="18b13-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="18b13-143">响应</span><span class="sxs-lookup"><span data-stu-id="18b13-143">Response</span></span>

<span data-ttu-id="18b13-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="18b13-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="18b13-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="18b13-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="18b13-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="18b13-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="18b13-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="18b13-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="18b13-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="18b13-148">Report Refresh Date</span></span>
- <span data-ttu-id="18b13-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="18b13-149">User Principal Name</span></span>
- <span data-ttu-id="18b13-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="18b13-150">Last Activity Date</span></span>
- <span data-ttu-id="18b13-151">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="18b13-151">Used Windows</span></span>
- <span data-ttu-id="18b13-152">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="18b13-152">Used Windows Phone</span></span>
- <span data-ttu-id="18b13-153">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="18b13-153">Used Android Phone</span></span>
- <span data-ttu-id="18b13-154">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="18b13-154">Used iPhone</span></span>
- <span data-ttu-id="18b13-155">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="18b13-155">Used iPad</span></span>
- <span data-ttu-id="18b13-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="18b13-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="18b13-157">示例</span><span class="sxs-lookup"><span data-stu-id="18b13-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="18b13-158">请求</span><span class="sxs-lookup"><span data-stu-id="18b13-158">Request</span></span>

<span data-ttu-id="18b13-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18b13-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="18b13-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="18b13-160">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18b13-161">C#</span><span class="sxs-lookup"><span data-stu-id="18b13-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18b13-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18b13-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18b13-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="18b13-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18b13-164">Java</span><span class="sxs-lookup"><span data-stu-id="18b13-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="18b13-165">响应</span><span class="sxs-lookup"><span data-stu-id="18b13-165">Response</span></span>

<span data-ttu-id="18b13-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18b13-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="18b13-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="18b13-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
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
