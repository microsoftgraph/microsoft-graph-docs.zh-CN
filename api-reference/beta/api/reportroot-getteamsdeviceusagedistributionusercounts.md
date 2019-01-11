---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.openlocfilehash: 274fd212d936df75122c5c7acafeae12a2e528b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830336"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="cac07-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="cac07-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="cac07-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cac07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cac07-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cac07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cac07-106">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="cac07-106">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="cac07-107">权限</span><span class="sxs-lookup"><span data-stu-id="cac07-107">Permissions</span></span>

<span data-ttu-id="cac07-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cac07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cac07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cac07-110">Permission type</span></span>                        | <span data-ttu-id="cac07-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cac07-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cac07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cac07-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cac07-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cac07-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cac07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cac07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cac07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cac07-115">Not supported.</span></span>                           |
| <span data-ttu-id="cac07-116">应用</span><span class="sxs-lookup"><span data-stu-id="cac07-116">Application</span></span>                            | <span data-ttu-id="cac07-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cac07-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cac07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cac07-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="cac07-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="cac07-119">Function parameters</span></span>

<span data-ttu-id="cac07-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="cac07-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cac07-121">参数</span><span class="sxs-lookup"><span data-stu-id="cac07-121">Parameter</span></span> | <span data-ttu-id="cac07-122">类型</span><span class="sxs-lookup"><span data-stu-id="cac07-122">Type</span></span>   | <span data-ttu-id="cac07-123">说明</span><span class="sxs-lookup"><span data-stu-id="cac07-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cac07-124">period</span><span class="sxs-lookup"><span data-stu-id="cac07-124">period</span></span>    | <span data-ttu-id="cac07-125">string</span><span class="sxs-lookup"><span data-stu-id="cac07-125">string</span></span> | <span data-ttu-id="cac07-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cac07-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cac07-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cac07-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cac07-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cac07-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cac07-129">必需。</span><span class="sxs-lookup"><span data-stu-id="cac07-129">Required.</span></span> |

<span data-ttu-id="cac07-130">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cac07-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cac07-131">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="cac07-131">The default output type is text/csv.</span></span> <span data-ttu-id="cac07-132">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="cac07-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cac07-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="cac07-133">Request headers</span></span>

| <span data-ttu-id="cac07-134">名称</span><span class="sxs-lookup"><span data-stu-id="cac07-134">Name</span></span>          | <span data-ttu-id="cac07-135">说明</span><span class="sxs-lookup"><span data-stu-id="cac07-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cac07-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac07-136">Authorization</span></span> | <span data-ttu-id="cac07-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cac07-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cac07-139">响应</span><span class="sxs-lookup"><span data-stu-id="cac07-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cac07-140">CSV</span><span class="sxs-lookup"><span data-stu-id="cac07-140">CSV</span></span>

<span data-ttu-id="cac07-141">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cac07-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cac07-142">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cac07-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cac07-143">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cac07-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cac07-144">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cac07-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cac07-145">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cac07-145">Report Refresh Date</span></span>
- <span data-ttu-id="cac07-146">Web</span><span class="sxs-lookup"><span data-stu-id="cac07-146">Web</span></span>
- <span data-ttu-id="cac07-147">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="cac07-147">Windows Phone</span></span>
- <span data-ttu-id="cac07-148">Android 手机</span><span class="sxs-lookup"><span data-stu-id="cac07-148">Android Phone</span></span>
- <span data-ttu-id="cac07-149">iOS</span><span class="sxs-lookup"><span data-stu-id="cac07-149">iOS</span></span>
- <span data-ttu-id="cac07-150">Mac</span><span class="sxs-lookup"><span data-stu-id="cac07-150">Mac</span></span>
- <span data-ttu-id="cac07-151">Windows</span><span class="sxs-lookup"><span data-stu-id="cac07-151">Windows</span></span>
- <span data-ttu-id="cac07-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="cac07-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cac07-153">JSON</span><span class="sxs-lookup"><span data-stu-id="cac07-153">JSON</span></span>

<span data-ttu-id="cac07-154">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="cac07-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac07-155">示例</span><span class="sxs-lookup"><span data-stu-id="cac07-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cac07-156">CSV</span><span class="sxs-lookup"><span data-stu-id="cac07-156">CSV</span></span>

<span data-ttu-id="cac07-157">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="cac07-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cac07-158">请求</span><span class="sxs-lookup"><span data-stu-id="cac07-158">Request</span></span>

<span data-ttu-id="cac07-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cac07-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cac07-160">响应</span><span class="sxs-lookup"><span data-stu-id="cac07-160">Response</span></span>

<span data-ttu-id="cac07-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cac07-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cac07-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cac07-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="cac07-163">JSON</span><span class="sxs-lookup"><span data-stu-id="cac07-163">JSON</span></span>

<span data-ttu-id="cac07-164">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="cac07-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cac07-165">请求</span><span class="sxs-lookup"><span data-stu-id="cac07-165">Request</span></span>

<span data-ttu-id="cac07-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cac07-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cac07-167">响应</span><span class="sxs-lookup"><span data-stu-id="cac07-167">Response</span></span>

<span data-ttu-id="cac07-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cac07-168">The following is an example of the response.</span></span>

> <span data-ttu-id="cac07-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cac07-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
