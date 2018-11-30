---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: 获取 SharePoint 网站使用情况的详细信息。
ms.openlocfilehash: 58c51bfcc14f3478a53c45f66f64ce7dc547ea6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046222"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="8eef3-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="8eef3-103">reportRoot: getSharePointSiteUsageDetail</span></span>

> <span data-ttu-id="8eef3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8eef3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eef3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8eef3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eef3-106">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8eef3-106">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="8eef3-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="8eef3-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eef3-108">权限</span><span class="sxs-lookup"><span data-stu-id="8eef3-108">Permissions</span></span>

<span data-ttu-id="8eef3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eef3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8eef3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eef3-111">Permission type</span></span>                        | <span data-ttu-id="8eef3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8eef3-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8eef3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eef3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8eef3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eef3-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8eef3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eef3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eef3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eef3-116">Not supported.</span></span>                           |
| <span data-ttu-id="8eef3-117">应用</span><span class="sxs-lookup"><span data-stu-id="8eef3-117">Application</span></span>                            | <span data-ttu-id="8eef3-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eef3-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8eef3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eef3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8eef3-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="8eef3-120">Function parameters</span></span>

<span data-ttu-id="8eef3-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="8eef3-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8eef3-122">参数</span><span class="sxs-lookup"><span data-stu-id="8eef3-122">Parameter</span></span> | <span data-ttu-id="8eef3-123">类型</span><span class="sxs-lookup"><span data-stu-id="8eef3-123">Type</span></span>   | <span data-ttu-id="8eef3-124">说明</span><span class="sxs-lookup"><span data-stu-id="8eef3-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8eef3-125">period</span><span class="sxs-lookup"><span data-stu-id="8eef3-125">period</span></span>    | <span data-ttu-id="8eef3-126">string</span><span class="sxs-lookup"><span data-stu-id="8eef3-126">string</span></span> | <span data-ttu-id="8eef3-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8eef3-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8eef3-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8eef3-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8eef3-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8eef3-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8eef3-130">date</span><span class="sxs-lookup"><span data-stu-id="8eef3-130">date</span></span>      | <span data-ttu-id="8eef3-131">Date</span><span class="sxs-lookup"><span data-stu-id="8eef3-131">Date</span></span>   | <span data-ttu-id="8eef3-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="8eef3-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8eef3-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="8eef3-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8eef3-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="8eef3-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8eef3-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="8eef3-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="8eef3-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8eef3-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8eef3-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="8eef3-137">The default output type is text/csv.</span></span> <span data-ttu-id="8eef3-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="8eef3-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eef3-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eef3-139">Request headers</span></span>

| <span data-ttu-id="8eef3-140">名称</span><span class="sxs-lookup"><span data-stu-id="8eef3-140">Name</span></span>          | <span data-ttu-id="8eef3-141">说明</span><span class="sxs-lookup"><span data-stu-id="8eef3-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8eef3-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eef3-142">Authorization</span></span> | <span data-ttu-id="8eef3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8eef3-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8eef3-145">响应</span><span class="sxs-lookup"><span data-stu-id="8eef3-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8eef3-146">CSV</span><span class="sxs-lookup"><span data-stu-id="8eef3-146">CSV</span></span>

<span data-ttu-id="8eef3-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8eef3-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8eef3-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8eef3-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8eef3-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8eef3-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8eef3-150">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="8eef3-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="8eef3-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8eef3-151">Report Refresh Date</span></span>
- <span data-ttu-id="8eef3-152">网站 Id</span><span class="sxs-lookup"><span data-stu-id="8eef3-152">Site Id</span></span>
- <span data-ttu-id="8eef3-153">网站 URL</span><span class="sxs-lookup"><span data-stu-id="8eef3-153">Site URL</span></span>
- <span data-ttu-id="8eef3-154">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="8eef3-154">Owner Display Name</span></span>
- <span data-ttu-id="8eef3-155">已删除</span><span class="sxs-lookup"><span data-stu-id="8eef3-155">Is Deleted</span></span>
- <span data-ttu-id="8eef3-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="8eef3-156">Last Activity Date</span></span>
- <span data-ttu-id="8eef3-157">文件数</span><span class="sxs-lookup"><span data-stu-id="8eef3-157">File Count</span></span>
- <span data-ttu-id="8eef3-158">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="8eef3-158">Active File Count</span></span>
- <span data-ttu-id="8eef3-159">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="8eef3-159">Page View Count</span></span>
- <span data-ttu-id="8eef3-160">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="8eef3-160">Visited Page Count</span></span>
- <span data-ttu-id="8eef3-161">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="8eef3-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="8eef3-162">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="8eef3-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="8eef3-163">根网站模板</span><span class="sxs-lookup"><span data-stu-id="8eef3-163">Root Web Template</span></span>
- <span data-ttu-id="8eef3-164">报表周期</span><span class="sxs-lookup"><span data-stu-id="8eef3-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8eef3-165">JSON</span><span class="sxs-lookup"><span data-stu-id="8eef3-165">JSON</span></span>

<span data-ttu-id="8eef3-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="8eef3-166">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="8eef3-167">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="8eef3-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="8eef3-168">示例</span><span class="sxs-lookup"><span data-stu-id="8eef3-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8eef3-169">CSV</span><span class="sxs-lookup"><span data-stu-id="8eef3-169">CSV</span></span>

<span data-ttu-id="8eef3-170">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="8eef3-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8eef3-171">请求</span><span class="sxs-lookup"><span data-stu-id="8eef3-171">Request</span></span>

<span data-ttu-id="8eef3-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8eef3-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8eef3-173">响应</span><span class="sxs-lookup"><span data-stu-id="8eef3-173">Response</span></span>

<span data-ttu-id="8eef3-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8eef3-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8eef3-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8eef3-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```

### <a name="json"></a><span data-ttu-id="8eef3-176">JSON</span><span class="sxs-lookup"><span data-stu-id="8eef3-176">JSON</span></span>

<span data-ttu-id="8eef3-177">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="8eef3-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8eef3-178">请求</span><span class="sxs-lookup"><span data-stu-id="8eef3-178">Request</span></span>

<span data-ttu-id="8eef3-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8eef3-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8eef3-180">响应</span><span class="sxs-lookup"><span data-stu-id="8eef3-180">Response</span></span>

<span data-ttu-id="8eef3-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8eef3-181">The following is an example of the response.</span></span>

> <span data-ttu-id="8eef3-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8eef3-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
      "reportPeriod": "7"
    }
  ]
}
```
