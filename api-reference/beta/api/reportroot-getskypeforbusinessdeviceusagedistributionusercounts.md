---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: bf5bbcfb92a840157222975f50684bea514a379a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517755"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="1a48b-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1a48b-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a48b-105">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="1a48b-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="1a48b-106">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="1a48b-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="1a48b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="1a48b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a48b-108">权限</span><span class="sxs-lookup"><span data-stu-id="1a48b-108">Permissions</span></span>

<span data-ttu-id="1a48b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a48b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a48b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a48b-111">Permission type</span></span>                        | <span data-ttu-id="1a48b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a48b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1a48b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a48b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a48b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a48b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1a48b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a48b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a48b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a48b-116">Not supported.</span></span>                           |
| <span data-ttu-id="1a48b-117">应用</span><span class="sxs-lookup"><span data-stu-id="1a48b-117">Application</span></span>                            | <span data-ttu-id="1a48b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a48b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1a48b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a48b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1a48b-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="1a48b-120">Function parameters</span></span>

<span data-ttu-id="1a48b-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1a48b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1a48b-122">参数</span><span class="sxs-lookup"><span data-stu-id="1a48b-122">Parameter</span></span> | <span data-ttu-id="1a48b-123">类型</span><span class="sxs-lookup"><span data-stu-id="1a48b-123">Type</span></span>   | <span data-ttu-id="1a48b-124">说明</span><span class="sxs-lookup"><span data-stu-id="1a48b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1a48b-125">period</span><span class="sxs-lookup"><span data-stu-id="1a48b-125">period</span></span>    | <span data-ttu-id="1a48b-126">string</span><span class="sxs-lookup"><span data-stu-id="1a48b-126">string</span></span> | <span data-ttu-id="1a48b-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1a48b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1a48b-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1a48b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1a48b-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1a48b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1a48b-130">必需。</span><span class="sxs-lookup"><span data-stu-id="1a48b-130">Required.</span></span> |

<span data-ttu-id="1a48b-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1a48b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1a48b-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="1a48b-132">The default output type is text/csv.</span></span> <span data-ttu-id="1a48b-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="1a48b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a48b-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a48b-134">Request headers</span></span>

| <span data-ttu-id="1a48b-135">名称</span><span class="sxs-lookup"><span data-stu-id="1a48b-135">Name</span></span>          | <span data-ttu-id="1a48b-136">说明</span><span class="sxs-lookup"><span data-stu-id="1a48b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1a48b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a48b-137">Authorization</span></span> | <span data-ttu-id="1a48b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a48b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1a48b-140">响应</span><span class="sxs-lookup"><span data-stu-id="1a48b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1a48b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1a48b-141">CSV</span></span>

<span data-ttu-id="1a48b-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1a48b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1a48b-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1a48b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1a48b-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1a48b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1a48b-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1a48b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1a48b-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1a48b-146">Report Refresh Date</span></span>
- <span data-ttu-id="1a48b-147">Windows</span><span class="sxs-lookup"><span data-stu-id="1a48b-147">Windows</span></span>
- <span data-ttu-id="1a48b-148">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="1a48b-148">Windows Phone</span></span>
- <span data-ttu-id="1a48b-149">Android 手机</span><span class="sxs-lookup"><span data-stu-id="1a48b-149">Android Phone</span></span>
- <span data-ttu-id="1a48b-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="1a48b-150">iPhone</span></span>
- <span data-ttu-id="1a48b-151">iPad</span><span class="sxs-lookup"><span data-stu-id="1a48b-151">iPad</span></span>
- <span data-ttu-id="1a48b-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="1a48b-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1a48b-153">JSON</span><span class="sxs-lookup"><span data-stu-id="1a48b-153">JSON</span></span>

<span data-ttu-id="1a48b-154">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1a48b-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a48b-155">示例</span><span class="sxs-lookup"><span data-stu-id="1a48b-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1a48b-156">CSV</span><span class="sxs-lookup"><span data-stu-id="1a48b-156">CSV</span></span>

<span data-ttu-id="1a48b-157">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="1a48b-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1a48b-158">请求</span><span class="sxs-lookup"><span data-stu-id="1a48b-158">Request</span></span>

<span data-ttu-id="1a48b-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a48b-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1a48b-160">响应</span><span class="sxs-lookup"><span data-stu-id="1a48b-160">Response</span></span>

<span data-ttu-id="1a48b-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a48b-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1a48b-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1a48b-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="1a48b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="1a48b-163">JSON</span></span>

<span data-ttu-id="1a48b-164">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1a48b-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1a48b-165">请求</span><span class="sxs-lookup"><span data-stu-id="1a48b-165">Request</span></span>

<span data-ttu-id="1a48b-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a48b-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1a48b-167">响应</span><span class="sxs-lookup"><span data-stu-id="1a48b-167">Response</span></span>

<span data-ttu-id="1a48b-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a48b-168">The following is an example of the response.</span></span>

> <span data-ttu-id="1a48b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1a48b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
