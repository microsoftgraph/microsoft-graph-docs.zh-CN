---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ceff341f4f75690263267fcc8924db19e0a19a16
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053522"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="a3a9f-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a3a9f-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="a3a9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a9f-105">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3a9f-106">权限</span><span class="sxs-lookup"><span data-stu-id="a3a9f-106">Permissions</span></span>

<span data-ttu-id="a3a9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3a9f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3a9f-109">Permission type</span></span>                        | <span data-ttu-id="a3a9f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3a9f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a3a9f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3a9f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3a9f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a9f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a3a9f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3a9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3a9f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-114">Not supported.</span></span>                           |
| <span data-ttu-id="a3a9f-115">应用</span><span class="sxs-lookup"><span data-stu-id="a3a9f-115">Application</span></span>                            | <span data-ttu-id="a3a9f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a9f-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="a3a9f-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a3a9f-118">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a3a9f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3a9f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="a3a9f-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="a3a9f-120">Function parameters</span></span>

<span data-ttu-id="a3a9f-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a3a9f-122">参数</span><span class="sxs-lookup"><span data-stu-id="a3a9f-122">Parameter</span></span> | <span data-ttu-id="a3a9f-123">类型</span><span class="sxs-lookup"><span data-stu-id="a3a9f-123">Type</span></span>   | <span data-ttu-id="a3a9f-124">说明</span><span class="sxs-lookup"><span data-stu-id="a3a9f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a3a9f-125">period</span><span class="sxs-lookup"><span data-stu-id="a3a9f-125">period</span></span>    | <span data-ttu-id="a3a9f-126">string</span><span class="sxs-lookup"><span data-stu-id="a3a9f-126">string</span></span> | <span data-ttu-id="a3a9f-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a3a9f-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a3a9f-129">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a3a9f-130">date</span><span class="sxs-lookup"><span data-stu-id="a3a9f-130">date</span></span>      | <span data-ttu-id="a3a9f-131">Date</span><span class="sxs-lookup"><span data-stu-id="a3a9f-131">Date</span></span>   | <span data-ttu-id="a3a9f-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a3a9f-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a3a9f-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a3a9f-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a3a9f-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a3a9f-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-137">The default output type is text/csv.</span></span> <span data-ttu-id="a3a9f-138">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3a9f-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3a9f-139">Request headers</span></span>

| <span data-ttu-id="a3a9f-140">名称</span><span class="sxs-lookup"><span data-stu-id="a3a9f-140">Name</span></span>          | <span data-ttu-id="a3a9f-141">说明</span><span class="sxs-lookup"><span data-stu-id="a3a9f-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3a9f-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3a9f-142">Authorization</span></span> | <span data-ttu-id="a3a9f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3a9f-145">响应</span><span class="sxs-lookup"><span data-stu-id="a3a9f-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a3a9f-146">CSV</span><span class="sxs-lookup"><span data-stu-id="a3a9f-146">CSV</span></span>

<span data-ttu-id="a3a9f-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a3a9f-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a3a9f-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a3a9f-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a3a9f-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a3a9f-151">Report Refresh Date</span></span>
- <span data-ttu-id="a3a9f-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a3a9f-152">User Principal Name</span></span>
- <span data-ttu-id="a3a9f-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a3a9f-153">Last Activity Date</span></span>
- <span data-ttu-id="a3a9f-154">已删除</span><span class="sxs-lookup"><span data-stu-id="a3a9f-154">Is Deleted</span></span>
- <span data-ttu-id="a3a9f-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="a3a9f-155">Deleted Date</span></span>
- <span data-ttu-id="a3a9f-156">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="a3a9f-156">Used Web</span></span>
- <span data-ttu-id="a3a9f-157">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="a3a9f-157">Used Windows Phone</span></span>
- <span data-ttu-id="a3a9f-158">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="a3a9f-158">Used iOS</span></span>
- <span data-ttu-id="a3a9f-159">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="a3a9f-159">Used Mac</span></span>
- <span data-ttu-id="a3a9f-160">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="a3a9f-160">Used Android Phone</span></span>
- <span data-ttu-id="a3a9f-161">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="a3a9f-161">Used Windows</span></span>
- <span data-ttu-id="a3a9f-162">使用的 Chrome 操作系统</span><span class="sxs-lookup"><span data-stu-id="a3a9f-162">Used Chrome OS</span></span>
- <span data-ttu-id="a3a9f-163">已使用的 Linux</span><span class="sxs-lookup"><span data-stu-id="a3a9f-163">Used Linux</span></span>
- <span data-ttu-id="a3a9f-164">已许可</span><span class="sxs-lookup"><span data-stu-id="a3a9f-164">Is Licensed</span></span>
- <span data-ttu-id="a3a9f-165">报表周期</span><span class="sxs-lookup"><span data-stu-id="a3a9f-165">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a3a9f-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a3a9f-166">JSON</span></span>

<span data-ttu-id="a3a9f-167">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-167">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="a3a9f-168">此请求的默认页面大小为 2000 个项目。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-168">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="a3a9f-169">示例</span><span class="sxs-lookup"><span data-stu-id="a3a9f-169">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a3a9f-170">CSV</span><span class="sxs-lookup"><span data-stu-id="a3a9f-170">CSV</span></span>

<span data-ttu-id="a3a9f-171">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-171">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a3a9f-172">请求</span><span class="sxs-lookup"><span data-stu-id="a3a9f-172">Request</span></span>

<span data-ttu-id="a3a9f-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-173">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a3a9f-174">响应</span><span class="sxs-lookup"><span data-stu-id="a3a9f-174">Response</span></span>

<span data-ttu-id="a3a9f-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a3a9f-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Used Chrome OS,Used Linux,Is Licensed,Report Period
```

### <a name="json"></a><span data-ttu-id="a3a9f-177">JSON</span><span class="sxs-lookup"><span data-stu-id="a3a9f-177">JSON</span></span>

<span data-ttu-id="a3a9f-178">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a3a9f-179">请求</span><span class="sxs-lookup"><span data-stu-id="a3a9f-179">Request</span></span>

<span data-ttu-id="a3a9f-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-180">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a3a9f-181">响应</span><span class="sxs-lookup"><span data-stu-id="a3a9f-181">Response</span></span>

<span data-ttu-id="a3a9f-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-182">The following is an example of the response.</span></span>

> <span data-ttu-id="a3a9f-183">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3a9f-183">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "isLicensed": true, 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "usedChromeOS": false, 
      "usedLinux": false, 
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


