---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: 获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。 会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0f6aafae83d47b44be57490b9a05351af00f9709
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276172"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="ad559-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ad559-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="ad559-105">获取使用情况趋势，即组织中用户召开和组织的会议会话的唯一用户数和类型。</span><span class="sxs-lookup"><span data-stu-id="ad559-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="ad559-106">会议会话类型包括 IM、音频/视频、应用共享、Web、第三方拨入/拨出和 Microsoft 拨入/拨出。</span><span class="sxs-lookup"><span data-stu-id="ad559-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="ad559-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议组织者活动](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)。</span><span class="sxs-lookup"><span data-stu-id="ad559-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad559-108">权限</span><span class="sxs-lookup"><span data-stu-id="ad559-108">Permissions</span></span>

<span data-ttu-id="ad559-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad559-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad559-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad559-111">Permission type</span></span>                        | <span data-ttu-id="ad559-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad559-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad559-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad559-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad559-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad559-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad559-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad559-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad559-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad559-116">Not supported.</span></span>                           |
| <span data-ttu-id="ad559-117">应用</span><span class="sxs-lookup"><span data-stu-id="ad559-117">Application</span></span>                            | <span data-ttu-id="ad559-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad559-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad559-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad559-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ad559-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="ad559-120">Function parameters</span></span>

<span data-ttu-id="ad559-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ad559-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ad559-122">参数</span><span class="sxs-lookup"><span data-stu-id="ad559-122">Parameter</span></span> | <span data-ttu-id="ad559-123">类型</span><span class="sxs-lookup"><span data-stu-id="ad559-123">Type</span></span>   | <span data-ttu-id="ad559-124">说明</span><span class="sxs-lookup"><span data-stu-id="ad559-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad559-125">period</span><span class="sxs-lookup"><span data-stu-id="ad559-125">period</span></span>    | <span data-ttu-id="ad559-126">string</span><span class="sxs-lookup"><span data-stu-id="ad559-126">string</span></span> | <span data-ttu-id="ad559-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ad559-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad559-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ad559-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad559-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ad559-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ad559-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ad559-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ad559-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad559-131">Request headers</span></span>

| <span data-ttu-id="ad559-132">名称</span><span class="sxs-lookup"><span data-stu-id="ad559-132">Name</span></span>          | <span data-ttu-id="ad559-133">说明</span><span class="sxs-lookup"><span data-stu-id="ad559-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ad559-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad559-134">Authorization</span></span> | <span data-ttu-id="ad559-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad559-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ad559-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ad559-137">If-None-Match</span></span> | <span data-ttu-id="ad559-138">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ad559-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ad559-139">可选。</span><span class="sxs-lookup"><span data-stu-id="ad559-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ad559-140">响应</span><span class="sxs-lookup"><span data-stu-id="ad559-140">Response</span></span>

<span data-ttu-id="ad559-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ad559-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad559-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ad559-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad559-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ad559-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad559-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ad559-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad559-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ad559-145">Report Refresh Date</span></span>
- <span data-ttu-id="ad559-146">报表日期</span><span class="sxs-lookup"><span data-stu-id="ad559-146">Report Date</span></span>
- <span data-ttu-id="ad559-147">报表周期</span><span class="sxs-lookup"><span data-stu-id="ad559-147">Report Period</span></span>
- <span data-ttu-id="ad559-148">IM</span><span class="sxs-lookup"><span data-stu-id="ad559-148">IM</span></span>
- <span data-ttu-id="ad559-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="ad559-149">Audio/Video</span></span>
- <span data-ttu-id="ad559-150">应用共享</span><span class="sxs-lookup"><span data-stu-id="ad559-150">App Sharing</span></span>
- <span data-ttu-id="ad559-151">Web</span><span class="sxs-lookup"><span data-stu-id="ad559-151">Web</span></span>
- <span data-ttu-id="ad559-152">第三方拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="ad559-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="ad559-153">Microsoft 拨入/拨出</span><span class="sxs-lookup"><span data-stu-id="ad559-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="ad559-154">示例</span><span class="sxs-lookup"><span data-stu-id="ad559-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ad559-155">请求</span><span class="sxs-lookup"><span data-stu-id="ad559-155">Request</span></span>

<span data-ttu-id="ad559-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad559-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ad559-157">响应</span><span class="sxs-lookup"><span data-stu-id="ad559-157">Response</span></span>

<span data-ttu-id="ad559-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad559-158">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad559-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ad559-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad559-160">C#</span><span class="sxs-lookup"><span data-stu-id="ad559-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad559-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad559-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ad559-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="ad559-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivityusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ad559-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ad559-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
