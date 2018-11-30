---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
ms.openlocfilehash: 61954c3eb8853a74044d3da921985b63113c03b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047919"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="aef60-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="aef60-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

> <span data-ttu-id="aef60-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aef60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aef60-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aef60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aef60-106">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="aef60-106">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="aef60-107">权限</span><span class="sxs-lookup"><span data-stu-id="aef60-107">Permissions</span></span>

<span data-ttu-id="aef60-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aef60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aef60-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aef60-110">Permission type</span></span>                        | <span data-ttu-id="aef60-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aef60-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aef60-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aef60-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="aef60-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef60-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aef60-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aef60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aef60-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aef60-115">Not supported.</span></span>                           |
| <span data-ttu-id="aef60-116">应用</span><span class="sxs-lookup"><span data-stu-id="aef60-116">Application</span></span>                            | <span data-ttu-id="aef60-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef60-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aef60-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aef60-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="aef60-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="aef60-119">Function parameters</span></span>

<span data-ttu-id="aef60-120">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="aef60-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="aef60-121">参数</span><span class="sxs-lookup"><span data-stu-id="aef60-121">Parameter</span></span> | <span data-ttu-id="aef60-122">类型</span><span class="sxs-lookup"><span data-stu-id="aef60-122">Type</span></span>   | <span data-ttu-id="aef60-123">说明</span><span class="sxs-lookup"><span data-stu-id="aef60-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aef60-124">period</span><span class="sxs-lookup"><span data-stu-id="aef60-124">period</span></span>    | <span data-ttu-id="aef60-125">string</span><span class="sxs-lookup"><span data-stu-id="aef60-125">string</span></span> | <span data-ttu-id="aef60-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aef60-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aef60-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="aef60-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aef60-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="aef60-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="aef60-129">date</span><span class="sxs-lookup"><span data-stu-id="aef60-129">date</span></span>      | <span data-ttu-id="aef60-130">Date</span><span class="sxs-lookup"><span data-stu-id="aef60-130">Date</span></span>   | <span data-ttu-id="aef60-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="aef60-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="aef60-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="aef60-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="aef60-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="aef60-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="aef60-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="aef60-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="aef60-135">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aef60-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aef60-136">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="aef60-136">The default output type is text/csv.</span></span> <span data-ttu-id="aef60-137">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="aef60-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aef60-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="aef60-138">Request headers</span></span>

| <span data-ttu-id="aef60-139">名称</span><span class="sxs-lookup"><span data-stu-id="aef60-139">Name</span></span>          | <span data-ttu-id="aef60-140">说明</span><span class="sxs-lookup"><span data-stu-id="aef60-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aef60-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="aef60-141">Authorization</span></span> | <span data-ttu-id="aef60-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aef60-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aef60-144">响应</span><span class="sxs-lookup"><span data-stu-id="aef60-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aef60-145">CSV</span><span class="sxs-lookup"><span data-stu-id="aef60-145">CSV</span></span>

<span data-ttu-id="aef60-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="aef60-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aef60-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="aef60-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aef60-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="aef60-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aef60-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="aef60-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aef60-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="aef60-150">Report Refresh Date</span></span>
- <span data-ttu-id="aef60-151">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="aef60-151">User Principal Name</span></span>
- <span data-ttu-id="aef60-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="aef60-152">Last Activity Date</span></span>
- <span data-ttu-id="aef60-153">已删除</span><span class="sxs-lookup"><span data-stu-id="aef60-153">Is Deleted</span></span>
- <span data-ttu-id="aef60-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="aef60-154">Deleted Date</span></span>
- <span data-ttu-id="aef60-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="aef60-155">Used Web</span></span>
- <span data-ttu-id="aef60-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="aef60-156">Used Windows Phone</span></span>
- <span data-ttu-id="aef60-157">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="aef60-157">Used iOS</span></span>
- <span data-ttu-id="aef60-158">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="aef60-158">Used Mac</span></span>
- <span data-ttu-id="aef60-159">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="aef60-159">Used Android Phone</span></span>
- <span data-ttu-id="aef60-160">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="aef60-160">Used Windows</span></span>
- <span data-ttu-id="aef60-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="aef60-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aef60-162">JSON</span><span class="sxs-lookup"><span data-stu-id="aef60-162">JSON</span></span>

<span data-ttu-id="aef60-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="aef60-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="aef60-164">为此请求的默认页面大小是 2000年个项目。</span><span class="sxs-lookup"><span data-stu-id="aef60-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="aef60-165">示例</span><span class="sxs-lookup"><span data-stu-id="aef60-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aef60-166">CSV</span><span class="sxs-lookup"><span data-stu-id="aef60-166">CSV</span></span>

<span data-ttu-id="aef60-167">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="aef60-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aef60-168">请求</span><span class="sxs-lookup"><span data-stu-id="aef60-168">Request</span></span>

<span data-ttu-id="aef60-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aef60-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="aef60-170">响应</span><span class="sxs-lookup"><span data-stu-id="aef60-170">Response</span></span>

<span data-ttu-id="aef60-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aef60-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aef60-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="aef60-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="aef60-173">JSON</span><span class="sxs-lookup"><span data-stu-id="aef60-173">JSON</span></span>

<span data-ttu-id="aef60-174">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="aef60-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aef60-175">请求</span><span class="sxs-lookup"><span data-stu-id="aef60-175">Request</span></span>

<span data-ttu-id="aef60-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aef60-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="aef60-177">响应</span><span class="sxs-lookup"><span data-stu-id="aef60-177">Response</span></span>

<span data-ttu-id="aef60-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aef60-178">The following is an example of the response.</span></span>

> <span data-ttu-id="aef60-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aef60-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
