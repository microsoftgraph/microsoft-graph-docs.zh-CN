---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 159ea091a233168744d0ecbcbb4fcdbb55be837b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454949"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="7cb68-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7cb68-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="7cb68-105">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="7cb68-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="7cb68-106">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="7cb68-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="7cb68-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="7cb68-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cb68-108">权限</span><span class="sxs-lookup"><span data-stu-id="7cb68-108">Permissions</span></span>

<span data-ttu-id="7cb68-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cb68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7cb68-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cb68-111">Permission type</span></span>                        | <span data-ttu-id="7cb68-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cb68-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7cb68-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb68-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cb68-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cb68-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7cb68-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cb68-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cb68-116">Not supported.</span></span>                           |
| <span data-ttu-id="7cb68-117">应用</span><span class="sxs-lookup"><span data-stu-id="7cb68-117">Application</span></span>                            | <span data-ttu-id="7cb68-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cb68-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7cb68-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cb68-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7cb68-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7cb68-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7cb68-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="7cb68-121">Function parameters</span></span>

<span data-ttu-id="7cb68-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7cb68-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7cb68-123">参数</span><span class="sxs-lookup"><span data-stu-id="7cb68-123">Parameter</span></span> | <span data-ttu-id="7cb68-124">类型</span><span class="sxs-lookup"><span data-stu-id="7cb68-124">Type</span></span>   | <span data-ttu-id="7cb68-125">说明</span><span class="sxs-lookup"><span data-stu-id="7cb68-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7cb68-126">period</span><span class="sxs-lookup"><span data-stu-id="7cb68-126">period</span></span>    | <span data-ttu-id="7cb68-127">string</span><span class="sxs-lookup"><span data-stu-id="7cb68-127">string</span></span> | <span data-ttu-id="7cb68-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7cb68-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7cb68-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7cb68-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7cb68-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7cb68-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7cb68-131">必需。</span><span class="sxs-lookup"><span data-stu-id="7cb68-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7cb68-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cb68-132">Request headers</span></span>

| <span data-ttu-id="7cb68-133">名称</span><span class="sxs-lookup"><span data-stu-id="7cb68-133">Name</span></span>          | <span data-ttu-id="7cb68-134">说明</span><span class="sxs-lookup"><span data-stu-id="7cb68-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7cb68-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cb68-135">Authorization</span></span> | <span data-ttu-id="7cb68-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cb68-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7cb68-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7cb68-138">If-None-Match</span></span> | <span data-ttu-id="7cb68-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7cb68-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7cb68-140">可选。</span><span class="sxs-lookup"><span data-stu-id="7cb68-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7cb68-141">响应</span><span class="sxs-lookup"><span data-stu-id="7cb68-141">Response</span></span>

<span data-ttu-id="7cb68-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7cb68-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7cb68-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7cb68-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7cb68-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7cb68-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7cb68-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7cb68-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7cb68-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7cb68-146">Report Refresh Date</span></span>
- <span data-ttu-id="7cb68-147">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="7cb68-147">Visited Page</span></span>
- <span data-ttu-id="7cb68-148">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="7cb68-148">Viewed Or Edited</span></span>
- <span data-ttu-id="7cb68-149">已同步</span><span class="sxs-lookup"><span data-stu-id="7cb68-149">Synced</span></span>
- <span data-ttu-id="7cb68-150">已内部共享</span><span class="sxs-lookup"><span data-stu-id="7cb68-150">Shared Internally</span></span>
- <span data-ttu-id="7cb68-151">已外部共享</span><span class="sxs-lookup"><span data-stu-id="7cb68-151">Shared Externally</span></span>
- <span data-ttu-id="7cb68-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="7cb68-152">Report Date</span></span>
- <span data-ttu-id="7cb68-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="7cb68-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7cb68-154">示例</span><span class="sxs-lookup"><span data-stu-id="7cb68-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7cb68-155">请求</span><span class="sxs-lookup"><span data-stu-id="7cb68-155">Request</span></span>

<span data-ttu-id="7cb68-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7cb68-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7cb68-157">C#</span><span class="sxs-lookup"><span data-stu-id="7cb68-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7cb68-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="7cb68-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7cb68-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="7cb68-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7cb68-160">响应</span><span class="sxs-lookup"><span data-stu-id="7cb68-160">Response</span></span>

<span data-ttu-id="7cb68-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7cb68-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="7cb68-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7cb68-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
