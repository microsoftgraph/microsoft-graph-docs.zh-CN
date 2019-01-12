---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: 获取组织中使用唯一设备的用户数。 报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ccae9dd215c74fee6ebc2703d848bc563ff1b0c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948042"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="7433f-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7433f-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="7433f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7433f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7433f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7433f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7433f-107">获取组织中使用唯一设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="7433f-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="7433f-108">报表会显示每台设备的用户数，包括 Windows、Windows 手机、Android 手机、iPhone 和 iPad。</span><span class="sxs-lookup"><span data-stu-id="7433f-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="7433f-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="7433f-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="7433f-110">权限</span><span class="sxs-lookup"><span data-stu-id="7433f-110">Permissions</span></span>

<span data-ttu-id="7433f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7433f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7433f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7433f-113">Permission type</span></span>                        | <span data-ttu-id="7433f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7433f-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7433f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7433f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7433f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7433f-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7433f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7433f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7433f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7433f-118">Not supported.</span></span>                           |
| <span data-ttu-id="7433f-119">应用</span><span class="sxs-lookup"><span data-stu-id="7433f-119">Application</span></span>                            | <span data-ttu-id="7433f-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7433f-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7433f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7433f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7433f-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="7433f-122">Function parameters</span></span>

<span data-ttu-id="7433f-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7433f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7433f-124">参数</span><span class="sxs-lookup"><span data-stu-id="7433f-124">Parameter</span></span> | <span data-ttu-id="7433f-125">类型</span><span class="sxs-lookup"><span data-stu-id="7433f-125">Type</span></span>   | <span data-ttu-id="7433f-126">说明</span><span class="sxs-lookup"><span data-stu-id="7433f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7433f-127">period</span><span class="sxs-lookup"><span data-stu-id="7433f-127">period</span></span>    | <span data-ttu-id="7433f-128">string</span><span class="sxs-lookup"><span data-stu-id="7433f-128">string</span></span> | <span data-ttu-id="7433f-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7433f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7433f-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7433f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7433f-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7433f-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7433f-132">必需。</span><span class="sxs-lookup"><span data-stu-id="7433f-132">Required.</span></span> |

<span data-ttu-id="7433f-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7433f-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7433f-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="7433f-134">The default output type is text/csv.</span></span> <span data-ttu-id="7433f-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="7433f-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7433f-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="7433f-136">Request headers</span></span>

| <span data-ttu-id="7433f-137">名称</span><span class="sxs-lookup"><span data-stu-id="7433f-137">Name</span></span>          | <span data-ttu-id="7433f-138">说明</span><span class="sxs-lookup"><span data-stu-id="7433f-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7433f-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="7433f-139">Authorization</span></span> | <span data-ttu-id="7433f-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7433f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7433f-142">响应</span><span class="sxs-lookup"><span data-stu-id="7433f-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7433f-143">CSV</span><span class="sxs-lookup"><span data-stu-id="7433f-143">CSV</span></span>

<span data-ttu-id="7433f-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7433f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7433f-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7433f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7433f-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7433f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7433f-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7433f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7433f-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7433f-148">Report Refresh Date</span></span>
- <span data-ttu-id="7433f-149">Windows</span><span class="sxs-lookup"><span data-stu-id="7433f-149">Windows</span></span>
- <span data-ttu-id="7433f-150">Windows 手机</span><span class="sxs-lookup"><span data-stu-id="7433f-150">Windows Phone</span></span>
- <span data-ttu-id="7433f-151">Android 手机</span><span class="sxs-lookup"><span data-stu-id="7433f-151">Android Phone</span></span>
- <span data-ttu-id="7433f-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="7433f-152">iPhone</span></span>
- <span data-ttu-id="7433f-153">iPad</span><span class="sxs-lookup"><span data-stu-id="7433f-153">iPad</span></span>
- <span data-ttu-id="7433f-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="7433f-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7433f-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7433f-155">JSON</span></span>

<span data-ttu-id="7433f-156">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7433f-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7433f-157">示例</span><span class="sxs-lookup"><span data-stu-id="7433f-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7433f-158">CSV</span><span class="sxs-lookup"><span data-stu-id="7433f-158">CSV</span></span>

<span data-ttu-id="7433f-159">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="7433f-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7433f-160">请求</span><span class="sxs-lookup"><span data-stu-id="7433f-160">Request</span></span>

<span data-ttu-id="7433f-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7433f-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7433f-162">响应</span><span class="sxs-lookup"><span data-stu-id="7433f-162">Response</span></span>

<span data-ttu-id="7433f-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7433f-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7433f-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7433f-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7433f-165">JSON</span><span class="sxs-lookup"><span data-stu-id="7433f-165">JSON</span></span>

<span data-ttu-id="7433f-166">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7433f-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7433f-167">请求</span><span class="sxs-lookup"><span data-stu-id="7433f-167">Request</span></span>

<span data-ttu-id="7433f-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7433f-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7433f-169">响应</span><span class="sxs-lookup"><span data-stu-id="7433f-169">Response</span></span>

<span data-ttu-id="7433f-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7433f-170">The following is an example of the response.</span></span>

> <span data-ttu-id="7433f-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7433f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
