---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: 获取报表周期内分配和使用的存储趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e288f61f47e1f4497ca0bef7281074eb2b430fa4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537921"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="f8ab8-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="f8ab8-103">reportRoot: getSharePointSiteUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8ab8-104">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="f8ab8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8ab8-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8ab8-106">Permissions</span></span>

<span data-ttu-id="f8ab8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8ab8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8ab8-109">Permission type</span></span>                        | <span data-ttu-id="f8ab8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8ab8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8ab8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ab8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8ab8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8ab8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f8ab8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ab8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8ab8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-114">Not supported.</span></span>                           |
| <span data-ttu-id="f8ab8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8ab8-115">Application</span></span>                            | <span data-ttu-id="f8ab8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8ab8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f8ab8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8ab8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f8ab8-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="f8ab8-118">Function parameters</span></span>

<span data-ttu-id="f8ab8-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f8ab8-120">参数</span><span class="sxs-lookup"><span data-stu-id="f8ab8-120">Parameter</span></span> | <span data-ttu-id="f8ab8-121">类型</span><span class="sxs-lookup"><span data-stu-id="f8ab8-121">Type</span></span>   | <span data-ttu-id="f8ab8-122">说明</span><span class="sxs-lookup"><span data-stu-id="f8ab8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8ab8-123">period</span><span class="sxs-lookup"><span data-stu-id="f8ab8-123">period</span></span>    | <span data-ttu-id="f8ab8-124">string</span><span class="sxs-lookup"><span data-stu-id="f8ab8-124">string</span></span> | <span data-ttu-id="f8ab8-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8ab8-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8ab8-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8ab8-128">必需。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-128">Required.</span></span> |

<span data-ttu-id="f8ab8-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f8ab8-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-130">The default output type is text/csv.</span></span> <span data-ttu-id="f8ab8-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8ab8-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8ab8-132">Request headers</span></span>

| <span data-ttu-id="f8ab8-133">名称</span><span class="sxs-lookup"><span data-stu-id="f8ab8-133">Name</span></span>          | <span data-ttu-id="f8ab8-134">说明</span><span class="sxs-lookup"><span data-stu-id="f8ab8-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f8ab8-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8ab8-135">Authorization</span></span> | <span data-ttu-id="f8ab8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f8ab8-138">响应</span><span class="sxs-lookup"><span data-stu-id="f8ab8-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f8ab8-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f8ab8-139">CSV</span></span>

<span data-ttu-id="f8ab8-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8ab8-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8ab8-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f8ab8-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8ab8-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f8ab8-144">Report Refresh Date</span></span>
- <span data-ttu-id="f8ab8-145">网站类型</span><span class="sxs-lookup"><span data-stu-id="f8ab8-145">Site Type</span></span>
- <span data-ttu-id="f8ab8-146">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="f8ab8-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="f8ab8-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="f8ab8-147">Report Date</span></span>
- <span data-ttu-id="f8ab8-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="f8ab8-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f8ab8-149">JSON</span><span class="sxs-lookup"><span data-stu-id="f8ab8-149">JSON</span></span>

<span data-ttu-id="f8ab8-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[siteUsageStorage](../resources/siteusagestorage.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8ab8-151">示例</span><span class="sxs-lookup"><span data-stu-id="f8ab8-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f8ab8-152">CSV</span><span class="sxs-lookup"><span data-stu-id="f8ab8-152">CSV</span></span>

<span data-ttu-id="f8ab8-153">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f8ab8-154">请求</span><span class="sxs-lookup"><span data-stu-id="f8ab8-154">Request</span></span>

<span data-ttu-id="f8ab8-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f8ab8-156">响应</span><span class="sxs-lookup"><span data-stu-id="f8ab8-156">Response</span></span>

<span data-ttu-id="f8ab8-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f8ab8-158">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f8ab8-159">JSON</span><span class="sxs-lookup"><span data-stu-id="f8ab8-159">JSON</span></span>

<span data-ttu-id="f8ab8-160">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f8ab8-161">请求</span><span class="sxs-lookup"><span data-stu-id="f8ab8-161">Request</span></span>

<span data-ttu-id="f8ab8-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f8ab8-163">响应</span><span class="sxs-lookup"><span data-stu-id="f8ab8-163">Response</span></span>

<span data-ttu-id="f8ab8-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-164">The following is an example of the response.</span></span>

> <span data-ttu-id="f8ab8-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8ab8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 171835798971, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagestorage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
