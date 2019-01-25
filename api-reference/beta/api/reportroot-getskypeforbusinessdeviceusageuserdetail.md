---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: 获取用户的 Skype for Business 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8162acdbfc1cb8387e4920bb12cb15be4ef549f9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526814"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="87acd-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="87acd-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87acd-104">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="87acd-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="87acd-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="87acd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="87acd-106">权限</span><span class="sxs-lookup"><span data-stu-id="87acd-106">Permissions</span></span>

<span data-ttu-id="87acd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87acd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87acd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="87acd-109">Permission type</span></span>                        | <span data-ttu-id="87acd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87acd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="87acd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87acd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87acd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87acd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="87acd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87acd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87acd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="87acd-114">Not supported.</span></span>                           |
| <span data-ttu-id="87acd-115">应用</span><span class="sxs-lookup"><span data-stu-id="87acd-115">Application</span></span>                            | <span data-ttu-id="87acd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87acd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="87acd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87acd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="87acd-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="87acd-118">Function parameters</span></span>

<span data-ttu-id="87acd-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="87acd-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="87acd-120">参数</span><span class="sxs-lookup"><span data-stu-id="87acd-120">Parameter</span></span> | <span data-ttu-id="87acd-121">类型</span><span class="sxs-lookup"><span data-stu-id="87acd-121">Type</span></span>   | <span data-ttu-id="87acd-122">说明</span><span class="sxs-lookup"><span data-stu-id="87acd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="87acd-123">period</span><span class="sxs-lookup"><span data-stu-id="87acd-123">period</span></span>    | <span data-ttu-id="87acd-124">string</span><span class="sxs-lookup"><span data-stu-id="87acd-124">string</span></span> | <span data-ttu-id="87acd-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="87acd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="87acd-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="87acd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="87acd-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="87acd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="87acd-128">date</span><span class="sxs-lookup"><span data-stu-id="87acd-128">date</span></span>      | <span data-ttu-id="87acd-129">Date</span><span class="sxs-lookup"><span data-stu-id="87acd-129">Date</span></span>   | <span data-ttu-id="87acd-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="87acd-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="87acd-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="87acd-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="87acd-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="87acd-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="87acd-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="87acd-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="87acd-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="87acd-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="87acd-135">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="87acd-135">The default output type is text/csv.</span></span> <span data-ttu-id="87acd-136">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="87acd-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87acd-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="87acd-137">Request headers</span></span>

| <span data-ttu-id="87acd-138">名称</span><span class="sxs-lookup"><span data-stu-id="87acd-138">Name</span></span>          | <span data-ttu-id="87acd-139">说明</span><span class="sxs-lookup"><span data-stu-id="87acd-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="87acd-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="87acd-140">Authorization</span></span> | <span data-ttu-id="87acd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87acd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="87acd-143">响应</span><span class="sxs-lookup"><span data-stu-id="87acd-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="87acd-144">CSV</span><span class="sxs-lookup"><span data-stu-id="87acd-144">CSV</span></span>

<span data-ttu-id="87acd-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="87acd-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="87acd-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="87acd-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="87acd-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="87acd-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="87acd-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="87acd-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="87acd-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="87acd-149">Report Refresh Date</span></span>
- <span data-ttu-id="87acd-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="87acd-150">User Principal Name</span></span>
- <span data-ttu-id="87acd-151">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="87acd-151">Last Activity Date</span></span>
- <span data-ttu-id="87acd-152">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="87acd-152">Used Windows</span></span>
- <span data-ttu-id="87acd-153">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="87acd-153">Used Windows Phone</span></span>
- <span data-ttu-id="87acd-154">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="87acd-154">Used Android Phone</span></span>
- <span data-ttu-id="87acd-155">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="87acd-155">Used iPhone</span></span>
- <span data-ttu-id="87acd-156">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="87acd-156">Used iPad</span></span>
- <span data-ttu-id="87acd-157">报表周期</span><span class="sxs-lookup"><span data-stu-id="87acd-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="87acd-158">JSON</span><span class="sxs-lookup"><span data-stu-id="87acd-158">JSON</span></span>

<span data-ttu-id="87acd-159">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="87acd-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="87acd-160">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="87acd-160">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="87acd-161">示例</span><span class="sxs-lookup"><span data-stu-id="87acd-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="87acd-162">CSV</span><span class="sxs-lookup"><span data-stu-id="87acd-162">CSV</span></span>

<span data-ttu-id="87acd-163">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="87acd-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="87acd-164">请求</span><span class="sxs-lookup"><span data-stu-id="87acd-164">Request</span></span>

<span data-ttu-id="87acd-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="87acd-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="87acd-166">响应</span><span class="sxs-lookup"><span data-stu-id="87acd-166">Response</span></span>

<span data-ttu-id="87acd-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="87acd-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="87acd-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="87acd-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="87acd-169">JSON</span><span class="sxs-lookup"><span data-stu-id="87acd-169">JSON</span></span>

<span data-ttu-id="87acd-170">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="87acd-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="87acd-171">请求</span><span class="sxs-lookup"><span data-stu-id="87acd-171">Request</span></span>

<span data-ttu-id="87acd-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="87acd-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="87acd-173">响应</span><span class="sxs-lookup"><span data-stu-id="87acd-173">Response</span></span>

<span data-ttu-id="87acd-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="87acd-174">The following is an example of the response.</span></span>

> <span data-ttu-id="87acd-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87acd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
