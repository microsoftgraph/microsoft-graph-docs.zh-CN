---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 55549d2872232f292eeaabff550b1612ad2d1657
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577191"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="7032f-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="7032f-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7032f-104">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7032f-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="7032f-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="7032f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="7032f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7032f-106">Permissions</span></span>

<span data-ttu-id="7032f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7032f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7032f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7032f-109">Permission type</span></span>                        | <span data-ttu-id="7032f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7032f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7032f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7032f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7032f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7032f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7032f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7032f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7032f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7032f-114">Not supported.</span></span>                           |
| <span data-ttu-id="7032f-115">应用</span><span class="sxs-lookup"><span data-stu-id="7032f-115">Application</span></span>                            | <span data-ttu-id="7032f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7032f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7032f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7032f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7032f-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="7032f-118">Function parameters</span></span>

<span data-ttu-id="7032f-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="7032f-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7032f-120">参数</span><span class="sxs-lookup"><span data-stu-id="7032f-120">Parameter</span></span> | <span data-ttu-id="7032f-121">类型</span><span class="sxs-lookup"><span data-stu-id="7032f-121">Type</span></span>   | <span data-ttu-id="7032f-122">说明</span><span class="sxs-lookup"><span data-stu-id="7032f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7032f-123">period</span><span class="sxs-lookup"><span data-stu-id="7032f-123">period</span></span>    | <span data-ttu-id="7032f-124">string</span><span class="sxs-lookup"><span data-stu-id="7032f-124">string</span></span> | <span data-ttu-id="7032f-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7032f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7032f-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7032f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7032f-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7032f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7032f-128">date</span><span class="sxs-lookup"><span data-stu-id="7032f-128">date</span></span>      | <span data-ttu-id="7032f-129">Date</span><span class="sxs-lookup"><span data-stu-id="7032f-129">Date</span></span>   | <span data-ttu-id="7032f-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="7032f-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7032f-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="7032f-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7032f-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="7032f-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7032f-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="7032f-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7032f-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7032f-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7032f-135">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="7032f-135">The default output type is text/csv.</span></span> <span data-ttu-id="7032f-136">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="7032f-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7032f-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="7032f-137">Request headers</span></span>

| <span data-ttu-id="7032f-138">名称</span><span class="sxs-lookup"><span data-stu-id="7032f-138">Name</span></span>          | <span data-ttu-id="7032f-139">说明</span><span class="sxs-lookup"><span data-stu-id="7032f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7032f-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="7032f-140">Authorization</span></span> | <span data-ttu-id="7032f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7032f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7032f-143">响应</span><span class="sxs-lookup"><span data-stu-id="7032f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7032f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7032f-144">CSV</span></span>

<span data-ttu-id="7032f-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7032f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7032f-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7032f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7032f-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7032f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7032f-148">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="7032f-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="7032f-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7032f-149">Report Refresh Date</span></span>
- <span data-ttu-id="7032f-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="7032f-150">User Principal Name</span></span>
- <span data-ttu-id="7032f-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="7032f-151">Display Name</span></span>
- <span data-ttu-id="7032f-152">已删除</span><span class="sxs-lookup"><span data-stu-id="7032f-152">Is Deleted</span></span>
- <span data-ttu-id="7032f-153">删除日期</span><span class="sxs-lookup"><span data-stu-id="7032f-153">Deleted Date</span></span>
- <span data-ttu-id="7032f-154">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-154">Has Exchange License</span></span>
- <span data-ttu-id="7032f-155">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-155">Has OneDrive License</span></span>
- <span data-ttu-id="7032f-156">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-156">Has SharePoint License</span></span>
- <span data-ttu-id="7032f-157">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-157">Has Skype For Business License</span></span>
- <span data-ttu-id="7032f-158">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-158">Has Yammer License</span></span>
- <span data-ttu-id="7032f-159">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-159">Has Teams License</span></span>
- <span data-ttu-id="7032f-160">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="7032f-161">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="7032f-162">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="7032f-163">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="7032f-164">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="7032f-165">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="7032f-166">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="7032f-167">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="7032f-168">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="7032f-169">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="7032f-170">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="7032f-171">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-171">Teams License Assign Date</span></span>
- <span data-ttu-id="7032f-172">分配的产品</span><span class="sxs-lookup"><span data-stu-id="7032f-172">Assigned Products</span></span>

<span data-ttu-id="7032f-173">在 Microsoft Graph 中国由 21Vianet 不支持下列：</span><span class="sxs-lookup"><span data-stu-id="7032f-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="7032f-174">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-174">Has Yammer License</span></span>
- <span data-ttu-id="7032f-175">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="7032f-175">Has Teams License</span></span>
- <span data-ttu-id="7032f-176">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="7032f-177">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="7032f-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="7032f-178">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="7032f-179">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="7032f-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="7032f-180">JSON</span><span class="sxs-lookup"><span data-stu-id="7032f-180">JSON</span></span>

<span data-ttu-id="7032f-181">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7032f-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7032f-182">在 Microsoft Graph 中国由 21Vianet 不支持**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="7032f-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="7032f-183">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="7032f-183">hasYammerLicense</span></span>
- <span data-ttu-id="7032f-184">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="7032f-184">hasTeamsLicense</span></span>
- <span data-ttu-id="7032f-185">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7032f-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="7032f-186">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7032f-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="7032f-187">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="7032f-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="7032f-188">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="7032f-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="7032f-189">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="7032f-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7032f-190">示例</span><span class="sxs-lookup"><span data-stu-id="7032f-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7032f-191">CSV</span><span class="sxs-lookup"><span data-stu-id="7032f-191">CSV</span></span>

<span data-ttu-id="7032f-192">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="7032f-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7032f-193">请求</span><span class="sxs-lookup"><span data-stu-id="7032f-193">Request</span></span>

<span data-ttu-id="7032f-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7032f-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7032f-195">响应</span><span class="sxs-lookup"><span data-stu-id="7032f-195">Response</span></span>

<span data-ttu-id="7032f-196">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7032f-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7032f-197">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7032f-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a><span data-ttu-id="7032f-198">JSON</span><span class="sxs-lookup"><span data-stu-id="7032f-198">JSON</span></span>

<span data-ttu-id="7032f-199">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7032f-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7032f-200">请求</span><span class="sxs-lookup"><span data-stu-id="7032f-200">Request</span></span>

<span data-ttu-id="7032f-201">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7032f-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7032f-202">响应</span><span class="sxs-lookup"><span data-stu-id="7032f-202">Response</span></span>

<span data-ttu-id="7032f-203">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7032f-203">The following is an example of the response.</span></span>

> <span data-ttu-id="7032f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7032f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
