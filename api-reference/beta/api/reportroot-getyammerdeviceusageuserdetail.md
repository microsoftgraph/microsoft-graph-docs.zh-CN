---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 37e3a5fae633dd3d202c82d54573a77a8f6dfd6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537848"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="854fa-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="854fa-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="854fa-104">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="854fa-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="854fa-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="854fa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="854fa-106">权限</span><span class="sxs-lookup"><span data-stu-id="854fa-106">Permissions</span></span>

<span data-ttu-id="854fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="854fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="854fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="854fa-109">Permission type</span></span>                        | <span data-ttu-id="854fa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="854fa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="854fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="854fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="854fa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="854fa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="854fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="854fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="854fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="854fa-114">Not supported.</span></span>                           |
| <span data-ttu-id="854fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="854fa-115">Application</span></span>                            | <span data-ttu-id="854fa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="854fa-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="854fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="854fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="854fa-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="854fa-118">Function parameters</span></span>

<span data-ttu-id="854fa-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="854fa-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="854fa-120">参数</span><span class="sxs-lookup"><span data-stu-id="854fa-120">Parameter</span></span> | <span data-ttu-id="854fa-121">类型</span><span class="sxs-lookup"><span data-stu-id="854fa-121">Type</span></span>   | <span data-ttu-id="854fa-122">说明</span><span class="sxs-lookup"><span data-stu-id="854fa-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="854fa-123">period</span><span class="sxs-lookup"><span data-stu-id="854fa-123">period</span></span>    | <span data-ttu-id="854fa-124">string</span><span class="sxs-lookup"><span data-stu-id="854fa-124">string</span></span> | <span data-ttu-id="854fa-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="854fa-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="854fa-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="854fa-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="854fa-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="854fa-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="854fa-128">date</span><span class="sxs-lookup"><span data-stu-id="854fa-128">date</span></span>      | <span data-ttu-id="854fa-129">Date</span><span class="sxs-lookup"><span data-stu-id="854fa-129">Date</span></span>   | <span data-ttu-id="854fa-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="854fa-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="854fa-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="854fa-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="854fa-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="854fa-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="854fa-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="854fa-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="854fa-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="854fa-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="854fa-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="854fa-135">The default output type is text/csv.</span></span> <span data-ttu-id="854fa-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="854fa-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="854fa-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="854fa-137">Request headers</span></span>

| <span data-ttu-id="854fa-138">名称</span><span class="sxs-lookup"><span data-stu-id="854fa-138">Name</span></span>          | <span data-ttu-id="854fa-139">说明</span><span class="sxs-lookup"><span data-stu-id="854fa-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="854fa-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="854fa-140">Authorization</span></span> | <span data-ttu-id="854fa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="854fa-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="854fa-143">响应</span><span class="sxs-lookup"><span data-stu-id="854fa-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="854fa-144">CSV</span><span class="sxs-lookup"><span data-stu-id="854fa-144">CSV</span></span>

<span data-ttu-id="854fa-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="854fa-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="854fa-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="854fa-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="854fa-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="854fa-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="854fa-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="854fa-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="854fa-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="854fa-149">Report Refresh Date</span></span>
- <span data-ttu-id="854fa-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="854fa-150">User Principal Name</span></span>
- <span data-ttu-id="854fa-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="854fa-151">Display Name</span></span>
- <span data-ttu-id="854fa-152">用户状态</span><span class="sxs-lookup"><span data-stu-id="854fa-152">User State</span></span>
- <span data-ttu-id="854fa-153">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="854fa-153">State Change Date</span></span>
- <span data-ttu-id="854fa-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="854fa-154">Last Activity Date</span></span>
- <span data-ttu-id="854fa-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="854fa-155">Used Web</span></span>
- <span data-ttu-id="854fa-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="854fa-156">Used Windows Phone</span></span>
- <span data-ttu-id="854fa-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="854fa-157">Used Android Phone</span></span>
- <span data-ttu-id="854fa-158">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="854fa-158">Used iPhone</span></span>
- <span data-ttu-id="854fa-159">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="854fa-159">Used iPad</span></span>
- <span data-ttu-id="854fa-160">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="854fa-160">Used Others</span></span>
- <span data-ttu-id="854fa-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="854fa-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="854fa-162">JSON</span><span class="sxs-lookup"><span data-stu-id="854fa-162">JSON</span></span>

<span data-ttu-id="854fa-163">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="854fa-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="854fa-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="854fa-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="854fa-165">示例</span><span class="sxs-lookup"><span data-stu-id="854fa-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="854fa-166">CSV</span><span class="sxs-lookup"><span data-stu-id="854fa-166">CSV</span></span>

<span data-ttu-id="854fa-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="854fa-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="854fa-168">请求</span><span class="sxs-lookup"><span data-stu-id="854fa-168">Request</span></span>

<span data-ttu-id="854fa-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="854fa-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="854fa-170">响应</span><span class="sxs-lookup"><span data-stu-id="854fa-170">Response</span></span>

<span data-ttu-id="854fa-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="854fa-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="854fa-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="854fa-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="854fa-173">JSON</span><span class="sxs-lookup"><span data-stu-id="854fa-173">JSON</span></span>

<span data-ttu-id="854fa-174">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="854fa-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="854fa-175">请求</span><span class="sxs-lookup"><span data-stu-id="854fa-175">Request</span></span>

<span data-ttu-id="854fa-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="854fa-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="854fa-177">响应</span><span class="sxs-lookup"><span data-stu-id="854fa-177">Response</span></span>

<span data-ttu-id="854fa-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="854fa-178">The following is an example of the response.</span></span>

> <span data-ttu-id="854fa-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="854fa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
