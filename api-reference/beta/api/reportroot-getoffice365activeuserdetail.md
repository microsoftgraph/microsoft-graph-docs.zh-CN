---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3192062a7e533995804b0e26bf948277690047e8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869141"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="3edbf-103">reportRoot：getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="3edbf-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3edbf-104">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3edbf-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="3edbf-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="3edbf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3edbf-106">权限</span><span class="sxs-lookup"><span data-stu-id="3edbf-106">Permissions</span></span>

<span data-ttu-id="3edbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3edbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3edbf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3edbf-109">Permission type</span></span>                        | <span data-ttu-id="3edbf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3edbf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3edbf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3edbf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3edbf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3edbf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3edbf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3edbf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3edbf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3edbf-114">Not supported.</span></span>                           |
| <span data-ttu-id="3edbf-115">应用</span><span class="sxs-lookup"><span data-stu-id="3edbf-115">Application</span></span>                            | <span data-ttu-id="3edbf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3edbf-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3edbf-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3edbf-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3edbf-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3edbf-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3edbf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3edbf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3edbf-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="3edbf-120">Function parameters</span></span>

<span data-ttu-id="3edbf-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3edbf-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3edbf-122">参数</span><span class="sxs-lookup"><span data-stu-id="3edbf-122">Parameter</span></span> | <span data-ttu-id="3edbf-123">类型</span><span class="sxs-lookup"><span data-stu-id="3edbf-123">Type</span></span>   | <span data-ttu-id="3edbf-124">说明</span><span class="sxs-lookup"><span data-stu-id="3edbf-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3edbf-125">period</span><span class="sxs-lookup"><span data-stu-id="3edbf-125">period</span></span>    | <span data-ttu-id="3edbf-126">string</span><span class="sxs-lookup"><span data-stu-id="3edbf-126">string</span></span> | <span data-ttu-id="3edbf-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3edbf-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3edbf-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3edbf-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3edbf-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3edbf-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3edbf-130">date</span><span class="sxs-lookup"><span data-stu-id="3edbf-130">date</span></span>      | <span data-ttu-id="3edbf-131">Date</span><span class="sxs-lookup"><span data-stu-id="3edbf-131">Date</span></span>   | <span data-ttu-id="3edbf-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="3edbf-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3edbf-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="3edbf-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3edbf-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="3edbf-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3edbf-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="3edbf-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3edbf-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3edbf-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3edbf-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3edbf-137">The default output type is text/csv.</span></span> <span data-ttu-id="3edbf-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3edbf-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3edbf-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="3edbf-139">Request headers</span></span>

| <span data-ttu-id="3edbf-140">名称</span><span class="sxs-lookup"><span data-stu-id="3edbf-140">Name</span></span>          | <span data-ttu-id="3edbf-141">说明</span><span class="sxs-lookup"><span data-stu-id="3edbf-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3edbf-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="3edbf-142">Authorization</span></span> | <span data-ttu-id="3edbf-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3edbf-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3edbf-145">响应</span><span class="sxs-lookup"><span data-stu-id="3edbf-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3edbf-146">CSV</span><span class="sxs-lookup"><span data-stu-id="3edbf-146">CSV</span></span>

<span data-ttu-id="3edbf-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3edbf-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3edbf-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3edbf-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3edbf-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="3edbf-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3edbf-150">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="3edbf-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3edbf-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-151">Report Refresh Date</span></span>
- <span data-ttu-id="3edbf-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="3edbf-152">User Principal Name</span></span>
- <span data-ttu-id="3edbf-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="3edbf-153">Display Name</span></span>
- <span data-ttu-id="3edbf-154">已删除</span><span class="sxs-lookup"><span data-stu-id="3edbf-154">Is Deleted</span></span>
- <span data-ttu-id="3edbf-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-155">Deleted Date</span></span>
- <span data-ttu-id="3edbf-156">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-156">Has Exchange License</span></span>
- <span data-ttu-id="3edbf-157">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-157">Has OneDrive License</span></span>
- <span data-ttu-id="3edbf-158">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-158">Has SharePoint License</span></span>
- <span data-ttu-id="3edbf-159">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-159">Has Skype For Business License</span></span>
- <span data-ttu-id="3edbf-160">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-160">Has Yammer License</span></span>
- <span data-ttu-id="3edbf-161">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-161">Has Teams License</span></span>
- <span data-ttu-id="3edbf-162">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="3edbf-163">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="3edbf-164">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="3edbf-165">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="3edbf-166">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="3edbf-167">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="3edbf-168">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="3edbf-169">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="3edbf-170">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="3edbf-171">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="3edbf-172">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="3edbf-173">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-173">Teams License Assign Date</span></span>
- <span data-ttu-id="3edbf-174">分配的产品</span><span class="sxs-lookup"><span data-stu-id="3edbf-174">Assigned Products</span></span>

<span data-ttu-id="3edbf-175">由世纪互联运营的 Microsoft Graph 中国不支持以下各列：</span><span class="sxs-lookup"><span data-stu-id="3edbf-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3edbf-176">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-176">Has Yammer License</span></span>
- <span data-ttu-id="3edbf-177">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="3edbf-177">Has Teams License</span></span>
- <span data-ttu-id="3edbf-178">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="3edbf-179">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="3edbf-180">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="3edbf-181">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="3edbf-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="3edbf-182">JSON</span><span class="sxs-lookup"><span data-stu-id="3edbf-182">JSON</span></span>

<span data-ttu-id="3edbf-183">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3edbf-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="3edbf-184">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="3edbf-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3edbf-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="3edbf-185">hasYammerLicense</span></span>
- <span data-ttu-id="3edbf-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="3edbf-186">hasTeamsLicense</span></span>
- <span data-ttu-id="3edbf-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3edbf-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="3edbf-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3edbf-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="3edbf-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="3edbf-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="3edbf-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="3edbf-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="3edbf-191">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="3edbf-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3edbf-192">示例</span><span class="sxs-lookup"><span data-stu-id="3edbf-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3edbf-193">CSV</span><span class="sxs-lookup"><span data-stu-id="3edbf-193">CSV</span></span>

<span data-ttu-id="3edbf-194">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3edbf-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3edbf-195">请求</span><span class="sxs-lookup"><span data-stu-id="3edbf-195">Request</span></span>

<span data-ttu-id="3edbf-196">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3edbf-196">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3edbf-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="3edbf-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3edbf-198">C#</span><span class="sxs-lookup"><span data-stu-id="3edbf-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3edbf-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3edbf-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3edbf-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3edbf-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3edbf-201">响应</span><span class="sxs-lookup"><span data-stu-id="3edbf-201">Response</span></span>

<span data-ttu-id="3edbf-202">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3edbf-202">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3edbf-203">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3edbf-203">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3edbf-204">JSON</span><span class="sxs-lookup"><span data-stu-id="3edbf-204">JSON</span></span>

<span data-ttu-id="3edbf-205">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3edbf-205">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3edbf-206">请求</span><span class="sxs-lookup"><span data-stu-id="3edbf-206">Request</span></span>

<span data-ttu-id="3edbf-207">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3edbf-207">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3edbf-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="3edbf-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3edbf-209">C#</span><span class="sxs-lookup"><span data-stu-id="3edbf-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3edbf-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3edbf-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3edbf-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3edbf-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3edbf-212">响应</span><span class="sxs-lookup"><span data-stu-id="3edbf-212">Response</span></span>

<span data-ttu-id="3edbf-213">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3edbf-213">The following is an example of the response.</span></span>

> <span data-ttu-id="3edbf-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3edbf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
