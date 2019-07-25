---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: 获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。 会话类型包括音频和视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eebfaf36a0f27236ca31906c9827d93160de410e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855667"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="8d159-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="8d159-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="8d159-105">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="8d159-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="8d159-106">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="8d159-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="8d159-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="8d159-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d159-108">权限</span><span class="sxs-lookup"><span data-stu-id="8d159-108">Permissions</span></span>

<span data-ttu-id="8d159-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d159-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d159-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d159-111">Permission type</span></span>                        | <span data-ttu-id="8d159-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d159-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8d159-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d159-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d159-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d159-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8d159-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d159-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d159-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d159-116">Not supported.</span></span>                           |
| <span data-ttu-id="8d159-117">应用</span><span class="sxs-lookup"><span data-stu-id="8d159-117">Application</span></span>                            | <span data-ttu-id="8d159-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d159-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8d159-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d159-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d159-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8d159-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8d159-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="8d159-121">Function parameters</span></span>

<span data-ttu-id="8d159-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="8d159-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8d159-123">参数</span><span class="sxs-lookup"><span data-stu-id="8d159-123">Parameter</span></span> | <span data-ttu-id="8d159-124">类型</span><span class="sxs-lookup"><span data-stu-id="8d159-124">Type</span></span>   | <span data-ttu-id="8d159-125">说明</span><span class="sxs-lookup"><span data-stu-id="8d159-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8d159-126">period</span><span class="sxs-lookup"><span data-stu-id="8d159-126">period</span></span>    | <span data-ttu-id="8d159-127">string</span><span class="sxs-lookup"><span data-stu-id="8d159-127">string</span></span> | <span data-ttu-id="8d159-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8d159-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8d159-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8d159-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8d159-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8d159-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8d159-131">必需。</span><span class="sxs-lookup"><span data-stu-id="8d159-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8d159-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d159-132">Request headers</span></span>

| <span data-ttu-id="8d159-133">名称</span><span class="sxs-lookup"><span data-stu-id="8d159-133">Name</span></span>          | <span data-ttu-id="8d159-134">说明</span><span class="sxs-lookup"><span data-stu-id="8d159-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8d159-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d159-135">Authorization</span></span> | <span data-ttu-id="8d159-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d159-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8d159-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8d159-138">If-None-Match</span></span> | <span data-ttu-id="8d159-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8d159-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8d159-140">可选。</span><span class="sxs-lookup"><span data-stu-id="8d159-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8d159-141">响应</span><span class="sxs-lookup"><span data-stu-id="8d159-141">Response</span></span>

<span data-ttu-id="8d159-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8d159-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8d159-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8d159-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8d159-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8d159-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8d159-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="8d159-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8d159-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8d159-146">Report Refresh Date</span></span>
- <span data-ttu-id="8d159-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="8d159-147">Report Date</span></span>
- <span data-ttu-id="8d159-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="8d159-148">Report Period</span></span>
- <span data-ttu-id="8d159-149">音频</span><span class="sxs-lookup"><span data-stu-id="8d159-149">Audio</span></span>
- <span data-ttu-id="8d159-150">视频</span><span class="sxs-lookup"><span data-stu-id="8d159-150">Video</span></span>

## <a name="example"></a><span data-ttu-id="8d159-151">示例</span><span class="sxs-lookup"><span data-stu-id="8d159-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8d159-152">请求</span><span class="sxs-lookup"><span data-stu-id="8d159-152">Request</span></span>

<span data-ttu-id="8d159-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d159-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d159-154">C#</span><span class="sxs-lookup"><span data-stu-id="8d159-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d159-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d159-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d159-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="8d159-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8d159-157">Java</span><span class="sxs-lookup"><span data-stu-id="8d159-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d159-158">响应</span><span class="sxs-lookup"><span data-stu-id="8d159-158">Response</span></span>

<span data-ttu-id="8d159-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d159-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="8d159-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8d159-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
