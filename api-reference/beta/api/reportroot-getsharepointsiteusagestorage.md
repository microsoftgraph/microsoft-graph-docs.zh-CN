---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: 获取报表周期内分配和使用的存储趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d586d2736b5da0949f0b9207c7918e9fb8ad60ef
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896218"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="fc80c-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="fc80c-103">reportRoot: getSharePointSiteUsageStorage</span></span>

<span data-ttu-id="fc80c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc80c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc80c-105">获取报表周期内分配和使用的存储趋势。</span><span class="sxs-lookup"><span data-stu-id="fc80c-105">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="fc80c-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="fc80c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc80c-107">权限</span><span class="sxs-lookup"><span data-stu-id="fc80c-107">Permissions</span></span>

<span data-ttu-id="fc80c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc80c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc80c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc80c-110">Permission type</span></span>                        | <span data-ttu-id="fc80c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc80c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fc80c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc80c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc80c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc80c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fc80c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc80c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc80c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc80c-115">Not supported.</span></span>                           |
| <span data-ttu-id="fc80c-116">应用</span><span class="sxs-lookup"><span data-stu-id="fc80c-116">Application</span></span>                            | <span data-ttu-id="fc80c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc80c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="fc80c-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="fc80c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="fc80c-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="fc80c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="fc80c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc80c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fc80c-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="fc80c-121">Function parameters</span></span>

<span data-ttu-id="fc80c-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fc80c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fc80c-123">参数</span><span class="sxs-lookup"><span data-stu-id="fc80c-123">Parameter</span></span> | <span data-ttu-id="fc80c-124">类型</span><span class="sxs-lookup"><span data-stu-id="fc80c-124">Type</span></span>   | <span data-ttu-id="fc80c-125">说明</span><span class="sxs-lookup"><span data-stu-id="fc80c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fc80c-126">period</span><span class="sxs-lookup"><span data-stu-id="fc80c-126">period</span></span>    | <span data-ttu-id="fc80c-127">string</span><span class="sxs-lookup"><span data-stu-id="fc80c-127">string</span></span> | <span data-ttu-id="fc80c-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fc80c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fc80c-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fc80c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fc80c-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fc80c-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fc80c-131">必需。</span><span class="sxs-lookup"><span data-stu-id="fc80c-131">Required.</span></span> |

<span data-ttu-id="fc80c-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fc80c-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fc80c-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="fc80c-133">The default output type is text/csv.</span></span> <span data-ttu-id="fc80c-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="fc80c-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc80c-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc80c-135">Request headers</span></span>

| <span data-ttu-id="fc80c-136">名称</span><span class="sxs-lookup"><span data-stu-id="fc80c-136">Name</span></span>          | <span data-ttu-id="fc80c-137">说明</span><span class="sxs-lookup"><span data-stu-id="fc80c-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fc80c-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc80c-138">Authorization</span></span> | <span data-ttu-id="fc80c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc80c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fc80c-141">响应</span><span class="sxs-lookup"><span data-stu-id="fc80c-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fc80c-142">CSV</span><span class="sxs-lookup"><span data-stu-id="fc80c-142">CSV</span></span>

<span data-ttu-id="fc80c-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fc80c-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fc80c-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fc80c-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fc80c-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fc80c-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fc80c-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fc80c-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fc80c-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fc80c-147">Report Refresh Date</span></span>
- <span data-ttu-id="fc80c-148">网站类型</span><span class="sxs-lookup"><span data-stu-id="fc80c-148">Site Type</span></span>
- <span data-ttu-id="fc80c-149">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="fc80c-149">Storage Used (Byte)</span></span>
- <span data-ttu-id="fc80c-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="fc80c-150">Report Date</span></span>
- <span data-ttu-id="fc80c-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="fc80c-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fc80c-152">JSON</span><span class="sxs-lookup"><span data-stu-id="fc80c-152">JSON</span></span>

<span data-ttu-id="fc80c-153">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[siteUsageStorage](../resources/siteusagestorage.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fc80c-153">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc80c-154">示例</span><span class="sxs-lookup"><span data-stu-id="fc80c-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fc80c-155">CSV</span><span class="sxs-lookup"><span data-stu-id="fc80c-155">CSV</span></span>

<span data-ttu-id="fc80c-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc80c-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fc80c-157">请求</span><span class="sxs-lookup"><span data-stu-id="fc80c-157">Request</span></span>

<span data-ttu-id="fc80c-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc80c-158">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="fc80c-159">响应</span><span class="sxs-lookup"><span data-stu-id="fc80c-159">Response</span></span>

<span data-ttu-id="fc80c-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc80c-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fc80c-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fc80c-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fc80c-162">JSON</span><span class="sxs-lookup"><span data-stu-id="fc80c-162">JSON</span></span>

<span data-ttu-id="fc80c-163">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc80c-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fc80c-164">请求</span><span class="sxs-lookup"><span data-stu-id="fc80c-164">Request</span></span>

<span data-ttu-id="fc80c-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc80c-165">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="fc80c-166">响应</span><span class="sxs-lookup"><span data-stu-id="fc80c-166">Response</span></span>

<span data-ttu-id="fc80c-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc80c-167">The following is an example of the response.</span></span>

> <span data-ttu-id="fc80c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc80c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
