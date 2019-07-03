---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: 获取使用情况趋势，即组织中召开的会话的次数和类型。 会话类型包括 IM、音频、视频、应用共享和文件传输。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f1f1d104f85e85a475afd258b9428ce0971ba497
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444454"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="92e23-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="92e23-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="92e23-105">获取使用情况趋势，即组织中召开的会话的次数和类型。</span><span class="sxs-lookup"><span data-stu-id="92e23-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="92e23-106">会话类型包括 IM、音频、视频、应用共享和文件传输。</span><span class="sxs-lookup"><span data-stu-id="92e23-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="92e23-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="92e23-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="92e23-108">权限</span><span class="sxs-lookup"><span data-stu-id="92e23-108">Permissions</span></span>

<span data-ttu-id="92e23-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92e23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92e23-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92e23-111">Permission type</span></span>                        | <span data-ttu-id="92e23-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92e23-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="92e23-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92e23-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="92e23-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92e23-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="92e23-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92e23-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92e23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e23-116">Not supported.</span></span>                           |
| <span data-ttu-id="92e23-117">应用</span><span class="sxs-lookup"><span data-stu-id="92e23-117">Application</span></span>                            | <span data-ttu-id="92e23-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92e23-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="92e23-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92e23-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92e23-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="92e23-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="92e23-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="92e23-121">Function parameters</span></span>

<span data-ttu-id="92e23-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="92e23-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="92e23-123">参数</span><span class="sxs-lookup"><span data-stu-id="92e23-123">Parameter</span></span> | <span data-ttu-id="92e23-124">类型</span><span class="sxs-lookup"><span data-stu-id="92e23-124">Type</span></span>   | <span data-ttu-id="92e23-125">说明</span><span class="sxs-lookup"><span data-stu-id="92e23-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="92e23-126">period</span><span class="sxs-lookup"><span data-stu-id="92e23-126">period</span></span>    | <span data-ttu-id="92e23-127">string</span><span class="sxs-lookup"><span data-stu-id="92e23-127">string</span></span> | <span data-ttu-id="92e23-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="92e23-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="92e23-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="92e23-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="92e23-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="92e23-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="92e23-131">必需。</span><span class="sxs-lookup"><span data-stu-id="92e23-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="92e23-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="92e23-132">Request headers</span></span>

| <span data-ttu-id="92e23-133">名称</span><span class="sxs-lookup"><span data-stu-id="92e23-133">Name</span></span>          | <span data-ttu-id="92e23-134">说明</span><span class="sxs-lookup"><span data-stu-id="92e23-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="92e23-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e23-135">Authorization</span></span> | <span data-ttu-id="92e23-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="92e23-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="92e23-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="92e23-138">If-None-Match</span></span> | <span data-ttu-id="92e23-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="92e23-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="92e23-140">可选。</span><span class="sxs-lookup"><span data-stu-id="92e23-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="92e23-141">响应</span><span class="sxs-lookup"><span data-stu-id="92e23-141">Response</span></span>

<span data-ttu-id="92e23-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="92e23-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="92e23-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="92e23-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="92e23-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="92e23-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="92e23-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="92e23-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="92e23-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="92e23-146">Report Refresh Date</span></span>
- <span data-ttu-id="92e23-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="92e23-147">Report Date</span></span>
- <span data-ttu-id="92e23-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="92e23-148">Report Period</span></span>
- <span data-ttu-id="92e23-149">IM</span><span class="sxs-lookup"><span data-stu-id="92e23-149">IM</span></span>
- <span data-ttu-id="92e23-150">音频</span><span class="sxs-lookup"><span data-stu-id="92e23-150">Audio</span></span>
- <span data-ttu-id="92e23-151">视频</span><span class="sxs-lookup"><span data-stu-id="92e23-151">Video</span></span>
- <span data-ttu-id="92e23-152">应用共享</span><span class="sxs-lookup"><span data-stu-id="92e23-152">App Sharing</span></span>
- <span data-ttu-id="92e23-153">文件传输</span><span class="sxs-lookup"><span data-stu-id="92e23-153">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="92e23-154">示例</span><span class="sxs-lookup"><span data-stu-id="92e23-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="92e23-155">请求</span><span class="sxs-lookup"><span data-stu-id="92e23-155">Request</span></span>

<span data-ttu-id="92e23-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92e23-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92e23-157">C#</span><span class="sxs-lookup"><span data-stu-id="92e23-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92e23-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="92e23-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92e23-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="92e23-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92e23-160">响应</span><span class="sxs-lookup"><span data-stu-id="92e23-160">Response</span></span>

<span data-ttu-id="92e23-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92e23-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="92e23-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="92e23-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
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
