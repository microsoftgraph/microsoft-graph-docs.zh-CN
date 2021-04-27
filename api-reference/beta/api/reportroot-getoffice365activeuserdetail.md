---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取有关 Microsoft 365 活动用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ebb4c09758fec323e015cf2efbda6b04f1e8cf5a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050904"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="76888-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="76888-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="76888-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76888-105">获取有关 Microsoft 365 活动用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="76888-105">Get details about Microsoft 365 active users.</span></span>

> <span data-ttu-id="76888-106">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="76888-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="76888-107">权限</span><span class="sxs-lookup"><span data-stu-id="76888-107">Permissions</span></span>

<span data-ttu-id="76888-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76888-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="76888-110">Permission type</span></span>                        | <span data-ttu-id="76888-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76888-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="76888-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76888-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76888-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76888-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="76888-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76888-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76888-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76888-115">Not supported.</span></span>                           |
| <span data-ttu-id="76888-116">应用</span><span class="sxs-lookup"><span data-stu-id="76888-116">Application</span></span>                            | <span data-ttu-id="76888-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76888-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="76888-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="76888-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="76888-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="76888-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="76888-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76888-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="76888-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="76888-121">Function parameters</span></span>

<span data-ttu-id="76888-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="76888-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="76888-123">参数</span><span class="sxs-lookup"><span data-stu-id="76888-123">Parameter</span></span> | <span data-ttu-id="76888-124">类型</span><span class="sxs-lookup"><span data-stu-id="76888-124">Type</span></span>   | <span data-ttu-id="76888-125">说明</span><span class="sxs-lookup"><span data-stu-id="76888-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="76888-126">period</span><span class="sxs-lookup"><span data-stu-id="76888-126">period</span></span>    | <span data-ttu-id="76888-127">string</span><span class="sxs-lookup"><span data-stu-id="76888-127">string</span></span> | <span data-ttu-id="76888-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="76888-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="76888-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="76888-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="76888-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="76888-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="76888-131">date</span><span class="sxs-lookup"><span data-stu-id="76888-131">date</span></span>      | <span data-ttu-id="76888-132">Date</span><span class="sxs-lookup"><span data-stu-id="76888-132">Date</span></span>   | <span data-ttu-id="76888-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="76888-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="76888-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="76888-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="76888-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="76888-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="76888-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="76888-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="76888-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76888-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="76888-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="76888-138">The default output type is text/csv.</span></span> <span data-ttu-id="76888-139">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="76888-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76888-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="76888-140">Request headers</span></span>

| <span data-ttu-id="76888-141">名称</span><span class="sxs-lookup"><span data-stu-id="76888-141">Name</span></span>          | <span data-ttu-id="76888-142">说明</span><span class="sxs-lookup"><span data-stu-id="76888-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="76888-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="76888-143">Authorization</span></span> | <span data-ttu-id="76888-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76888-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="76888-146">响应</span><span class="sxs-lookup"><span data-stu-id="76888-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="76888-147">CSV</span><span class="sxs-lookup"><span data-stu-id="76888-147">CSV</span></span>

