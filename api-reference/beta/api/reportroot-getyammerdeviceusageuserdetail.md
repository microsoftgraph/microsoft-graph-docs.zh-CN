---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0e8707ebdf2de009794f8df274df1870e0a19259
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896607"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="b694c-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="b694c-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="b694c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b694c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b694c-105">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b694c-105">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="b694c-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="b694c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="b694c-107">权限</span><span class="sxs-lookup"><span data-stu-id="b694c-107">Permissions</span></span>

<span data-ttu-id="b694c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b694c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b694c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b694c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b694c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b694c-110">Permission type</span></span>                        | <span data-ttu-id="b694c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b694c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b694c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b694c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b694c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b694c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b694c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b694c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b694c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b694c-115">Not supported.</span></span>                           |
| <span data-ttu-id="b694c-116">应用</span><span class="sxs-lookup"><span data-stu-id="b694c-116">Application</span></span>                            | <span data-ttu-id="b694c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b694c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="b694c-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="b694c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b694c-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="b694c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b694c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b694c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b694c-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="b694c-121">Function parameters</span></span>

<span data-ttu-id="b694c-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b694c-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b694c-123">参数</span><span class="sxs-lookup"><span data-stu-id="b694c-123">Parameter</span></span> | <span data-ttu-id="b694c-124">类型</span><span class="sxs-lookup"><span data-stu-id="b694c-124">Type</span></span>   | <span data-ttu-id="b694c-125">说明</span><span class="sxs-lookup"><span data-stu-id="b694c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b694c-126">period</span><span class="sxs-lookup"><span data-stu-id="b694c-126">period</span></span>    | <span data-ttu-id="b694c-127">string</span><span class="sxs-lookup"><span data-stu-id="b694c-127">string</span></span> | <span data-ttu-id="b694c-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b694c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b694c-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b694c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b694c-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b694c-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b694c-131">date</span><span class="sxs-lookup"><span data-stu-id="b694c-131">date</span></span>      | <span data-ttu-id="b694c-132">Date</span><span class="sxs-lookup"><span data-stu-id="b694c-132">Date</span></span>   | <span data-ttu-id="b694c-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b694c-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b694c-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b694c-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b694c-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b694c-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b694c-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b694c-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b694c-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b694c-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b694c-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="b694c-138">The default output type is text/csv.</span></span> <span data-ttu-id="b694c-139">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="b694c-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b694c-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="b694c-140">Request headers</span></span>

| <span data-ttu-id="b694c-141">名称</span><span class="sxs-lookup"><span data-stu-id="b694c-141">Name</span></span>          | <span data-ttu-id="b694c-142">说明</span><span class="sxs-lookup"><span data-stu-id="b694c-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b694c-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="b694c-143">Authorization</span></span> | <span data-ttu-id="b694c-144">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b694c-144">Bearer {token}.</span></span> <span data-ttu-id="b694c-145">Required.</span><span class="sxs-lookup"><span data-stu-id="b694c-145">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b694c-146">响应</span><span class="sxs-lookup"><span data-stu-id="b694c-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b694c-147">CSV</span><span class="sxs-lookup"><span data-stu-id="b694c-147">CSV</span></span>

<span data-ttu-id="b694c-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b694c-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b694c-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b694c-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b694c-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b694c-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b694c-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b694c-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b694c-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b694c-152">Report Refresh Date</span></span>
- <span data-ttu-id="b694c-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b694c-153">User Principal Name</span></span>
- <span data-ttu-id="b694c-154">显示名称</span><span class="sxs-lookup"><span data-stu-id="b694c-154">Display Name</span></span>
- <span data-ttu-id="b694c-155">用户状态</span><span class="sxs-lookup"><span data-stu-id="b694c-155">User State</span></span>
- <span data-ttu-id="b694c-156">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="b694c-156">State Change Date</span></span>
- <span data-ttu-id="b694c-157">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b694c-157">Last Activity Date</span></span>
- <span data-ttu-id="b694c-158">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="b694c-158">Used Web</span></span>
- <span data-ttu-id="b694c-159">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="b694c-159">Used Windows Phone</span></span>
- <span data-ttu-id="b694c-160">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="b694c-160">Used Android Phone</span></span>
- <span data-ttu-id="b694c-161">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="b694c-161">Used iPhone</span></span>
- <span data-ttu-id="b694c-162">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="b694c-162">Used iPad</span></span>
- <span data-ttu-id="b694c-163">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="b694c-163">Used Others</span></span>
- <span data-ttu-id="b694c-164">报表周期</span><span class="sxs-lookup"><span data-stu-id="b694c-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b694c-165">JSON</span><span class="sxs-lookup"><span data-stu-id="b694c-165">JSON</span></span>

<span data-ttu-id="b694c-166">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b694c-166">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b694c-167">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="b694c-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b694c-168">示例</span><span class="sxs-lookup"><span data-stu-id="b694c-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b694c-169">CSV</span><span class="sxs-lookup"><span data-stu-id="b694c-169">CSV</span></span>

<span data-ttu-id="b694c-170">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="b694c-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b694c-171">请求</span><span class="sxs-lookup"><span data-stu-id="b694c-171">Request</span></span>

<span data-ttu-id="b694c-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b694c-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="b694c-173">响应</span><span class="sxs-lookup"><span data-stu-id="b694c-173">Response</span></span>

<span data-ttu-id="b694c-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b694c-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b694c-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b694c-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b694c-176">JSON</span><span class="sxs-lookup"><span data-stu-id="b694c-176">JSON</span></span>

<span data-ttu-id="b694c-177">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b694c-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b694c-178">请求</span><span class="sxs-lookup"><span data-stu-id="b694c-178">Request</span></span>

<span data-ttu-id="b694c-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b694c-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="b694c-180">响应</span><span class="sxs-lookup"><span data-stu-id="b694c-180">Response</span></span>

<span data-ttu-id="b694c-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b694c-181">The following is an example of the response.</span></span>

> <span data-ttu-id="b694c-182">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b694c-182">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b694c-183">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b694c-183">All the properties will be returned from an actual call.</span></span>

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
