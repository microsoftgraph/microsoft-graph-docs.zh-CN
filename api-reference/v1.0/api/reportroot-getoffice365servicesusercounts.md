---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2807e1958f6b015dff475b0831e1f20f2365ca17
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268619"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="f8698-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="f8698-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="f8698-104">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="f8698-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="f8698-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="f8698-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8698-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8698-106">Permissions</span></span>

<span data-ttu-id="f8698-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8698-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8698-109">Permission type</span></span>                        | <span data-ttu-id="f8698-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8698-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8698-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8698-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8698-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8698-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f8698-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8698-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8698-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8698-114">Not supported.</span></span>                           |
| <span data-ttu-id="f8698-115">应用</span><span class="sxs-lookup"><span data-stu-id="f8698-115">Application</span></span>                            | <span data-ttu-id="f8698-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8698-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f8698-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8698-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f8698-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="f8698-118">Function parameters</span></span>

<span data-ttu-id="f8698-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f8698-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f8698-120">参数</span><span class="sxs-lookup"><span data-stu-id="f8698-120">Parameter</span></span> | <span data-ttu-id="f8698-121">类型</span><span class="sxs-lookup"><span data-stu-id="f8698-121">Type</span></span>   | <span data-ttu-id="f8698-122">说明</span><span class="sxs-lookup"><span data-stu-id="f8698-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8698-123">period</span><span class="sxs-lookup"><span data-stu-id="f8698-123">period</span></span>    | <span data-ttu-id="f8698-124">string</span><span class="sxs-lookup"><span data-stu-id="f8698-124">string</span></span> | <span data-ttu-id="f8698-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8698-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8698-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f8698-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8698-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8698-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8698-128">必需。</span><span class="sxs-lookup"><span data-stu-id="f8698-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f8698-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8698-129">Request headers</span></span>

| <span data-ttu-id="f8698-130">名称</span><span class="sxs-lookup"><span data-stu-id="f8698-130">Name</span></span>          | <span data-ttu-id="f8698-131">说明</span><span class="sxs-lookup"><span data-stu-id="f8698-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f8698-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8698-132">Authorization</span></span> | <span data-ttu-id="f8698-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8698-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f8698-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f8698-135">If-None-Match</span></span> | <span data-ttu-id="f8698-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f8698-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f8698-137">可选。</span><span class="sxs-lookup"><span data-stu-id="f8698-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f8698-138">响应</span><span class="sxs-lookup"><span data-stu-id="f8698-138">Response</span></span>

<span data-ttu-id="f8698-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f8698-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8698-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f8698-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8698-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f8698-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f8698-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f8698-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8698-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f8698-143">Report Refresh Date</span></span>
- <span data-ttu-id="f8698-144">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-144">Exchange Active</span></span>
- <span data-ttu-id="f8698-145">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-145">Exchange Inactive</span></span>
- <span data-ttu-id="f8698-146">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-146">OneDrive Active</span></span>
- <span data-ttu-id="f8698-147">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-147">OneDrive Inactive</span></span>
- <span data-ttu-id="f8698-148">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-148">SharePoint Active</span></span>
- <span data-ttu-id="f8698-149">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-149">SharePoint Inactive</span></span>
- <span data-ttu-id="f8698-150">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-150">Skype For Business Active</span></span>
- <span data-ttu-id="f8698-151">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="f8698-152">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-152">Yammer Active</span></span>
- <span data-ttu-id="f8698-153">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-153">Yammer Inactive</span></span>
- <span data-ttu-id="f8698-154">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-154">Teams Active</span></span>
- <span data-ttu-id="f8698-155">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="f8698-155">Teams Inactive</span></span>
- <span data-ttu-id="f8698-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="f8698-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f8698-157">示例</span><span class="sxs-lookup"><span data-stu-id="f8698-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8698-158">请求</span><span class="sxs-lookup"><span data-stu-id="f8698-158">Request</span></span>

<span data-ttu-id="f8698-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8698-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f8698-160">响应</span><span class="sxs-lookup"><span data-stu-id="f8698-160">Response</span></span>

<span data-ttu-id="f8698-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8698-161">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8698-162">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8698-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8698-163">C#</span><span class="sxs-lookup"><span data-stu-id="f8698-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8698-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8698-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8698-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8698-165">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f8698-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f8698-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
