---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 06689e29143afbc318ad1c9e0866db7c6f7658ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537782"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="d7d38-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d7d38-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d38-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d7d38-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7d38-105">权限</span><span class="sxs-lookup"><span data-stu-id="d7d38-105">Permissions</span></span>

<span data-ttu-id="d7d38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7d38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7d38-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7d38-108">Permission type</span></span>                        | <span data-ttu-id="d7d38-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7d38-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d7d38-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7d38-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7d38-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7d38-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d7d38-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7d38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d38-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7d38-113">Not supported.</span></span>                           |
| <span data-ttu-id="d7d38-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7d38-114">Application</span></span>                            | <span data-ttu-id="d7d38-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7d38-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d7d38-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7d38-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="d7d38-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="d7d38-117">Function parameters</span></span>

<span data-ttu-id="d7d38-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d7d38-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d7d38-119">参数</span><span class="sxs-lookup"><span data-stu-id="d7d38-119">Parameter</span></span> | <span data-ttu-id="d7d38-120">类型</span><span class="sxs-lookup"><span data-stu-id="d7d38-120">Type</span></span>   | <span data-ttu-id="d7d38-121">说明</span><span class="sxs-lookup"><span data-stu-id="d7d38-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d7d38-122">period</span><span class="sxs-lookup"><span data-stu-id="d7d38-122">period</span></span>    | <span data-ttu-id="d7d38-123">string</span><span class="sxs-lookup"><span data-stu-id="d7d38-123">string</span></span> | <span data-ttu-id="d7d38-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d7d38-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d7d38-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d7d38-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d7d38-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d7d38-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d7d38-127">date</span><span class="sxs-lookup"><span data-stu-id="d7d38-127">date</span></span>      | <span data-ttu-id="d7d38-128">Date</span><span class="sxs-lookup"><span data-stu-id="d7d38-128">Date</span></span>   | <span data-ttu-id="d7d38-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="d7d38-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d7d38-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="d7d38-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d7d38-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="d7d38-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d7d38-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="d7d38-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d7d38-133">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d7d38-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d7d38-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d7d38-134">The default output type is text/csv.</span></span> <span data-ttu-id="d7d38-135">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d7d38-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7d38-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7d38-136">Request headers</span></span>

| <span data-ttu-id="d7d38-137">名称</span><span class="sxs-lookup"><span data-stu-id="d7d38-137">Name</span></span>          | <span data-ttu-id="d7d38-138">说明</span><span class="sxs-lookup"><span data-stu-id="d7d38-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d7d38-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d38-139">Authorization</span></span> | <span data-ttu-id="d7d38-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7d38-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d7d38-142">响应</span><span class="sxs-lookup"><span data-stu-id="d7d38-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d7d38-143">CSV</span><span class="sxs-lookup"><span data-stu-id="d7d38-143">CSV</span></span>

<span data-ttu-id="d7d38-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d7d38-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d7d38-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d7d38-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d7d38-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d7d38-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d7d38-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d7d38-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d7d38-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d7d38-148">Report Refresh Date</span></span>
- <span data-ttu-id="d7d38-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d7d38-149">User Principal Name</span></span>
- <span data-ttu-id="d7d38-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d7d38-150">Last Activity Date</span></span>
- <span data-ttu-id="d7d38-151">已删除</span><span class="sxs-lookup"><span data-stu-id="d7d38-151">Is Deleted</span></span>
- <span data-ttu-id="d7d38-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="d7d38-152">Deleted Date</span></span>
- <span data-ttu-id="d7d38-153">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="d7d38-153">Used Web</span></span>
- <span data-ttu-id="d7d38-154">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="d7d38-154">Used Windows Phone</span></span>
- <span data-ttu-id="d7d38-155">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="d7d38-155">Used iOS</span></span>
- <span data-ttu-id="d7d38-156">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="d7d38-156">Used Mac</span></span>
- <span data-ttu-id="d7d38-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="d7d38-157">Used Android Phone</span></span>
- <span data-ttu-id="d7d38-158">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="d7d38-158">Used Windows</span></span>
- <span data-ttu-id="d7d38-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="d7d38-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d7d38-160">JSON</span><span class="sxs-lookup"><span data-stu-id="d7d38-160">JSON</span></span>

<span data-ttu-id="d7d38-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d7d38-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d7d38-162">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="d7d38-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="d7d38-163">示例</span><span class="sxs-lookup"><span data-stu-id="d7d38-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d7d38-164">CSV</span><span class="sxs-lookup"><span data-stu-id="d7d38-164">CSV</span></span>

<span data-ttu-id="d7d38-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7d38-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d7d38-166">请求</span><span class="sxs-lookup"><span data-stu-id="d7d38-166">Request</span></span>

<span data-ttu-id="d7d38-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7d38-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d7d38-168">响应</span><span class="sxs-lookup"><span data-stu-id="d7d38-168">Response</span></span>

<span data-ttu-id="d7d38-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7d38-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d7d38-170">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d7d38-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d7d38-171">JSON</span><span class="sxs-lookup"><span data-stu-id="d7d38-171">JSON</span></span>

<span data-ttu-id="d7d38-172">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7d38-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d7d38-173">请求</span><span class="sxs-lookup"><span data-stu-id="d7d38-173">Request</span></span>

<span data-ttu-id="d7d38-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7d38-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d7d38-175">响应</span><span class="sxs-lookup"><span data-stu-id="d7d38-175">Response</span></span>

<span data-ttu-id="d7d38-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7d38-176">The following is an example of the response.</span></span>

> <span data-ttu-id="d7d38-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7d38-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
