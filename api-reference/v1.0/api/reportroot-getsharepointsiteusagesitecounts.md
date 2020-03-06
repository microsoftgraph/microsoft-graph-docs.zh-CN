---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 482a7dcb319f243222b656be1880ed6e83eaa96c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510198"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="9c2ca-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="9c2ca-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="9c2ca-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2ca-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c2ca-106">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-106">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="9c2ca-107">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-107">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="9c2ca-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c2ca-109">权限</span><span class="sxs-lookup"><span data-stu-id="9c2ca-109">Permissions</span></span>

<span data-ttu-id="9c2ca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c2ca-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c2ca-112">Permission type</span></span>                        | <span data-ttu-id="9c2ca-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c2ca-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9c2ca-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c2ca-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c2ca-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c2ca-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9c2ca-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c2ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c2ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-117">Not supported.</span></span>                           |
| <span data-ttu-id="9c2ca-118">应用</span><span class="sxs-lookup"><span data-stu-id="9c2ca-118">Application</span></span>                            | <span data-ttu-id="9c2ca-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c2ca-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="9c2ca-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9c2ca-121">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9c2ca-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c2ca-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9c2ca-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="9c2ca-123">Function parameters</span></span>

<span data-ttu-id="9c2ca-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9c2ca-125">参数</span><span class="sxs-lookup"><span data-stu-id="9c2ca-125">Parameter</span></span> | <span data-ttu-id="9c2ca-126">类型</span><span class="sxs-lookup"><span data-stu-id="9c2ca-126">Type</span></span>   | <span data-ttu-id="9c2ca-127">说明</span><span class="sxs-lookup"><span data-stu-id="9c2ca-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9c2ca-128">period</span><span class="sxs-lookup"><span data-stu-id="9c2ca-128">period</span></span>    | <span data-ttu-id="9c2ca-129">string</span><span class="sxs-lookup"><span data-stu-id="9c2ca-129">string</span></span> | <span data-ttu-id="9c2ca-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9c2ca-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9c2ca-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9c2ca-133">必需。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9c2ca-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c2ca-134">Request headers</span></span>

| <span data-ttu-id="9c2ca-135">名称</span><span class="sxs-lookup"><span data-stu-id="9c2ca-135">Name</span></span>          | <span data-ttu-id="9c2ca-136">说明</span><span class="sxs-lookup"><span data-stu-id="9c2ca-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9c2ca-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c2ca-137">Authorization</span></span> | <span data-ttu-id="9c2ca-p106">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9c2ca-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9c2ca-140">If-None-Match</span></span> | <span data-ttu-id="9c2ca-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9c2ca-142">可选。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9c2ca-143">响应</span><span class="sxs-lookup"><span data-stu-id="9c2ca-143">Response</span></span>

<span data-ttu-id="9c2ca-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9c2ca-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9c2ca-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9c2ca-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9c2ca-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9c2ca-148">Report Refresh Date</span></span>
- <span data-ttu-id="9c2ca-149">网站类型</span><span class="sxs-lookup"><span data-stu-id="9c2ca-149">Site Type</span></span>
- <span data-ttu-id="9c2ca-150">总计</span><span class="sxs-lookup"><span data-stu-id="9c2ca-150">Total</span></span>
- <span data-ttu-id="9c2ca-151">活跃</span><span class="sxs-lookup"><span data-stu-id="9c2ca-151">Active</span></span>
- <span data-ttu-id="9c2ca-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="9c2ca-152">Report Date</span></span>
- <span data-ttu-id="9c2ca-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="9c2ca-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9c2ca-154">示例</span><span class="sxs-lookup"><span data-stu-id="9c2ca-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9c2ca-155">请求</span><span class="sxs-lookup"><span data-stu-id="9c2ca-155">Request</span></span>

<span data-ttu-id="9c2ca-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c2ca-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c2ca-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="9c2ca-158">C#</span><span class="sxs-lookup"><span data-stu-id="9c2ca-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c2ca-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c2ca-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c2ca-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c2ca-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c2ca-161">Java</span><span class="sxs-lookup"><span data-stu-id="9c2ca-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagesitecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c2ca-162">响应</span><span class="sxs-lookup"><span data-stu-id="9c2ca-162">Response</span></span>

<span data-ttu-id="9c2ca-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="9c2ca-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9c2ca-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
