---
title: 'reportRoot: getYammerActivityCounts'
description: 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d861bdb51990a8e143bcbd978e69786d210dfc35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882980"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="1a52a-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="1a52a-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="1a52a-104">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="1a52a-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="1a52a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="1a52a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a52a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a52a-106">Permissions</span></span>

<span data-ttu-id="1a52a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a52a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a52a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a52a-109">Permission type</span></span>                        | <span data-ttu-id="1a52a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a52a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1a52a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a52a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a52a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a52a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1a52a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a52a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a52a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a52a-114">Not supported.</span></span>                           |
| <span data-ttu-id="1a52a-115">应用</span><span class="sxs-lookup"><span data-stu-id="1a52a-115">Application</span></span>                            | <span data-ttu-id="1a52a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a52a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1a52a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a52a-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1a52a-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1a52a-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1a52a-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="1a52a-119">Function parameters</span></span>

<span data-ttu-id="1a52a-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1a52a-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1a52a-121">参数</span><span class="sxs-lookup"><span data-stu-id="1a52a-121">Parameter</span></span> | <span data-ttu-id="1a52a-122">类型</span><span class="sxs-lookup"><span data-stu-id="1a52a-122">Type</span></span>   | <span data-ttu-id="1a52a-123">说明</span><span class="sxs-lookup"><span data-stu-id="1a52a-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1a52a-124">period</span><span class="sxs-lookup"><span data-stu-id="1a52a-124">period</span></span>    | <span data-ttu-id="1a52a-125">string</span><span class="sxs-lookup"><span data-stu-id="1a52a-125">string</span></span> | <span data-ttu-id="1a52a-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1a52a-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1a52a-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1a52a-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1a52a-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1a52a-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1a52a-129">必需。</span><span class="sxs-lookup"><span data-stu-id="1a52a-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1a52a-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a52a-130">Request headers</span></span>

| <span data-ttu-id="1a52a-131">名称</span><span class="sxs-lookup"><span data-stu-id="1a52a-131">Name</span></span>          | <span data-ttu-id="1a52a-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a52a-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1a52a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a52a-133">Authorization</span></span> | <span data-ttu-id="1a52a-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a52a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1a52a-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1a52a-136">If-None-Match</span></span> | <span data-ttu-id="1a52a-137">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a52a-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1a52a-138">可选。</span><span class="sxs-lookup"><span data-stu-id="1a52a-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1a52a-139">响应</span><span class="sxs-lookup"><span data-stu-id="1a52a-139">Response</span></span>

<span data-ttu-id="1a52a-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1a52a-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1a52a-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1a52a-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1a52a-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1a52a-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1a52a-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1a52a-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1a52a-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1a52a-144">Report Refresh Date</span></span>
- <span data-ttu-id="1a52a-145">已赞</span><span class="sxs-lookup"><span data-stu-id="1a52a-145">Liked</span></span>
- <span data-ttu-id="1a52a-146">已发布</span><span class="sxs-lookup"><span data-stu-id="1a52a-146">Posted</span></span>
- <span data-ttu-id="1a52a-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="1a52a-147">Read</span></span>
- <span data-ttu-id="1a52a-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="1a52a-148">Report Date</span></span>
- <span data-ttu-id="1a52a-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="1a52a-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1a52a-150">示例</span><span class="sxs-lookup"><span data-stu-id="1a52a-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1a52a-151">请求</span><span class="sxs-lookup"><span data-stu-id="1a52a-151">Request</span></span>

<span data-ttu-id="1a52a-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a52a-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a52a-153">C#</span><span class="sxs-lookup"><span data-stu-id="1a52a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a52a-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a52a-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a52a-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="1a52a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a52a-156">Java</span><span class="sxs-lookup"><span data-stu-id="1a52a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a52a-157">响应</span><span class="sxs-lookup"><span data-stu-id="1a52a-157">Response</span></span>

<span data-ttu-id="1a52a-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a52a-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="1a52a-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1a52a-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
