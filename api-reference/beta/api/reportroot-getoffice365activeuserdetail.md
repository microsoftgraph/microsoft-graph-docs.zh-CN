---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Normal
ms.openlocfilehash: dd727648c9b4b0000888a0d45d55737280fc11ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882381"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="e5386-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="e5386-103">reportRoot: getOffice365ActiveUserDetail</span></span>

> <span data-ttu-id="e5386-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5386-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5386-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5386-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5386-106">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e5386-106">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="e5386-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="e5386-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5386-108">权限</span><span class="sxs-lookup"><span data-stu-id="e5386-108">Permissions</span></span>

<span data-ttu-id="e5386-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5386-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5386-111">Permission type</span></span>                        | <span data-ttu-id="e5386-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5386-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e5386-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5386-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5386-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5386-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e5386-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5386-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5386-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5386-116">Not supported.</span></span>                           |
| <span data-ttu-id="e5386-117">应用</span><span class="sxs-lookup"><span data-stu-id="e5386-117">Application</span></span>                            | <span data-ttu-id="e5386-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5386-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e5386-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5386-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e5386-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="e5386-120">Function parameters</span></span>

<span data-ttu-id="e5386-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="e5386-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e5386-122">参数</span><span class="sxs-lookup"><span data-stu-id="e5386-122">Parameter</span></span> | <span data-ttu-id="e5386-123">类型</span><span class="sxs-lookup"><span data-stu-id="e5386-123">Type</span></span>   | <span data-ttu-id="e5386-124">说明</span><span class="sxs-lookup"><span data-stu-id="e5386-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e5386-125">period</span><span class="sxs-lookup"><span data-stu-id="e5386-125">period</span></span>    | <span data-ttu-id="e5386-126">string</span><span class="sxs-lookup"><span data-stu-id="e5386-126">string</span></span> | <span data-ttu-id="e5386-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e5386-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e5386-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e5386-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e5386-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e5386-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e5386-130">date</span><span class="sxs-lookup"><span data-stu-id="e5386-130">date</span></span>      | <span data-ttu-id="e5386-131">Date</span><span class="sxs-lookup"><span data-stu-id="e5386-131">Date</span></span>   | <span data-ttu-id="e5386-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="e5386-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e5386-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="e5386-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e5386-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="e5386-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e5386-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="e5386-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e5386-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5386-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e5386-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="e5386-137">The default output type is text/csv.</span></span> <span data-ttu-id="e5386-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="e5386-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5386-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5386-139">Request headers</span></span>

| <span data-ttu-id="e5386-140">名称</span><span class="sxs-lookup"><span data-stu-id="e5386-140">Name</span></span>          | <span data-ttu-id="e5386-141">说明</span><span class="sxs-lookup"><span data-stu-id="e5386-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e5386-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5386-142">Authorization</span></span> | <span data-ttu-id="e5386-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5386-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e5386-145">响应</span><span class="sxs-lookup"><span data-stu-id="e5386-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e5386-146">CSV</span><span class="sxs-lookup"><span data-stu-id="e5386-146">CSV</span></span>

<span data-ttu-id="e5386-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e5386-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e5386-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e5386-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e5386-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e5386-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e5386-150">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="e5386-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="e5386-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e5386-151">Report Refresh Date</span></span>
- <span data-ttu-id="e5386-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e5386-152">User Principal Name</span></span>
- <span data-ttu-id="e5386-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="e5386-153">Display Name</span></span>
- <span data-ttu-id="e5386-154">已删除</span><span class="sxs-lookup"><span data-stu-id="e5386-154">Is Deleted</span></span>
- <span data-ttu-id="e5386-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="e5386-155">Deleted Date</span></span>
- <span data-ttu-id="e5386-156">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-156">Has Exchange License</span></span>
- <span data-ttu-id="e5386-157">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-157">Has OneDrive License</span></span>
- <span data-ttu-id="e5386-158">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-158">Has SharePoint License</span></span>
- <span data-ttu-id="e5386-159">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-159">Has Skype For Business License</span></span>
- <span data-ttu-id="e5386-160">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-160">Has Yammer License</span></span>
- <span data-ttu-id="e5386-161">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-161">Has Teams License</span></span>
- <span data-ttu-id="e5386-162">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="e5386-163">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="e5386-164">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="e5386-165">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="e5386-166">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="e5386-167">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="e5386-168">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="e5386-169">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="e5386-170">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="e5386-171">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="e5386-172">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="e5386-173">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-173">Teams License Assign Date</span></span>
- <span data-ttu-id="e5386-174">分配的产品</span><span class="sxs-lookup"><span data-stu-id="e5386-174">Assigned Products</span></span>

<span data-ttu-id="e5386-175">在 Microsoft Graph 中国由 21Vianet 不支持下列：</span><span class="sxs-lookup"><span data-stu-id="e5386-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e5386-176">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-176">Has Yammer License</span></span>
- <span data-ttu-id="e5386-177">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="e5386-177">Has Teams License</span></span>
- <span data-ttu-id="e5386-178">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="e5386-179">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e5386-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="e5386-180">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="e5386-181">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="e5386-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="e5386-182">JSON</span><span class="sxs-lookup"><span data-stu-id="e5386-182">JSON</span></span>

<span data-ttu-id="e5386-183">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e5386-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="e5386-184">在 Microsoft Graph 中国由 21Vianet 不支持**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="e5386-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e5386-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="e5386-185">hasYammerLicense</span></span>
- <span data-ttu-id="e5386-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="e5386-186">hasTeamsLicense</span></span>
- <span data-ttu-id="e5386-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e5386-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="e5386-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e5386-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="e5386-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="e5386-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="e5386-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="e5386-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="e5386-191">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="e5386-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e5386-192">示例</span><span class="sxs-lookup"><span data-stu-id="e5386-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e5386-193">CSV</span><span class="sxs-lookup"><span data-stu-id="e5386-193">CSV</span></span>

<span data-ttu-id="e5386-194">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="e5386-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e5386-195">请求</span><span class="sxs-lookup"><span data-stu-id="e5386-195">Request</span></span>

<span data-ttu-id="e5386-196">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5386-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e5386-197">响应</span><span class="sxs-lookup"><span data-stu-id="e5386-197">Response</span></span>

<span data-ttu-id="e5386-198">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5386-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e5386-199">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e5386-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e5386-200">JSON</span><span class="sxs-lookup"><span data-stu-id="e5386-200">JSON</span></span>

<span data-ttu-id="e5386-201">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e5386-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e5386-202">请求</span><span class="sxs-lookup"><span data-stu-id="e5386-202">Request</span></span>

<span data-ttu-id="e5386-203">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5386-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e5386-204">响应</span><span class="sxs-lookup"><span data-stu-id="e5386-204">Response</span></span>

<span data-ttu-id="e5386-205">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5386-205">The following is an example of the response.</span></span>

> <span data-ttu-id="e5386-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5386-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
