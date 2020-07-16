---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 56127a9a99c467fbf1951934f8b4658eadb59ca0
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896271"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="cb63b-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="cb63b-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="cb63b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb63b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb63b-105">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="cb63b-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="cb63b-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="cb63b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb63b-107">权限</span><span class="sxs-lookup"><span data-stu-id="cb63b-107">Permissions</span></span>

<span data-ttu-id="cb63b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb63b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb63b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb63b-110">Permission type</span></span>                        | <span data-ttu-id="cb63b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb63b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cb63b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb63b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb63b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb63b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cb63b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb63b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb63b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb63b-115">Not supported.</span></span>                           |
| <span data-ttu-id="cb63b-116">应用</span><span class="sxs-lookup"><span data-stu-id="cb63b-116">Application</span></span>                            | <span data-ttu-id="cb63b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb63b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="cb63b-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="cb63b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="cb63b-119">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="cb63b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="cb63b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb63b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cb63b-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="cb63b-121">Function parameters</span></span>

<span data-ttu-id="cb63b-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="cb63b-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cb63b-123">参数</span><span class="sxs-lookup"><span data-stu-id="cb63b-123">Parameter</span></span> | <span data-ttu-id="cb63b-124">类型</span><span class="sxs-lookup"><span data-stu-id="cb63b-124">Type</span></span>   | <span data-ttu-id="cb63b-125">说明</span><span class="sxs-lookup"><span data-stu-id="cb63b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cb63b-126">period</span><span class="sxs-lookup"><span data-stu-id="cb63b-126">period</span></span>    | <span data-ttu-id="cb63b-127">string</span><span class="sxs-lookup"><span data-stu-id="cb63b-127">string</span></span> | <span data-ttu-id="cb63b-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cb63b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cb63b-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cb63b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cb63b-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cb63b-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cb63b-131">必需。</span><span class="sxs-lookup"><span data-stu-id="cb63b-131">Required.</span></span> |

<span data-ttu-id="cb63b-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb63b-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cb63b-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="cb63b-133">The default output type is text/csv.</span></span> <span data-ttu-id="cb63b-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="cb63b-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb63b-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb63b-135">Request headers</span></span>

| <span data-ttu-id="cb63b-136">名称</span><span class="sxs-lookup"><span data-stu-id="cb63b-136">Name</span></span>          | <span data-ttu-id="cb63b-137">说明</span><span class="sxs-lookup"><span data-stu-id="cb63b-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb63b-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb63b-138">Authorization</span></span> | <span data-ttu-id="cb63b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb63b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cb63b-141">响应</span><span class="sxs-lookup"><span data-stu-id="cb63b-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cb63b-142">CSV</span><span class="sxs-lookup"><span data-stu-id="cb63b-142">CSV</span></span>

<span data-ttu-id="cb63b-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cb63b-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cb63b-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cb63b-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cb63b-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cb63b-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cb63b-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cb63b-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cb63b-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cb63b-147">Report Refresh Date</span></span>
- <span data-ttu-id="cb63b-148">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-148">Exchange Active</span></span>
- <span data-ttu-id="cb63b-149">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-149">Exchange Inactive</span></span>
- <span data-ttu-id="cb63b-150">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-150">OneDrive Active</span></span>
- <span data-ttu-id="cb63b-151">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-151">OneDrive Inactive</span></span>
- <span data-ttu-id="cb63b-152">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-152">SharePoint Active</span></span>
- <span data-ttu-id="cb63b-153">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-153">SharePoint Inactive</span></span>
- <span data-ttu-id="cb63b-154">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-154">Skype For Business Active</span></span>
- <span data-ttu-id="cb63b-155">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-155">Skype For Business Inactive</span></span>
- <span data-ttu-id="cb63b-156">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-156">Yammer Active</span></span>
- <span data-ttu-id="cb63b-157">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-157">Yammer Inactive</span></span>
- <span data-ttu-id="cb63b-158">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-158">Teams Active</span></span>
- <span data-ttu-id="cb63b-159">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-159">Teams Inactive</span></span>
- <span data-ttu-id="cb63b-160">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="cb63b-160">Office 365 Active</span></span>
- <span data-ttu-id="cb63b-161">Office 365 非活动</span><span class="sxs-lookup"><span data-stu-id="cb63b-161">Office 365 Inactive</span></span>
- <span data-ttu-id="cb63b-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="cb63b-162">Report Period</span></span>

<span data-ttu-id="cb63b-163">由世纪互联运营的 Microsoft Graph 中国不支持以下各列：</span><span class="sxs-lookup"><span data-stu-id="cb63b-163">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="cb63b-164">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-164">Yammer Active</span></span>
- <span data-ttu-id="cb63b-165">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-165">Yammer Inactive</span></span>
- <span data-ttu-id="cb63b-166">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-166">Teams Active</span></span>
- <span data-ttu-id="cb63b-167">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="cb63b-167">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="cb63b-168">JSON</span><span class="sxs-lookup"><span data-stu-id="cb63b-168">JSON</span></span>

<span data-ttu-id="cb63b-169">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="cb63b-169">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="cb63b-170">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="cb63b-170">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="cb63b-171">yammerActive</span><span class="sxs-lookup"><span data-stu-id="cb63b-171">yammerActive</span></span>
- <span data-ttu-id="cb63b-172">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="cb63b-172">yammerInactive</span></span>
- <span data-ttu-id="cb63b-173">teamsActive</span><span class="sxs-lookup"><span data-stu-id="cb63b-173">teamsActive</span></span>
- <span data-ttu-id="cb63b-174">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="cb63b-174">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="cb63b-175">示例</span><span class="sxs-lookup"><span data-stu-id="cb63b-175">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cb63b-176">CSV</span><span class="sxs-lookup"><span data-stu-id="cb63b-176">CSV</span></span>

<span data-ttu-id="cb63b-177">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="cb63b-177">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cb63b-178">请求</span><span class="sxs-lookup"><span data-stu-id="cb63b-178">Request</span></span>

<span data-ttu-id="cb63b-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb63b-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="cb63b-180">响应</span><span class="sxs-lookup"><span data-stu-id="cb63b-180">Response</span></span>

<span data-ttu-id="cb63b-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb63b-181">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cb63b-182">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cb63b-182">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="cb63b-183">JSON</span><span class="sxs-lookup"><span data-stu-id="cb63b-183">JSON</span></span> 

<span data-ttu-id="cb63b-184">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="cb63b-184">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cb63b-185">请求</span><span class="sxs-lookup"><span data-stu-id="cb63b-185">Request</span></span>

<span data-ttu-id="cb63b-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb63b-186">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="cb63b-187">响应</span><span class="sxs-lookup"><span data-stu-id="cb63b-187">Response</span></span>

<span data-ttu-id="cb63b-188">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb63b-188">The following is an example of the response.</span></span>

> <span data-ttu-id="cb63b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cb63b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "office365Active": 2791,
      "office365Inactive": 503,
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
