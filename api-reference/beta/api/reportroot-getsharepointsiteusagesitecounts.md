---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.openlocfilehash: da690c7761e56b598a1c9cb9e223b3e7f888b904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822356"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="727db-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="727db-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

> <span data-ttu-id="727db-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="727db-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="727db-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="727db-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="727db-107">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="727db-107">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="727db-108">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="727db-108">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="727db-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="727db-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="727db-110">权限</span><span class="sxs-lookup"><span data-stu-id="727db-110">Permissions</span></span>

<span data-ttu-id="727db-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="727db-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="727db-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="727db-113">Permission type</span></span>                        | <span data-ttu-id="727db-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="727db-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="727db-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="727db-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="727db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="727db-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="727db-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="727db-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="727db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="727db-118">Not supported.</span></span>                           |
| <span data-ttu-id="727db-119">应用</span><span class="sxs-lookup"><span data-stu-id="727db-119">Application</span></span>                            | <span data-ttu-id="727db-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="727db-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="727db-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="727db-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="727db-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="727db-122">Function parameters</span></span>

<span data-ttu-id="727db-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="727db-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="727db-124">参数</span><span class="sxs-lookup"><span data-stu-id="727db-124">Parameter</span></span> | <span data-ttu-id="727db-125">类型</span><span class="sxs-lookup"><span data-stu-id="727db-125">Type</span></span>   | <span data-ttu-id="727db-126">说明</span><span class="sxs-lookup"><span data-stu-id="727db-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="727db-127">period</span><span class="sxs-lookup"><span data-stu-id="727db-127">period</span></span>    | <span data-ttu-id="727db-128">string</span><span class="sxs-lookup"><span data-stu-id="727db-128">string</span></span> | <span data-ttu-id="727db-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="727db-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="727db-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="727db-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="727db-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="727db-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="727db-132">必需。</span><span class="sxs-lookup"><span data-stu-id="727db-132">Required.</span></span> |

<span data-ttu-id="727db-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="727db-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="727db-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="727db-134">The default output type is text/csv.</span></span> <span data-ttu-id="727db-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="727db-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="727db-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="727db-136">Request headers</span></span>

| <span data-ttu-id="727db-137">名称</span><span class="sxs-lookup"><span data-stu-id="727db-137">Name</span></span>          | <span data-ttu-id="727db-138">说明</span><span class="sxs-lookup"><span data-stu-id="727db-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="727db-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="727db-139">Authorization</span></span> | <span data-ttu-id="727db-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="727db-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="727db-142">响应</span><span class="sxs-lookup"><span data-stu-id="727db-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="727db-143">CSV</span><span class="sxs-lookup"><span data-stu-id="727db-143">CSV</span></span>

<span data-ttu-id="727db-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="727db-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="727db-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="727db-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="727db-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="727db-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="727db-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="727db-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="727db-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="727db-148">Report Refresh Date</span></span>
- <span data-ttu-id="727db-149">网站类型</span><span class="sxs-lookup"><span data-stu-id="727db-149">Site Type</span></span>
- <span data-ttu-id="727db-150">总计</span><span class="sxs-lookup"><span data-stu-id="727db-150">Total</span></span>
- <span data-ttu-id="727db-151">活跃</span><span class="sxs-lookup"><span data-stu-id="727db-151">Active</span></span>
- <span data-ttu-id="727db-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="727db-152">Report Date</span></span>
- <span data-ttu-id="727db-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="727db-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="727db-154">JSON</span><span class="sxs-lookup"><span data-stu-id="727db-154">JSON</span></span>

<span data-ttu-id="727db-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="727db-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="727db-156">示例</span><span class="sxs-lookup"><span data-stu-id="727db-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="727db-157">CSV</span><span class="sxs-lookup"><span data-stu-id="727db-157">CSV</span></span>

<span data-ttu-id="727db-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="727db-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="727db-159">请求</span><span class="sxs-lookup"><span data-stu-id="727db-159">Request</span></span>

<span data-ttu-id="727db-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="727db-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="727db-161">响应</span><span class="sxs-lookup"><span data-stu-id="727db-161">Response</span></span>

<span data-ttu-id="727db-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="727db-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="727db-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="727db-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="727db-164">JSON</span><span class="sxs-lookup"><span data-stu-id="727db-164">JSON</span></span>

<span data-ttu-id="727db-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="727db-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="727db-166">请求</span><span class="sxs-lookup"><span data-stu-id="727db-166">Request</span></span>

<span data-ttu-id="727db-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="727db-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="727db-168">响应</span><span class="sxs-lookup"><span data-stu-id="727db-168">Response</span></span>

<span data-ttu-id="727db-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="727db-169">The following is an example of the response.</span></span>

> <span data-ttu-id="727db-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="727db-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageSiteCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 47, 
      "active": 15, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
