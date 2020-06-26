---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: 在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 60bf9b1d0ee47bb35d6abbb21f3f813442536f70
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896173"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="5efda-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5efda-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="5efda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5efda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5efda-105">在选定的时间段内按设备类型获取 Microsoft Teams 唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="5efda-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="5efda-106">权限</span><span class="sxs-lookup"><span data-stu-id="5efda-106">Permissions</span></span>

<span data-ttu-id="5efda-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5efda-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5efda-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5efda-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5efda-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5efda-109">Permission type</span></span>                        | <span data-ttu-id="5efda-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5efda-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5efda-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5efda-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5efda-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5efda-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5efda-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5efda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5efda-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5efda-114">Not supported.</span></span>                           |
| <span data-ttu-id="5efda-115">应用</span><span class="sxs-lookup"><span data-stu-id="5efda-115">Application</span></span>                            | <span data-ttu-id="5efda-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5efda-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5efda-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5efda-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5efda-118">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="5efda-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5efda-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5efda-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="5efda-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="5efda-120">Function parameters</span></span>

<span data-ttu-id="5efda-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5efda-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5efda-122">参数</span><span class="sxs-lookup"><span data-stu-id="5efda-122">Parameter</span></span> | <span data-ttu-id="5efda-123">类型</span><span class="sxs-lookup"><span data-stu-id="5efda-123">Type</span></span>   | <span data-ttu-id="5efda-124">说明</span><span class="sxs-lookup"><span data-stu-id="5efda-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5efda-125">period</span><span class="sxs-lookup"><span data-stu-id="5efda-125">period</span></span>    | <span data-ttu-id="5efda-126">string</span><span class="sxs-lookup"><span data-stu-id="5efda-126">string</span></span> | <span data-ttu-id="5efda-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5efda-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5efda-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5efda-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5efda-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5efda-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5efda-130">必需。</span><span class="sxs-lookup"><span data-stu-id="5efda-130">Required.</span></span> |

<span data-ttu-id="5efda-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5efda-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5efda-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="5efda-132">The default output type is text/csv.</span></span> <span data-ttu-id="5efda-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="5efda-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5efda-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="5efda-134">Request headers</span></span>

| <span data-ttu-id="5efda-135">名称</span><span class="sxs-lookup"><span data-stu-id="5efda-135">Name</span></span>          | <span data-ttu-id="5efda-136">说明</span><span class="sxs-lookup"><span data-stu-id="5efda-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5efda-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5efda-137">Authorization</span></span> | <span data-ttu-id="5efda-138">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5efda-138">Bearer {token}.</span></span> <span data-ttu-id="5efda-139">Required.</span><span class="sxs-lookup"><span data-stu-id="5efda-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5efda-140">响应</span><span class="sxs-lookup"><span data-stu-id="5efda-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5efda-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5efda-141">CSV</span></span>

<span data-ttu-id="5efda-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5efda-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5efda-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5efda-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5efda-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5efda-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5efda-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5efda-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5efda-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5efda-146">Report Refresh Date</span></span>
- <span data-ttu-id="5efda-147">Web</span><span class="sxs-lookup"><span data-stu-id="5efda-147">Web</span></span>
- <span data-ttu-id="5efda-148">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="5efda-148">Windows Phone</span></span>
- <span data-ttu-id="5efda-149">Android 手机</span><span class="sxs-lookup"><span data-stu-id="5efda-149">Android Phone</span></span>
- <span data-ttu-id="5efda-150">iOS</span><span class="sxs-lookup"><span data-stu-id="5efda-150">iOS</span></span>
- <span data-ttu-id="5efda-151">Mac</span><span class="sxs-lookup"><span data-stu-id="5efda-151">Mac</span></span>
- <span data-ttu-id="5efda-152">Windows</span><span class="sxs-lookup"><span data-stu-id="5efda-152">Windows</span></span>
- <span data-ttu-id="5efda-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="5efda-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5efda-154">JSON</span><span class="sxs-lookup"><span data-stu-id="5efda-154">JSON</span></span>

<span data-ttu-id="5efda-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="5efda-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5efda-156">示例</span><span class="sxs-lookup"><span data-stu-id="5efda-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5efda-157">CSV</span><span class="sxs-lookup"><span data-stu-id="5efda-157">CSV</span></span>

<span data-ttu-id="5efda-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="5efda-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5efda-159">请求</span><span class="sxs-lookup"><span data-stu-id="5efda-159">Request</span></span>

<span data-ttu-id="5efda-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5efda-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5efda-161">响应</span><span class="sxs-lookup"><span data-stu-id="5efda-161">Response</span></span>

<span data-ttu-id="5efda-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5efda-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5efda-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5efda-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5efda-164">JSON</span><span class="sxs-lookup"><span data-stu-id="5efda-164">JSON</span></span>

<span data-ttu-id="5efda-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="5efda-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5efda-166">请求</span><span class="sxs-lookup"><span data-stu-id="5efda-166">Request</span></span>

<span data-ttu-id="5efda-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5efda-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5efda-168">响应</span><span class="sxs-lookup"><span data-stu-id="5efda-168">Response</span></span>

<span data-ttu-id="5efda-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5efda-169">The following is an example of the response.</span></span>

> <span data-ttu-id="5efda-170">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5efda-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5efda-171">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5efda-171">All the properties will be returned from an actual call.</span></span>

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
