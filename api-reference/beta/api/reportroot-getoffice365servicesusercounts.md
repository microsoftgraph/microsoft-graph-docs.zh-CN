---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
ms.openlocfilehash: 9f331852c5ba47643e11ea6cfa86167669557aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044029"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="ef163-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="ef163-103">reportRoot: getOffice365ServicesUserCounts</span></span>

> <span data-ttu-id="ef163-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef163-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef163-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef163-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef163-106">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="ef163-106">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="ef163-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="ef163-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef163-108">权限</span><span class="sxs-lookup"><span data-stu-id="ef163-108">Permissions</span></span>

<span data-ttu-id="ef163-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef163-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef163-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef163-111">Permission type</span></span>                        | <span data-ttu-id="ef163-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef163-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ef163-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef163-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef163-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef163-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ef163-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef163-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef163-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef163-116">Not supported.</span></span>                           |
| <span data-ttu-id="ef163-117">应用</span><span class="sxs-lookup"><span data-stu-id="ef163-117">Application</span></span>                            | <span data-ttu-id="ef163-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef163-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ef163-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef163-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ef163-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="ef163-120">Function parameters</span></span>

<span data-ttu-id="ef163-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ef163-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ef163-122">参数</span><span class="sxs-lookup"><span data-stu-id="ef163-122">Parameter</span></span> | <span data-ttu-id="ef163-123">类型</span><span class="sxs-lookup"><span data-stu-id="ef163-123">Type</span></span>   | <span data-ttu-id="ef163-124">说明</span><span class="sxs-lookup"><span data-stu-id="ef163-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ef163-125">period</span><span class="sxs-lookup"><span data-stu-id="ef163-125">period</span></span>    | <span data-ttu-id="ef163-126">string</span><span class="sxs-lookup"><span data-stu-id="ef163-126">string</span></span> | <span data-ttu-id="ef163-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ef163-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ef163-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ef163-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ef163-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ef163-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ef163-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ef163-130">Required.</span></span> |

<span data-ttu-id="ef163-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ef163-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ef163-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="ef163-132">The default output type is text/csv.</span></span> <span data-ttu-id="ef163-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="ef163-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef163-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef163-134">Request headers</span></span>

| <span data-ttu-id="ef163-135">名称</span><span class="sxs-lookup"><span data-stu-id="ef163-135">Name</span></span>          | <span data-ttu-id="ef163-136">说明</span><span class="sxs-lookup"><span data-stu-id="ef163-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ef163-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef163-137">Authorization</span></span> | <span data-ttu-id="ef163-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef163-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ef163-140">响应</span><span class="sxs-lookup"><span data-stu-id="ef163-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ef163-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ef163-141">CSV</span></span>

<span data-ttu-id="ef163-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ef163-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ef163-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ef163-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ef163-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ef163-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ef163-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ef163-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ef163-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ef163-146">Report Refresh Date</span></span>
- <span data-ttu-id="ef163-147">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-147">Exchange Active</span></span>
- <span data-ttu-id="ef163-148">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-148">Exchange Inactive</span></span>
- <span data-ttu-id="ef163-149">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-149">OneDrive Active</span></span>
- <span data-ttu-id="ef163-150">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-150">OneDrive Inactive</span></span>
- <span data-ttu-id="ef163-151">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-151">SharePoint Active</span></span>
- <span data-ttu-id="ef163-152">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-152">SharePoint Inactive</span></span>
- <span data-ttu-id="ef163-153">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-153">Skype For Business Active</span></span>
- <span data-ttu-id="ef163-154">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="ef163-155">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-155">Yammer Active</span></span>
- <span data-ttu-id="ef163-156">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-156">Yammer Inactive</span></span>
- <span data-ttu-id="ef163-157">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-157">Teams Active</span></span>
- <span data-ttu-id="ef163-158">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-158">Teams Inactive</span></span>
- <span data-ttu-id="ef163-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="ef163-159">Report Period</span></span>

<span data-ttu-id="ef163-160">在 Microsoft Graph 中国由 21Vianet 不支持下列：</span><span class="sxs-lookup"><span data-stu-id="ef163-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ef163-161">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-161">Yammer Active</span></span>
- <span data-ttu-id="ef163-162">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-162">Yammer Inactive</span></span>
- <span data-ttu-id="ef163-163">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-163">Teams Active</span></span>
- <span data-ttu-id="ef163-164">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="ef163-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="ef163-165">JSON</span><span class="sxs-lookup"><span data-stu-id="ef163-165">JSON</span></span>

<span data-ttu-id="ef163-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="ef163-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="ef163-167">在 Microsoft Graph 中国由 21Vianet 不支持**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="ef163-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ef163-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="ef163-168">yammerActive</span></span>
- <span data-ttu-id="ef163-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="ef163-169">yammerInactive</span></span>
- <span data-ttu-id="ef163-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="ef163-170">teamsActive</span></span>
- <span data-ttu-id="ef163-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="ef163-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="ef163-172">示例</span><span class="sxs-lookup"><span data-stu-id="ef163-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ef163-173">CSV</span><span class="sxs-lookup"><span data-stu-id="ef163-173">CSV</span></span>

<span data-ttu-id="ef163-174">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="ef163-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ef163-175">请求</span><span class="sxs-lookup"><span data-stu-id="ef163-175">Request</span></span>

<span data-ttu-id="ef163-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ef163-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ef163-177">响应</span><span class="sxs-lookup"><span data-stu-id="ef163-177">Response</span></span>

<span data-ttu-id="ef163-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ef163-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ef163-179">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ef163-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="ef163-180">JSON</span><span class="sxs-lookup"><span data-stu-id="ef163-180">JSON</span></span> 

<span data-ttu-id="ef163-181">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="ef163-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ef163-182">请求</span><span class="sxs-lookup"><span data-stu-id="ef163-182">Request</span></span>

<span data-ttu-id="ef163-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ef163-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ef163-184">响应</span><span class="sxs-lookup"><span data-stu-id="ef163-184">Response</span></span>

<span data-ttu-id="ef163-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ef163-185">The following is an example of the response.</span></span>

> <span data-ttu-id="ef163-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ef163-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "reportPeriod": "7"
    }
  ]
}
```
