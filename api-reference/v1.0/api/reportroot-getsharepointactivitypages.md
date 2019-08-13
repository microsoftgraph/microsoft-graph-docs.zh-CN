---
title: 'reportRoot: getSharePointActivityPages'
description: 获取用户访问的唯一页面数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 265805dc757f4de81f6aaef4d8c0181388f37d36
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321739"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="70443-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="70443-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="70443-104">获取用户访问的唯一页面数。</span><span class="sxs-lookup"><span data-stu-id="70443-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="70443-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="70443-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="70443-106">权限</span><span class="sxs-lookup"><span data-stu-id="70443-106">Permissions</span></span>

<span data-ttu-id="70443-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70443-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70443-109">Permission type</span></span>                        | <span data-ttu-id="70443-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70443-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70443-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70443-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70443-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70443-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70443-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70443-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70443-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70443-114">Not supported.</span></span>                           |
| <span data-ttu-id="70443-115">应用</span><span class="sxs-lookup"><span data-stu-id="70443-115">Application</span></span>                            | <span data-ttu-id="70443-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70443-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70443-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70443-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="70443-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="70443-118">Function parameters</span></span>

<span data-ttu-id="70443-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="70443-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="70443-120">参数</span><span class="sxs-lookup"><span data-stu-id="70443-120">Parameter</span></span> | <span data-ttu-id="70443-121">类型</span><span class="sxs-lookup"><span data-stu-id="70443-121">Type</span></span>   | <span data-ttu-id="70443-122">说明</span><span class="sxs-lookup"><span data-stu-id="70443-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70443-123">period</span><span class="sxs-lookup"><span data-stu-id="70443-123">period</span></span>    | <span data-ttu-id="70443-124">string</span><span class="sxs-lookup"><span data-stu-id="70443-124">string</span></span> | <span data-ttu-id="70443-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="70443-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70443-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="70443-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70443-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="70443-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="70443-128">必需。</span><span class="sxs-lookup"><span data-stu-id="70443-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="70443-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="70443-129">Request headers</span></span>

| <span data-ttu-id="70443-130">名称</span><span class="sxs-lookup"><span data-stu-id="70443-130">Name</span></span>          | <span data-ttu-id="70443-131">说明</span><span class="sxs-lookup"><span data-stu-id="70443-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="70443-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="70443-132">Authorization</span></span> | <span data-ttu-id="70443-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="70443-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="70443-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="70443-135">If-None-Match</span></span> | <span data-ttu-id="70443-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="70443-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="70443-137">可选。</span><span class="sxs-lookup"><span data-stu-id="70443-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="70443-138">响应</span><span class="sxs-lookup"><span data-stu-id="70443-138">Response</span></span>

<span data-ttu-id="70443-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="70443-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70443-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="70443-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70443-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="70443-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70443-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="70443-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70443-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="70443-143">Report Refresh Date</span></span>
- <span data-ttu-id="70443-144">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="70443-144">Visited Page Count</span></span>
- <span data-ttu-id="70443-145">报表日期</span><span class="sxs-lookup"><span data-stu-id="70443-145">Report Date</span></span>
- <span data-ttu-id="70443-146">报表周期</span><span class="sxs-lookup"><span data-stu-id="70443-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="70443-147">示例</span><span class="sxs-lookup"><span data-stu-id="70443-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="70443-148">请求</span><span class="sxs-lookup"><span data-stu-id="70443-148">Request</span></span>

<span data-ttu-id="70443-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70443-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70443-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="70443-150">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivitypages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70443-151">C#</span><span class="sxs-lookup"><span data-stu-id="70443-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70443-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70443-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70443-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="70443-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70443-154">Java</span><span class="sxs-lookup"><span data-stu-id="70443-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivitypages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70443-155">响应</span><span class="sxs-lookup"><span data-stu-id="70443-155">Response</span></span>

<span data-ttu-id="70443-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70443-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="70443-157">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="70443-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
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