<span data-ttu-id="76888-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="76888-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="76888-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="76888-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="76888-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="76888-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="76888-151">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="76888-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="76888-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="76888-152">Report Refresh Date</span></span>
- <span data-ttu-id="76888-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="76888-153">User Principal Name</span></span>
- <span data-ttu-id="76888-154">显示名称</span><span class="sxs-lookup"><span data-stu-id="76888-154">Display Name</span></span>
- <span data-ttu-id="76888-155">已删除</span><span class="sxs-lookup"><span data-stu-id="76888-155">Is Deleted</span></span>
- <span data-ttu-id="76888-156">删除日期</span><span class="sxs-lookup"><span data-stu-id="76888-156">Deleted Date</span></span>
- <span data-ttu-id="76888-157">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-157">Has Exchange License</span></span>
- <span data-ttu-id="76888-158">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-158">Has OneDrive License</span></span>
- <span data-ttu-id="76888-159">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-159">Has SharePoint License</span></span>
- <span data-ttu-id="76888-160">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-160">Has Skype For Business License</span></span>
- <span data-ttu-id="76888-161">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-161">Has Yammer License</span></span>
- <span data-ttu-id="76888-162">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-162">Has Teams License</span></span>
- <span data-ttu-id="76888-163">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-163">Exchange Last Activity Date</span></span>
- <span data-ttu-id="76888-164">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-164">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="76888-165">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-165">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="76888-166">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-166">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="76888-167">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-167">Yammer Last Activity Date</span></span>
- <span data-ttu-id="76888-168">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-168">Teams Last Activity Date</span></span>
- <span data-ttu-id="76888-169">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-169">Exchange License Assign Date</span></span>
- <span data-ttu-id="76888-170">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-170">OneDrive License Assign Date</span></span>
- <span data-ttu-id="76888-171">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-171">SharePoint License Assign Date</span></span>
- <span data-ttu-id="76888-172">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-172">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="76888-173">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-173">Yammer License Assign Date</span></span>
- <span data-ttu-id="76888-174">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-174">Teams License Assign Date</span></span>
- <span data-ttu-id="76888-175">分配的产品</span><span class="sxs-lookup"><span data-stu-id="76888-175">Assigned Products</span></span>

<span data-ttu-id="76888-176">由世纪Graph运营的 Microsoft Graph不支持以下列：</span><span class="sxs-lookup"><span data-stu-id="76888-176">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="76888-177">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-177">Has Yammer License</span></span>
- <span data-ttu-id="76888-178">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="76888-178">Has Teams License</span></span>
- <span data-ttu-id="76888-179">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-179">Yammer Last Activity Date</span></span>
- <span data-ttu-id="76888-180">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="76888-180">Teams Last Activity Date</span></span>
- <span data-ttu-id="76888-181">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-181">Yammer License Assign Date</span></span>
- <span data-ttu-id="76888-182">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="76888-182">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="76888-183">JSON</span><span class="sxs-lookup"><span data-stu-id="76888-183">JSON</span></span>

<span data-ttu-id="76888-184">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="76888-184">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="76888-185">由世纪银行运营的 Microsoft Graph不支持 **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="76888-185">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="76888-186">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="76888-186">hasYammerLicense</span></span>
- <span data-ttu-id="76888-187">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="76888-187">hasTeamsLicense</span></span>
- <span data-ttu-id="76888-188">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="76888-188">yammerLastActivityDate</span></span>
- <span data-ttu-id="76888-189">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="76888-189">teamsLastActivityDate</span></span>
- <span data-ttu-id="76888-190">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="76888-190">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="76888-191">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="76888-191">teamsLicenseAssignDate</span></span>

<span data-ttu-id="76888-192">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="76888-192">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="76888-193">示例</span><span class="sxs-lookup"><span data-stu-id="76888-193">Example</span></span>

### <a name="csv"></a><span data-ttu-id="76888-194">CSV</span><span class="sxs-lookup"><span data-stu-id="76888-194">CSV</span></span>

<span data-ttu-id="76888-195">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="76888-195">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="76888-196">请求</span><span class="sxs-lookup"><span data-stu-id="76888-196">Request</span></span>

<span data-ttu-id="76888-197">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76888-197">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="76888-198">响应</span><span class="sxs-lookup"><span data-stu-id="76888-198">Response</span></span>

<span data-ttu-id="76888-199">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76888-199">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="76888-200">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="76888-200">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="76888-201">JSON</span><span class="sxs-lookup"><span data-stu-id="76888-201">JSON</span></span>

<span data-ttu-id="76888-202">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="76888-202">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="76888-203">请求</span><span class="sxs-lookup"><span data-stu-id="76888-203">Request</span></span>

<span data-ttu-id="76888-204">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76888-204">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="76888-205">响应</span><span class="sxs-lookup"><span data-stu-id="76888-205">Response</span></span>

<span data-ttu-id="76888-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76888-206">The following is an example of the response.</span></span>

> <span data-ttu-id="76888-207">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="76888-207">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "Microsoft 365 ENTERPRISE E5"
      ]
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


