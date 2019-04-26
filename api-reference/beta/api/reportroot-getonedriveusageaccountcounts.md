---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1c588316235f7d6102860da0a8de21a60c5daec0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331816"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="a1b98-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="a1b98-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1b98-105">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="a1b98-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="a1b98-106">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="a1b98-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="a1b98-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="a1b98-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1b98-108">权限</span><span class="sxs-lookup"><span data-stu-id="a1b98-108">Permissions</span></span>

<span data-ttu-id="a1b98-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1b98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1b98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1b98-111">Permission type</span></span>                        | <span data-ttu-id="a1b98-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1b98-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a1b98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1b98-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1b98-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1b98-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a1b98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1b98-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1b98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1b98-116">Not supported.</span></span>                           |
| <span data-ttu-id="a1b98-117">应用</span><span class="sxs-lookup"><span data-stu-id="a1b98-117">Application</span></span>                            | <span data-ttu-id="a1b98-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1b98-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a1b98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1b98-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a1b98-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="a1b98-120">Function parameters</span></span>

<span data-ttu-id="a1b98-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a1b98-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a1b98-122">参数</span><span class="sxs-lookup"><span data-stu-id="a1b98-122">Parameter</span></span> | <span data-ttu-id="a1b98-123">类型</span><span class="sxs-lookup"><span data-stu-id="a1b98-123">Type</span></span>   | <span data-ttu-id="a1b98-124">说明</span><span class="sxs-lookup"><span data-stu-id="a1b98-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a1b98-125">period</span><span class="sxs-lookup"><span data-stu-id="a1b98-125">period</span></span>    | <span data-ttu-id="a1b98-126">string</span><span class="sxs-lookup"><span data-stu-id="a1b98-126">string</span></span> | <span data-ttu-id="a1b98-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a1b98-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a1b98-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a1b98-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a1b98-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a1b98-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a1b98-130">必需。</span><span class="sxs-lookup"><span data-stu-id="a1b98-130">Required.</span></span> |

<span data-ttu-id="a1b98-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1b98-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a1b98-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a1b98-132">The default output type is text/csv.</span></span> <span data-ttu-id="a1b98-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a1b98-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1b98-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1b98-134">Request headers</span></span>

| <span data-ttu-id="a1b98-135">名称</span><span class="sxs-lookup"><span data-stu-id="a1b98-135">Name</span></span>          | <span data-ttu-id="a1b98-136">说明</span><span class="sxs-lookup"><span data-stu-id="a1b98-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a1b98-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1b98-137">Authorization</span></span> | <span data-ttu-id="a1b98-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1b98-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a1b98-140">响应</span><span class="sxs-lookup"><span data-stu-id="a1b98-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a1b98-141">CSV</span><span class="sxs-lookup"><span data-stu-id="a1b98-141">CSV</span></span>

<span data-ttu-id="a1b98-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a1b98-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a1b98-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a1b98-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a1b98-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a1b98-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a1b98-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a1b98-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a1b98-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a1b98-146">Report Refresh Date</span></span>
- <span data-ttu-id="a1b98-147">网站类型</span><span class="sxs-lookup"><span data-stu-id="a1b98-147">Site Type</span></span>
- <span data-ttu-id="a1b98-148">总计</span><span class="sxs-lookup"><span data-stu-id="a1b98-148">Total</span></span>
- <span data-ttu-id="a1b98-149">活跃</span><span class="sxs-lookup"><span data-stu-id="a1b98-149">Active</span></span>
- <span data-ttu-id="a1b98-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="a1b98-150">Report Date</span></span>
- <span data-ttu-id="a1b98-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="a1b98-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a1b98-152">JSON</span><span class="sxs-lookup"><span data-stu-id="a1b98-152">JSON</span></span>

<span data-ttu-id="a1b98-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a1b98-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b98-154">示例</span><span class="sxs-lookup"><span data-stu-id="a1b98-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a1b98-155">CSV</span><span class="sxs-lookup"><span data-stu-id="a1b98-155">CSV</span></span>

<span data-ttu-id="a1b98-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a1b98-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a1b98-157">请求</span><span class="sxs-lookup"><span data-stu-id="a1b98-157">Request</span></span>

<span data-ttu-id="a1b98-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1b98-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a1b98-159">响应</span><span class="sxs-lookup"><span data-stu-id="a1b98-159">Response</span></span>

<span data-ttu-id="a1b98-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1b98-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a1b98-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a1b98-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a1b98-162">JSON</span><span class="sxs-lookup"><span data-stu-id="a1b98-162">JSON</span></span>

<span data-ttu-id="a1b98-163">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a1b98-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a1b98-164">请求</span><span class="sxs-lookup"><span data-stu-id="a1b98-164">Request</span></span>

<span data-ttu-id="a1b98-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1b98-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a1b98-166">响应</span><span class="sxs-lookup"><span data-stu-id="a1b98-166">Response</span></span>

<span data-ttu-id="a1b98-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1b98-167">The following is an example of the response.</span></span>

> <span data-ttu-id="a1b98-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a1b98-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
