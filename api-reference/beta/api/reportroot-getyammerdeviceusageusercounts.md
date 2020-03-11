---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: 按设备类型获取每日用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bf814775b7e54164af6827d77cb3413db9b10ee8
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590366"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="03644-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="03644-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="03644-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03644-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03644-105">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="03644-105">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="03644-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="03644-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="03644-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="03644-107">Permissions</span></span>

<span data-ttu-id="03644-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03644-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03644-110">Permission type</span></span>                        | <span data-ttu-id="03644-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03644-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="03644-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03644-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="03644-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03644-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="03644-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03644-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03644-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03644-115">Not supported.</span></span>                           |
| <span data-ttu-id="03644-116">应用</span><span class="sxs-lookup"><span data-stu-id="03644-116">Application</span></span>                            | <span data-ttu-id="03644-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03644-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="03644-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="03644-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="03644-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="03644-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="03644-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03644-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="03644-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="03644-121">Function parameters</span></span>

<span data-ttu-id="03644-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="03644-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="03644-123">参数</span><span class="sxs-lookup"><span data-stu-id="03644-123">Parameter</span></span> | <span data-ttu-id="03644-124">类型</span><span class="sxs-lookup"><span data-stu-id="03644-124">Type</span></span>   | <span data-ttu-id="03644-125">Description</span><span class="sxs-lookup"><span data-stu-id="03644-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="03644-126">period</span><span class="sxs-lookup"><span data-stu-id="03644-126">period</span></span>    | <span data-ttu-id="03644-127">string</span><span class="sxs-lookup"><span data-stu-id="03644-127">string</span></span> | <span data-ttu-id="03644-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="03644-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="03644-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="03644-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="03644-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="03644-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="03644-131">必需。</span><span class="sxs-lookup"><span data-stu-id="03644-131">Required.</span></span> |

<span data-ttu-id="03644-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="03644-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="03644-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="03644-133">The default output type is text/csv.</span></span> <span data-ttu-id="03644-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="03644-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03644-135">请求头</span><span class="sxs-lookup"><span data-stu-id="03644-135">Request headers</span></span>

| <span data-ttu-id="03644-136">名称</span><span class="sxs-lookup"><span data-stu-id="03644-136">Name</span></span>          | <span data-ttu-id="03644-137">说明</span><span class="sxs-lookup"><span data-stu-id="03644-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="03644-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="03644-138">Authorization</span></span> | <span data-ttu-id="03644-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03644-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="03644-141">响应</span><span class="sxs-lookup"><span data-stu-id="03644-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="03644-142">CSV</span><span class="sxs-lookup"><span data-stu-id="03644-142">CSV</span></span>

<span data-ttu-id="03644-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="03644-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="03644-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="03644-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="03644-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="03644-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="03644-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="03644-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="03644-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="03644-147">Report Refresh Date</span></span>
- <span data-ttu-id="03644-148">Web</span><span class="sxs-lookup"><span data-stu-id="03644-148">Web</span></span>
- <span data-ttu-id="03644-149">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="03644-149">Windows Phone</span></span>
- <span data-ttu-id="03644-150">Android 手机</span><span class="sxs-lookup"><span data-stu-id="03644-150">Android Phone</span></span>
- <span data-ttu-id="03644-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="03644-151">iPhone</span></span>
- <span data-ttu-id="03644-152">iPad</span><span class="sxs-lookup"><span data-stu-id="03644-152">iPad</span></span>
- <span data-ttu-id="03644-153">其他</span><span class="sxs-lookup"><span data-stu-id="03644-153">Other</span></span>
- <span data-ttu-id="03644-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="03644-154">Report Date</span></span>
- <span data-ttu-id="03644-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="03644-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="03644-156">JSON</span><span class="sxs-lookup"><span data-stu-id="03644-156">JSON</span></span>

<span data-ttu-id="03644-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="03644-157">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03644-158">示例</span><span class="sxs-lookup"><span data-stu-id="03644-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="03644-159">CSV</span><span class="sxs-lookup"><span data-stu-id="03644-159">CSV</span></span>

<span data-ttu-id="03644-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="03644-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="03644-161">请求</span><span class="sxs-lookup"><span data-stu-id="03644-161">Request</span></span>

<span data-ttu-id="03644-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03644-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="03644-163">响应</span><span class="sxs-lookup"><span data-stu-id="03644-163">Response</span></span>

<span data-ttu-id="03644-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="03644-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="03644-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="03644-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="03644-166">JSON</span><span class="sxs-lookup"><span data-stu-id="03644-166">JSON</span></span>

<span data-ttu-id="03644-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="03644-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="03644-168">请求</span><span class="sxs-lookup"><span data-stu-id="03644-168">Request</span></span>

<span data-ttu-id="03644-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03644-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="03644-170">响应</span><span class="sxs-lookup"><span data-stu-id="03644-170">Response</span></span>

<span data-ttu-id="03644-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03644-171">The following is an example of the response.</span></span>

> <span data-ttu-id="03644-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="03644-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
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
