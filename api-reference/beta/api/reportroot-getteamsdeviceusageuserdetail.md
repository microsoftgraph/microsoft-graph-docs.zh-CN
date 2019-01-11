---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.openlocfilehash: ade8bbcd2ce680bb7103bd0e9dbb09f3d49d1b03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842208"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="a0240-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a0240-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

> <span data-ttu-id="a0240-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0240-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0240-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0240-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0240-106">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0240-106">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0240-107">权限</span><span class="sxs-lookup"><span data-stu-id="a0240-107">Permissions</span></span>

<span data-ttu-id="a0240-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0240-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0240-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0240-110">Permission type</span></span>                        | <span data-ttu-id="a0240-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0240-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a0240-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0240-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0240-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0240-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a0240-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0240-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0240-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0240-115">Not supported.</span></span>                           |
| <span data-ttu-id="a0240-116">应用</span><span class="sxs-lookup"><span data-stu-id="a0240-116">Application</span></span>                            | <span data-ttu-id="a0240-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0240-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a0240-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0240-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="a0240-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="a0240-119">Function parameters</span></span>

<span data-ttu-id="a0240-120">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="a0240-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a0240-121">参数</span><span class="sxs-lookup"><span data-stu-id="a0240-121">Parameter</span></span> | <span data-ttu-id="a0240-122">类型</span><span class="sxs-lookup"><span data-stu-id="a0240-122">Type</span></span>   | <span data-ttu-id="a0240-123">说明</span><span class="sxs-lookup"><span data-stu-id="a0240-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a0240-124">period</span><span class="sxs-lookup"><span data-stu-id="a0240-124">period</span></span>    | <span data-ttu-id="a0240-125">string</span><span class="sxs-lookup"><span data-stu-id="a0240-125">string</span></span> | <span data-ttu-id="a0240-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a0240-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a0240-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a0240-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a0240-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a0240-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a0240-129">date</span><span class="sxs-lookup"><span data-stu-id="a0240-129">date</span></span>      | <span data-ttu-id="a0240-130">Date</span><span class="sxs-lookup"><span data-stu-id="a0240-130">Date</span></span>   | <span data-ttu-id="a0240-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a0240-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a0240-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a0240-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a0240-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a0240-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a0240-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a0240-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a0240-135">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0240-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a0240-136">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="a0240-136">The default output type is text/csv.</span></span> <span data-ttu-id="a0240-137">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="a0240-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0240-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0240-138">Request headers</span></span>

| <span data-ttu-id="a0240-139">名称</span><span class="sxs-lookup"><span data-stu-id="a0240-139">Name</span></span>          | <span data-ttu-id="a0240-140">说明</span><span class="sxs-lookup"><span data-stu-id="a0240-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a0240-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0240-141">Authorization</span></span> | <span data-ttu-id="a0240-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0240-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a0240-144">响应</span><span class="sxs-lookup"><span data-stu-id="a0240-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a0240-145">CSV</span><span class="sxs-lookup"><span data-stu-id="a0240-145">CSV</span></span>

<span data-ttu-id="a0240-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a0240-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a0240-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a0240-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a0240-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a0240-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a0240-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a0240-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a0240-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a0240-150">Report Refresh Date</span></span>
- <span data-ttu-id="a0240-151">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a0240-151">User Principal Name</span></span>
- <span data-ttu-id="a0240-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a0240-152">Last Activity Date</span></span>
- <span data-ttu-id="a0240-153">已删除</span><span class="sxs-lookup"><span data-stu-id="a0240-153">Is Deleted</span></span>
- <span data-ttu-id="a0240-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="a0240-154">Deleted Date</span></span>
- <span data-ttu-id="a0240-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="a0240-155">Used Web</span></span>
- <span data-ttu-id="a0240-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="a0240-156">Used Windows Phone</span></span>
- <span data-ttu-id="a0240-157">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="a0240-157">Used iOS</span></span>
- <span data-ttu-id="a0240-158">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="a0240-158">Used Mac</span></span>
- <span data-ttu-id="a0240-159">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="a0240-159">Used Android Phone</span></span>
- <span data-ttu-id="a0240-160">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="a0240-160">Used Windows</span></span>
- <span data-ttu-id="a0240-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="a0240-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a0240-162">JSON</span><span class="sxs-lookup"><span data-stu-id="a0240-162">JSON</span></span>

<span data-ttu-id="a0240-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a0240-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="a0240-164">为此请求的默认页面大小是 2000年个项目。</span><span class="sxs-lookup"><span data-stu-id="a0240-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="a0240-165">示例</span><span class="sxs-lookup"><span data-stu-id="a0240-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a0240-166">CSV</span><span class="sxs-lookup"><span data-stu-id="a0240-166">CSV</span></span>

<span data-ttu-id="a0240-167">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="a0240-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a0240-168">请求</span><span class="sxs-lookup"><span data-stu-id="a0240-168">Request</span></span>

<span data-ttu-id="a0240-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0240-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a0240-170">响应</span><span class="sxs-lookup"><span data-stu-id="a0240-170">Response</span></span>

<span data-ttu-id="a0240-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0240-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a0240-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a0240-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a0240-173">JSON</span><span class="sxs-lookup"><span data-stu-id="a0240-173">JSON</span></span>

<span data-ttu-id="a0240-174">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a0240-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a0240-175">请求</span><span class="sxs-lookup"><span data-stu-id="a0240-175">Request</span></span>

<span data-ttu-id="a0240-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0240-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a0240-177">响应</span><span class="sxs-lookup"><span data-stu-id="a0240-177">Response</span></span>

<span data-ttu-id="a0240-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0240-178">The following is an example of the response.</span></span>

> <span data-ttu-id="a0240-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0240-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
