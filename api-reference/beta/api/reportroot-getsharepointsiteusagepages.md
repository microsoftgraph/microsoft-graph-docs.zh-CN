---
title: 'reportRoot: getSharePointSiteUsagePages'
description: 获取跨所有网站浏览的页面数。
ms.openlocfilehash: 7e6d620179e5b6d41b5076ae6e79917fd27ef4bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048795"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="6ac7b-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="6ac7b-103">reportRoot: getSharePointSiteUsagePages</span></span>

> <span data-ttu-id="6ac7b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ac7b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ac7b-106">获取跨所有网站浏览的页面数。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-106">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="6ac7b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ac7b-108">权限</span><span class="sxs-lookup"><span data-stu-id="6ac7b-108">Permissions</span></span>

<span data-ttu-id="6ac7b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ac7b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ac7b-111">Permission type</span></span>                        | <span data-ttu-id="6ac7b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ac7b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6ac7b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac7b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ac7b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac7b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6ac7b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ac7b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-116">Not supported.</span></span>                           |
| <span data-ttu-id="6ac7b-117">应用</span><span class="sxs-lookup"><span data-stu-id="6ac7b-117">Application</span></span>                            | <span data-ttu-id="6ac7b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac7b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6ac7b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac7b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6ac7b-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="6ac7b-120">Function parameters</span></span>

<span data-ttu-id="6ac7b-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6ac7b-122">参数</span><span class="sxs-lookup"><span data-stu-id="6ac7b-122">Parameter</span></span> | <span data-ttu-id="6ac7b-123">类型</span><span class="sxs-lookup"><span data-stu-id="6ac7b-123">Type</span></span>   | <span data-ttu-id="6ac7b-124">说明</span><span class="sxs-lookup"><span data-stu-id="6ac7b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6ac7b-125">period</span><span class="sxs-lookup"><span data-stu-id="6ac7b-125">period</span></span>    | <span data-ttu-id="6ac7b-126">string</span><span class="sxs-lookup"><span data-stu-id="6ac7b-126">string</span></span> | <span data-ttu-id="6ac7b-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6ac7b-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6ac7b-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6ac7b-130">必需。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-130">Required.</span></span> |

<span data-ttu-id="6ac7b-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6ac7b-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-132">The default output type is text/csv.</span></span> <span data-ttu-id="6ac7b-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ac7b-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac7b-134">Request headers</span></span>

| <span data-ttu-id="6ac7b-135">名称</span><span class="sxs-lookup"><span data-stu-id="6ac7b-135">Name</span></span>          | <span data-ttu-id="6ac7b-136">说明</span><span class="sxs-lookup"><span data-stu-id="6ac7b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6ac7b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac7b-137">Authorization</span></span> | <span data-ttu-id="6ac7b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6ac7b-140">响应</span><span class="sxs-lookup"><span data-stu-id="6ac7b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6ac7b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="6ac7b-141">CSV</span></span>

<span data-ttu-id="6ac7b-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6ac7b-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6ac7b-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6ac7b-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6ac7b-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6ac7b-146">Report Refresh Date</span></span>
- <span data-ttu-id="6ac7b-147">网站类型</span><span class="sxs-lookup"><span data-stu-id="6ac7b-147">Site Type</span></span>
- <span data-ttu-id="6ac7b-148">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="6ac7b-148">Page View Count</span></span>
- <span data-ttu-id="6ac7b-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="6ac7b-149">Report Date</span></span>
- <span data-ttu-id="6ac7b-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="6ac7b-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6ac7b-151">JSON</span><span class="sxs-lookup"><span data-stu-id="6ac7b-151">JSON</span></span>

<span data-ttu-id="6ac7b-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-152">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ac7b-153">示例</span><span class="sxs-lookup"><span data-stu-id="6ac7b-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6ac7b-154">CSV</span><span class="sxs-lookup"><span data-stu-id="6ac7b-154">CSV</span></span>

<span data-ttu-id="6ac7b-155">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6ac7b-156">请求</span><span class="sxs-lookup"><span data-stu-id="6ac7b-156">Request</span></span>

<span data-ttu-id="6ac7b-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6ac7b-158">响应</span><span class="sxs-lookup"><span data-stu-id="6ac7b-158">Response</span></span>

<span data-ttu-id="6ac7b-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6ac7b-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6ac7b-161">JSON</span><span class="sxs-lookup"><span data-stu-id="6ac7b-161">JSON</span></span>

<span data-ttu-id="6ac7b-162">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6ac7b-163">请求</span><span class="sxs-lookup"><span data-stu-id="6ac7b-163">Request</span></span>

<span data-ttu-id="6ac7b-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6ac7b-165">响应</span><span class="sxs-lookup"><span data-stu-id="6ac7b-165">Response</span></span>

<span data-ttu-id="6ac7b-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-166">The following is an example of the response.</span></span>

> <span data-ttu-id="6ac7b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6ac7b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsagePages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "pageViewCount": 183, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
