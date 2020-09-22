---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c7a32567ab2fbe202860f9b0bc1af277a0042d74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053095"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="9d422-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="9d422-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="9d422-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d422-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d422-105">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9d422-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d422-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d422-106">Permissions</span></span>

<span data-ttu-id="9d422-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d422-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d422-109">Permission type</span></span>                        | <span data-ttu-id="9d422-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d422-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9d422-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d422-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d422-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d422-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9d422-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d422-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d422-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d422-114">Not supported.</span></span>                           |
| <span data-ttu-id="9d422-115">应用</span><span class="sxs-lookup"><span data-stu-id="9d422-115">Application</span></span>                            | <span data-ttu-id="9d422-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d422-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="9d422-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="9d422-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9d422-118">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="9d422-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9d422-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d422-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="9d422-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="9d422-120">Function parameters</span></span>

<span data-ttu-id="9d422-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="9d422-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9d422-122">参数</span><span class="sxs-lookup"><span data-stu-id="9d422-122">Parameter</span></span> | <span data-ttu-id="9d422-123">类型</span><span class="sxs-lookup"><span data-stu-id="9d422-123">Type</span></span>   | <span data-ttu-id="9d422-124">说明</span><span class="sxs-lookup"><span data-stu-id="9d422-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9d422-125">period</span><span class="sxs-lookup"><span data-stu-id="9d422-125">period</span></span>    | <span data-ttu-id="9d422-126">string</span><span class="sxs-lookup"><span data-stu-id="9d422-126">string</span></span> | <span data-ttu-id="9d422-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9d422-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9d422-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9d422-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9d422-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9d422-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9d422-130">date</span><span class="sxs-lookup"><span data-stu-id="9d422-130">date</span></span>      | <span data-ttu-id="9d422-131">Date</span><span class="sxs-lookup"><span data-stu-id="9d422-131">Date</span></span>   | <span data-ttu-id="9d422-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="9d422-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9d422-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="9d422-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9d422-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="9d422-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9d422-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="9d422-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9d422-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9d422-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9d422-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="9d422-137">The default output type is text/csv.</span></span> <span data-ttu-id="9d422-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="9d422-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d422-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d422-139">Request headers</span></span>

| <span data-ttu-id="9d422-140">名称</span><span class="sxs-lookup"><span data-stu-id="9d422-140">Name</span></span>          | <span data-ttu-id="9d422-141">说明</span><span class="sxs-lookup"><span data-stu-id="9d422-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9d422-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d422-142">Authorization</span></span> | <span data-ttu-id="9d422-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d422-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9d422-145">响应</span><span class="sxs-lookup"><span data-stu-id="9d422-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9d422-146">CSV</span><span class="sxs-lookup"><span data-stu-id="9d422-146">CSV</span></span>

<span data-ttu-id="9d422-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9d422-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9d422-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9d422-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9d422-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9d422-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9d422-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9d422-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9d422-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9d422-151">Report Refresh Date</span></span>
- <span data-ttu-id="9d422-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9d422-152">User Principal Name</span></span>
- <span data-ttu-id="9d422-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9d422-153">Last Activity Date</span></span>
- <span data-ttu-id="9d422-154">已删除</span><span class="sxs-lookup"><span data-stu-id="9d422-154">Is Deleted</span></span>
- <span data-ttu-id="9d422-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="9d422-155">Deleted Date</span></span>
- <span data-ttu-id="9d422-156">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="9d422-156">Used Web</span></span>
- <span data-ttu-id="9d422-157">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="9d422-157">Used Windows Phone</span></span>
- <span data-ttu-id="9d422-158">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="9d422-158">Used iOS</span></span>
- <span data-ttu-id="9d422-159">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="9d422-159">Used Mac</span></span>
- <span data-ttu-id="9d422-160">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="9d422-160">Used Android Phone</span></span>
- <span data-ttu-id="9d422-161">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="9d422-161">Used Windows</span></span>
- <span data-ttu-id="9d422-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="9d422-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9d422-163">JSON</span><span class="sxs-lookup"><span data-stu-id="9d422-163">JSON</span></span>

<span data-ttu-id="9d422-164">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="9d422-164">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9d422-165">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="9d422-165">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="9d422-166">示例</span><span class="sxs-lookup"><span data-stu-id="9d422-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9d422-167">CSV</span><span class="sxs-lookup"><span data-stu-id="9d422-167">CSV</span></span>

<span data-ttu-id="9d422-168">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="9d422-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9d422-169">请求</span><span class="sxs-lookup"><span data-stu-id="9d422-169">Request</span></span>

<span data-ttu-id="9d422-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d422-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="9d422-171">响应</span><span class="sxs-lookup"><span data-stu-id="9d422-171">Response</span></span>

<span data-ttu-id="9d422-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d422-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9d422-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9d422-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="9d422-174">JSON</span><span class="sxs-lookup"><span data-stu-id="9d422-174">JSON</span></span>

<span data-ttu-id="9d422-175">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="9d422-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9d422-176">请求</span><span class="sxs-lookup"><span data-stu-id="9d422-176">Request</span></span>

<span data-ttu-id="9d422-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d422-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="9d422-178">响应</span><span class="sxs-lookup"><span data-stu-id="9d422-178">Response</span></span>

<span data-ttu-id="9d422-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d422-179">The following is an example of the response.</span></span>

> <span data-ttu-id="9d422-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d422-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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


