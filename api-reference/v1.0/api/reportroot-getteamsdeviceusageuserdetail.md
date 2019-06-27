---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 00f60111ca906de3da5715c3c8b25bb2048a5941
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279049"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="23fc8-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="23fc8-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="23fc8-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23fc8-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="23fc8-105">权限</span><span class="sxs-lookup"><span data-stu-id="23fc8-105">Permissions</span></span>

<span data-ttu-id="23fc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23fc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23fc8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23fc8-108">Permission type</span></span>                        | <span data-ttu-id="23fc8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23fc8-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23fc8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23fc8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23fc8-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23fc8-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23fc8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23fc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23fc8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="23fc8-113">Not supported.</span></span>                           |
| <span data-ttu-id="23fc8-114">应用</span><span class="sxs-lookup"><span data-stu-id="23fc8-114">Application</span></span>                            | <span data-ttu-id="23fc8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23fc8-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="23fc8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23fc8-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="23fc8-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="23fc8-117">Function parameters</span></span>

<span data-ttu-id="23fc8-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="23fc8-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="23fc8-119">参数</span><span class="sxs-lookup"><span data-stu-id="23fc8-119">Parameter</span></span> | <span data-ttu-id="23fc8-120">类型</span><span class="sxs-lookup"><span data-stu-id="23fc8-120">Type</span></span>   | <span data-ttu-id="23fc8-121">说明</span><span class="sxs-lookup"><span data-stu-id="23fc8-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23fc8-122">period</span><span class="sxs-lookup"><span data-stu-id="23fc8-122">period</span></span>    | <span data-ttu-id="23fc8-123">string</span><span class="sxs-lookup"><span data-stu-id="23fc8-123">string</span></span> | <span data-ttu-id="23fc8-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="23fc8-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23fc8-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="23fc8-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23fc8-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="23fc8-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="23fc8-127">date</span><span class="sxs-lookup"><span data-stu-id="23fc8-127">date</span></span>      | <span data-ttu-id="23fc8-128">Date</span><span class="sxs-lookup"><span data-stu-id="23fc8-128">Date</span></span>   | <span data-ttu-id="23fc8-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="23fc8-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="23fc8-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="23fc8-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="23fc8-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="23fc8-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="23fc8-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="23fc8-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23fc8-133">请求头</span><span class="sxs-lookup"><span data-stu-id="23fc8-133">Request headers</span></span>

| <span data-ttu-id="23fc8-134">名称</span><span class="sxs-lookup"><span data-stu-id="23fc8-134">Name</span></span>          | <span data-ttu-id="23fc8-135">说明</span><span class="sxs-lookup"><span data-stu-id="23fc8-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23fc8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="23fc8-136">Authorization</span></span> | <span data-ttu-id="23fc8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23fc8-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23fc8-139">响应</span><span class="sxs-lookup"><span data-stu-id="23fc8-139">Response</span></span>

<span data-ttu-id="23fc8-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="23fc8-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23fc8-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="23fc8-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23fc8-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="23fc8-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23fc8-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="23fc8-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="23fc8-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="23fc8-144">Report Refresh Date</span></span>
- <span data-ttu-id="23fc8-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="23fc8-145">User Principal Name</span></span>
- <span data-ttu-id="23fc8-146">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="23fc8-146">Last Activity Date</span></span>
- <span data-ttu-id="23fc8-147">已删除</span><span class="sxs-lookup"><span data-stu-id="23fc8-147">Is Deleted</span></span>
- <span data-ttu-id="23fc8-148">删除日期</span><span class="sxs-lookup"><span data-stu-id="23fc8-148">Deleted Date</span></span>
- <span data-ttu-id="23fc8-149">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="23fc8-149">Used Web</span></span>
- <span data-ttu-id="23fc8-150">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="23fc8-150">Used Windows Phone</span></span>
- <span data-ttu-id="23fc8-151">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="23fc8-151">Used iOS</span></span>
- <span data-ttu-id="23fc8-152">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="23fc8-152">Used Mac</span></span>
- <span data-ttu-id="23fc8-153">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="23fc8-153">Used Android Phone</span></span>
- <span data-ttu-id="23fc8-154">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="23fc8-154">Used Windows</span></span>
- <span data-ttu-id="23fc8-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="23fc8-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="23fc8-156">示例</span><span class="sxs-lookup"><span data-stu-id="23fc8-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="23fc8-157">请求</span><span class="sxs-lookup"><span data-stu-id="23fc8-157">Request</span></span>

<span data-ttu-id="23fc8-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="23fc8-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="23fc8-159">响应</span><span class="sxs-lookup"><span data-stu-id="23fc8-159">Response</span></span>

<span data-ttu-id="23fc8-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="23fc8-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="23fc8-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="23fc8-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23fc8-162">C#</span><span class="sxs-lookup"><span data-stu-id="23fc8-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23fc8-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="23fc8-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="23fc8-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="23fc8-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="23fc8-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="23fc8-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
