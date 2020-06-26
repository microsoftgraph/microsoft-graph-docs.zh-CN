---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: 按设备类型获取每日用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a0835a4d2b203f706b6917fc42854b2685fae476
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896614"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="02b2a-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="02b2a-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="02b2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02b2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02b2a-105">按设备类型获取每日用户数。</span><span class="sxs-lookup"><span data-stu-id="02b2a-105">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="02b2a-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="02b2a-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="02b2a-107">权限</span><span class="sxs-lookup"><span data-stu-id="02b2a-107">Permissions</span></span>

<span data-ttu-id="02b2a-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="02b2a-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="02b2a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b2a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02b2a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="02b2a-110">Permission type</span></span>                        | <span data-ttu-id="02b2a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02b2a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="02b2a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02b2a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="02b2a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b2a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="02b2a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02b2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02b2a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="02b2a-115">Not supported.</span></span>                           |
| <span data-ttu-id="02b2a-116">应用</span><span class="sxs-lookup"><span data-stu-id="02b2a-116">Application</span></span>                            | <span data-ttu-id="02b2a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02b2a-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="02b2a-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="02b2a-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="02b2a-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="02b2a-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="02b2a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02b2a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="02b2a-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="02b2a-121">Function parameters</span></span>

<span data-ttu-id="02b2a-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="02b2a-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="02b2a-123">参数</span><span class="sxs-lookup"><span data-stu-id="02b2a-123">Parameter</span></span> | <span data-ttu-id="02b2a-124">类型</span><span class="sxs-lookup"><span data-stu-id="02b2a-124">Type</span></span>   | <span data-ttu-id="02b2a-125">说明</span><span class="sxs-lookup"><span data-stu-id="02b2a-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="02b2a-126">period</span><span class="sxs-lookup"><span data-stu-id="02b2a-126">period</span></span>    | <span data-ttu-id="02b2a-127">string</span><span class="sxs-lookup"><span data-stu-id="02b2a-127">string</span></span> | <span data-ttu-id="02b2a-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="02b2a-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="02b2a-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="02b2a-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="02b2a-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="02b2a-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="02b2a-131">必需。</span><span class="sxs-lookup"><span data-stu-id="02b2a-131">Required.</span></span> |

<span data-ttu-id="02b2a-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02b2a-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="02b2a-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="02b2a-133">The default output type is text/csv.</span></span> <span data-ttu-id="02b2a-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="02b2a-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02b2a-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="02b2a-135">Request headers</span></span>

| <span data-ttu-id="02b2a-136">名称</span><span class="sxs-lookup"><span data-stu-id="02b2a-136">Name</span></span>          | <span data-ttu-id="02b2a-137">说明</span><span class="sxs-lookup"><span data-stu-id="02b2a-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="02b2a-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="02b2a-138">Authorization</span></span> | <span data-ttu-id="02b2a-139">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="02b2a-139">Bearer {token}.</span></span> <span data-ttu-id="02b2a-140">Required.</span><span class="sxs-lookup"><span data-stu-id="02b2a-140">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="02b2a-141">响应</span><span class="sxs-lookup"><span data-stu-id="02b2a-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="02b2a-142">CSV</span><span class="sxs-lookup"><span data-stu-id="02b2a-142">CSV</span></span>

<span data-ttu-id="02b2a-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="02b2a-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="02b2a-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="02b2a-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="02b2a-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="02b2a-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="02b2a-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="02b2a-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="02b2a-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="02b2a-147">Report Refresh Date</span></span>
- <span data-ttu-id="02b2a-148">Web</span><span class="sxs-lookup"><span data-stu-id="02b2a-148">Web</span></span>
- <span data-ttu-id="02b2a-149">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="02b2a-149">Windows Phone</span></span>
- <span data-ttu-id="02b2a-150">Android 手机</span><span class="sxs-lookup"><span data-stu-id="02b2a-150">Android Phone</span></span>
- <span data-ttu-id="02b2a-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="02b2a-151">iPhone</span></span>
- <span data-ttu-id="02b2a-152">iPad</span><span class="sxs-lookup"><span data-stu-id="02b2a-152">iPad</span></span>
- <span data-ttu-id="02b2a-153">其他</span><span class="sxs-lookup"><span data-stu-id="02b2a-153">Other</span></span>
- <span data-ttu-id="02b2a-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="02b2a-154">Report Date</span></span>
- <span data-ttu-id="02b2a-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="02b2a-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="02b2a-156">JSON</span><span class="sxs-lookup"><span data-stu-id="02b2a-156">JSON</span></span>

<span data-ttu-id="02b2a-157">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="02b2a-157">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b2a-158">示例</span><span class="sxs-lookup"><span data-stu-id="02b2a-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="02b2a-159">CSV</span><span class="sxs-lookup"><span data-stu-id="02b2a-159">CSV</span></span>

<span data-ttu-id="02b2a-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="02b2a-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="02b2a-161">请求</span><span class="sxs-lookup"><span data-stu-id="02b2a-161">Request</span></span>

<span data-ttu-id="02b2a-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02b2a-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="02b2a-163">响应</span><span class="sxs-lookup"><span data-stu-id="02b2a-163">Response</span></span>

<span data-ttu-id="02b2a-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02b2a-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="02b2a-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="02b2a-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="02b2a-166">JSON</span><span class="sxs-lookup"><span data-stu-id="02b2a-166">JSON</span></span>

<span data-ttu-id="02b2a-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="02b2a-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="02b2a-168">请求</span><span class="sxs-lookup"><span data-stu-id="02b2a-168">Request</span></span>

<span data-ttu-id="02b2a-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02b2a-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="02b2a-170">响应</span><span class="sxs-lookup"><span data-stu-id="02b2a-170">Response</span></span>

<span data-ttu-id="02b2a-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02b2a-171">The following is an example of the response.</span></span>

> <span data-ttu-id="02b2a-172">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="02b2a-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="02b2a-173">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="02b2a-173">All the properties will be returned from an actual call.</span></span>

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
