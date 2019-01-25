---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: 按设备类型获取用户数。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 5d8f74926d6cbfee6a22f9a6789fb232f1166b55
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511371"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="1999c-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1999c-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1999c-104">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="1999c-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="1999c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="1999c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="1999c-106">权限</span><span class="sxs-lookup"><span data-stu-id="1999c-106">Permissions</span></span>

<span data-ttu-id="1999c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1999c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1999c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1999c-109">Permission type</span></span>                        | <span data-ttu-id="1999c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1999c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1999c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1999c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1999c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1999c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1999c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1999c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1999c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1999c-114">Not supported.</span></span>                           |
| <span data-ttu-id="1999c-115">应用</span><span class="sxs-lookup"><span data-stu-id="1999c-115">Application</span></span>                            | <span data-ttu-id="1999c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1999c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1999c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1999c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1999c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="1999c-118">Function parameters</span></span>

<span data-ttu-id="1999c-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1999c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1999c-120">参数</span><span class="sxs-lookup"><span data-stu-id="1999c-120">Parameter</span></span> | <span data-ttu-id="1999c-121">类型</span><span class="sxs-lookup"><span data-stu-id="1999c-121">Type</span></span>   | <span data-ttu-id="1999c-122">说明</span><span class="sxs-lookup"><span data-stu-id="1999c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1999c-123">period</span><span class="sxs-lookup"><span data-stu-id="1999c-123">period</span></span>    | <span data-ttu-id="1999c-124">string</span><span class="sxs-lookup"><span data-stu-id="1999c-124">string</span></span> | <span data-ttu-id="1999c-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1999c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1999c-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1999c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1999c-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1999c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1999c-128">必需。</span><span class="sxs-lookup"><span data-stu-id="1999c-128">Required.</span></span> |

<span data-ttu-id="1999c-129">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1999c-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1999c-130">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="1999c-130">The default output type is text/csv.</span></span> <span data-ttu-id="1999c-131">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="1999c-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1999c-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="1999c-132">Request headers</span></span>

| <span data-ttu-id="1999c-133">名称</span><span class="sxs-lookup"><span data-stu-id="1999c-133">Name</span></span>          | <span data-ttu-id="1999c-134">说明</span><span class="sxs-lookup"><span data-stu-id="1999c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1999c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="1999c-135">Authorization</span></span> | <span data-ttu-id="1999c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1999c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1999c-138">响应</span><span class="sxs-lookup"><span data-stu-id="1999c-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1999c-139">CSV</span><span class="sxs-lookup"><span data-stu-id="1999c-139">CSV</span></span>

<span data-ttu-id="1999c-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1999c-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1999c-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1999c-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1999c-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1999c-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1999c-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1999c-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1999c-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1999c-144">Report Refresh Date</span></span>
- <span data-ttu-id="1999c-145">Web</span><span class="sxs-lookup"><span data-stu-id="1999c-145">Web</span></span>
- <span data-ttu-id="1999c-146">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="1999c-146">Windows Phone</span></span>
- <span data-ttu-id="1999c-147">Android 手机</span><span class="sxs-lookup"><span data-stu-id="1999c-147">Android Phone</span></span>
- <span data-ttu-id="1999c-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="1999c-148">iPhone</span></span>
- <span data-ttu-id="1999c-149">iPad</span><span class="sxs-lookup"><span data-stu-id="1999c-149">iPad</span></span>
- <span data-ttu-id="1999c-150">其他</span><span class="sxs-lookup"><span data-stu-id="1999c-150">Other</span></span>
- <span data-ttu-id="1999c-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="1999c-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1999c-152">JSON</span><span class="sxs-lookup"><span data-stu-id="1999c-152">JSON</span></span>

<span data-ttu-id="1999c-153">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1999c-153">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1999c-154">示例</span><span class="sxs-lookup"><span data-stu-id="1999c-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1999c-155">CSV</span><span class="sxs-lookup"><span data-stu-id="1999c-155">CSV</span></span>

<span data-ttu-id="1999c-156">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="1999c-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1999c-157">请求</span><span class="sxs-lookup"><span data-stu-id="1999c-157">Request</span></span>

<span data-ttu-id="1999c-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1999c-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1999c-159">响应</span><span class="sxs-lookup"><span data-stu-id="1999c-159">Response</span></span>

<span data-ttu-id="1999c-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1999c-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1999c-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1999c-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```

### <a name="json"></a><span data-ttu-id="1999c-162">JSON</span><span class="sxs-lookup"><span data-stu-id="1999c-162">JSON</span></span>

<span data-ttu-id="1999c-163">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1999c-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1999c-164">请求</span><span class="sxs-lookup"><span data-stu-id="1999c-164">Request</span></span>

<span data-ttu-id="1999c-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1999c-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1999c-166">响应</span><span class="sxs-lookup"><span data-stu-id="1999c-166">Response</span></span>

<span data-ttu-id="1999c-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1999c-167">The following is an example of the response.</span></span>

> <span data-ttu-id="1999c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1999c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 138, 
      "windowsPhone": 1, 
      "androidPhone": 29, 
      "iPhone": 40, 
      "iPad": 2, 
      "other": 2, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
