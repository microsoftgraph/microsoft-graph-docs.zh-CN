---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c1098bdda5d832aa98934b91c501f4e91a3512dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522544"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="9b401-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="9b401-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b401-104">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="9b401-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b401-105">权限</span><span class="sxs-lookup"><span data-stu-id="9b401-105">Permissions</span></span>

<span data-ttu-id="9b401-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b401-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b401-108">Permission type</span></span>                        | <span data-ttu-id="9b401-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b401-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b401-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b401-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b401-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b401-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b401-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b401-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b401-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b401-113">Not supported.</span></span>                           |
| <span data-ttu-id="9b401-114">应用</span><span class="sxs-lookup"><span data-stu-id="9b401-114">Application</span></span>                            | <span data-ttu-id="9b401-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b401-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9b401-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b401-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="9b401-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="9b401-117">Function parameters</span></span>

<span data-ttu-id="9b401-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="9b401-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9b401-119">参数</span><span class="sxs-lookup"><span data-stu-id="9b401-119">Parameter</span></span> | <span data-ttu-id="9b401-120">类型</span><span class="sxs-lookup"><span data-stu-id="9b401-120">Type</span></span>   | <span data-ttu-id="9b401-121">说明</span><span class="sxs-lookup"><span data-stu-id="9b401-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9b401-122">period</span><span class="sxs-lookup"><span data-stu-id="9b401-122">period</span></span>    | <span data-ttu-id="9b401-123">string</span><span class="sxs-lookup"><span data-stu-id="9b401-123">string</span></span> | <span data-ttu-id="9b401-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9b401-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9b401-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9b401-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9b401-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9b401-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9b401-127">必需。</span><span class="sxs-lookup"><span data-stu-id="9b401-127">Required.</span></span> |

<span data-ttu-id="9b401-128">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9b401-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9b401-129">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="9b401-129">The default output type is text/csv.</span></span> <span data-ttu-id="9b401-130">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="9b401-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b401-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b401-131">Request headers</span></span>

| <span data-ttu-id="9b401-132">名称</span><span class="sxs-lookup"><span data-stu-id="9b401-132">Name</span></span>          | <span data-ttu-id="9b401-133">说明</span><span class="sxs-lookup"><span data-stu-id="9b401-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9b401-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b401-134">Authorization</span></span> | <span data-ttu-id="9b401-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b401-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9b401-137">响应</span><span class="sxs-lookup"><span data-stu-id="9b401-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9b401-138">CSV</span><span class="sxs-lookup"><span data-stu-id="9b401-138">CSV</span></span>

<span data-ttu-id="9b401-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9b401-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b401-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9b401-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b401-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9b401-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b401-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9b401-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b401-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9b401-143">Report Refresh Date</span></span>
- <span data-ttu-id="9b401-144">Web</span><span class="sxs-lookup"><span data-stu-id="9b401-144">Web</span></span>
- <span data-ttu-id="9b401-145">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="9b401-145">Windows Phone</span></span>
- <span data-ttu-id="9b401-146">Android 手机</span><span class="sxs-lookup"><span data-stu-id="9b401-146">Android Phone</span></span>
- <span data-ttu-id="9b401-147">iOS</span><span class="sxs-lookup"><span data-stu-id="9b401-147">iOS</span></span>
- <span data-ttu-id="9b401-148">Mac</span><span class="sxs-lookup"><span data-stu-id="9b401-148">Mac</span></span>
- <span data-ttu-id="9b401-149">Windows</span><span class="sxs-lookup"><span data-stu-id="9b401-149">Windows</span></span>
- <span data-ttu-id="9b401-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="9b401-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9b401-151">JSON</span><span class="sxs-lookup"><span data-stu-id="9b401-151">JSON</span></span>

<span data-ttu-id="9b401-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="9b401-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b401-153">示例</span><span class="sxs-lookup"><span data-stu-id="9b401-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9b401-154">CSV</span><span class="sxs-lookup"><span data-stu-id="9b401-154">CSV</span></span>

<span data-ttu-id="9b401-155">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="9b401-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9b401-156">请求</span><span class="sxs-lookup"><span data-stu-id="9b401-156">Request</span></span>

<span data-ttu-id="9b401-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b401-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9b401-158">响应</span><span class="sxs-lookup"><span data-stu-id="9b401-158">Response</span></span>

<span data-ttu-id="9b401-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9b401-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9b401-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9b401-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="9b401-161">JSON</span><span class="sxs-lookup"><span data-stu-id="9b401-161">JSON</span></span>

<span data-ttu-id="9b401-162">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="9b401-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9b401-163">请求</span><span class="sxs-lookup"><span data-stu-id="9b401-163">Request</span></span>

<span data-ttu-id="9b401-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b401-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9b401-165">响应</span><span class="sxs-lookup"><span data-stu-id="9b401-165">Response</span></span>

<span data-ttu-id="9b401-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b401-166">The following is an example of the response.</span></span>

> <span data-ttu-id="9b401-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b401-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
