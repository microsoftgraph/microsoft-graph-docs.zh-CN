---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: 按设备类型获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 64e79ab2a1c88b63f6902cac266765fe7256c3c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052974"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="26d88-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="26d88-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="26d88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d88-105">按设备类型获取用户数。</span><span class="sxs-lookup"><span data-stu-id="26d88-105">Get the number of users by device type.</span></span>

> <span data-ttu-id="26d88-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="26d88-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="26d88-107">权限</span><span class="sxs-lookup"><span data-stu-id="26d88-107">Permissions</span></span>

<span data-ttu-id="26d88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26d88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26d88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26d88-110">Permission type</span></span>                        | <span data-ttu-id="26d88-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26d88-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="26d88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26d88-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="26d88-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26d88-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="26d88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26d88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26d88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26d88-115">Not supported.</span></span>                           |
| <span data-ttu-id="26d88-116">应用</span><span class="sxs-lookup"><span data-stu-id="26d88-116">Application</span></span>                            | <span data-ttu-id="26d88-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26d88-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="26d88-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="26d88-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="26d88-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="26d88-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="26d88-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26d88-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="26d88-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="26d88-121">Function parameters</span></span>

<span data-ttu-id="26d88-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="26d88-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="26d88-123">参数</span><span class="sxs-lookup"><span data-stu-id="26d88-123">Parameter</span></span> | <span data-ttu-id="26d88-124">类型</span><span class="sxs-lookup"><span data-stu-id="26d88-124">Type</span></span>   | <span data-ttu-id="26d88-125">说明</span><span class="sxs-lookup"><span data-stu-id="26d88-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="26d88-126">period</span><span class="sxs-lookup"><span data-stu-id="26d88-126">period</span></span>    | <span data-ttu-id="26d88-127">string</span><span class="sxs-lookup"><span data-stu-id="26d88-127">string</span></span> | <span data-ttu-id="26d88-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="26d88-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="26d88-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="26d88-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="26d88-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="26d88-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="26d88-131">必需。</span><span class="sxs-lookup"><span data-stu-id="26d88-131">Required.</span></span> |

<span data-ttu-id="26d88-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="26d88-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="26d88-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="26d88-133">The default output type is text/csv.</span></span> <span data-ttu-id="26d88-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="26d88-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26d88-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="26d88-135">Request headers</span></span>

| <span data-ttu-id="26d88-136">名称</span><span class="sxs-lookup"><span data-stu-id="26d88-136">Name</span></span>          | <span data-ttu-id="26d88-137">说明</span><span class="sxs-lookup"><span data-stu-id="26d88-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="26d88-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="26d88-138">Authorization</span></span> | <span data-ttu-id="26d88-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26d88-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="26d88-141">响应</span><span class="sxs-lookup"><span data-stu-id="26d88-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="26d88-142">CSV</span><span class="sxs-lookup"><span data-stu-id="26d88-142">CSV</span></span>

<span data-ttu-id="26d88-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="26d88-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="26d88-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="26d88-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="26d88-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="26d88-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="26d88-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="26d88-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="26d88-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="26d88-147">Report Refresh Date</span></span>
- <span data-ttu-id="26d88-148">Web</span><span class="sxs-lookup"><span data-stu-id="26d88-148">Web</span></span>
- <span data-ttu-id="26d88-149">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="26d88-149">Windows Phone</span></span>
- <span data-ttu-id="26d88-150">Android 手机</span><span class="sxs-lookup"><span data-stu-id="26d88-150">Android Phone</span></span>
- <span data-ttu-id="26d88-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="26d88-151">iPhone</span></span>
- <span data-ttu-id="26d88-152">iPad</span><span class="sxs-lookup"><span data-stu-id="26d88-152">iPad</span></span>
- <span data-ttu-id="26d88-153">其他</span><span class="sxs-lookup"><span data-stu-id="26d88-153">Other</span></span>
- <span data-ttu-id="26d88-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="26d88-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="26d88-155">JSON</span><span class="sxs-lookup"><span data-stu-id="26d88-155">JSON</span></span>

<span data-ttu-id="26d88-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="26d88-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26d88-157">示例</span><span class="sxs-lookup"><span data-stu-id="26d88-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="26d88-158">CSV</span><span class="sxs-lookup"><span data-stu-id="26d88-158">CSV</span></span>

<span data-ttu-id="26d88-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="26d88-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="26d88-160">请求</span><span class="sxs-lookup"><span data-stu-id="26d88-160">Request</span></span>

<span data-ttu-id="26d88-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26d88-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="26d88-162">响应</span><span class="sxs-lookup"><span data-stu-id="26d88-162">Response</span></span>

<span data-ttu-id="26d88-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26d88-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="26d88-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="26d88-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="26d88-165">JSON</span><span class="sxs-lookup"><span data-stu-id="26d88-165">JSON</span></span>

<span data-ttu-id="26d88-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="26d88-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="26d88-167">请求</span><span class="sxs-lookup"><span data-stu-id="26d88-167">Request</span></span>

<span data-ttu-id="26d88-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26d88-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="26d88-169">响应</span><span class="sxs-lookup"><span data-stu-id="26d88-169">Response</span></span>

<span data-ttu-id="26d88-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26d88-170">The following is an example of the response.</span></span>

> <span data-ttu-id="26d88-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26d88-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


