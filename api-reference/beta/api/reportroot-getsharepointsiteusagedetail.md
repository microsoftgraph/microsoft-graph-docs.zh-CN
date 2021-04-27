---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: 获取 SharePoint 网站使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: b58d90ef3be8a723190909ee960f659de6f6c58b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049063"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="efb10-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="efb10-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="efb10-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efb10-105">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="efb10-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="efb10-106">**注意：** 有关不同报告视图和名称的详细信息，请参阅Microsoft 365 [报告 -](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)SharePoint使用率。</span><span class="sxs-lookup"><span data-stu-id="efb10-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="efb10-107">权限</span><span class="sxs-lookup"><span data-stu-id="efb10-107">Permissions</span></span>

<span data-ttu-id="efb10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efb10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efb10-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="efb10-110">Permission type</span></span>                        | <span data-ttu-id="efb10-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efb10-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="efb10-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efb10-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="efb10-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="efb10-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="efb10-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efb10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb10-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="efb10-115">Not supported.</span></span>                           |
| <span data-ttu-id="efb10-116">应用</span><span class="sxs-lookup"><span data-stu-id="efb10-116">Application</span></span>                            | <span data-ttu-id="efb10-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="efb10-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="efb10-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="efb10-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="efb10-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="efb10-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="efb10-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efb10-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="efb10-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="efb10-121">Function parameters</span></span>

<span data-ttu-id="efb10-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="efb10-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="efb10-123">参数</span><span class="sxs-lookup"><span data-stu-id="efb10-123">Parameter</span></span> | <span data-ttu-id="efb10-124">类型</span><span class="sxs-lookup"><span data-stu-id="efb10-124">Type</span></span>   | <span data-ttu-id="efb10-125">说明</span><span class="sxs-lookup"><span data-stu-id="efb10-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="efb10-126">period</span><span class="sxs-lookup"><span data-stu-id="efb10-126">period</span></span>    | <span data-ttu-id="efb10-127">string</span><span class="sxs-lookup"><span data-stu-id="efb10-127">string</span></span> | <span data-ttu-id="efb10-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="efb10-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="efb10-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="efb10-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="efb10-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="efb10-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="efb10-131">date</span><span class="sxs-lookup"><span data-stu-id="efb10-131">date</span></span>      | <span data-ttu-id="efb10-132">Date</span><span class="sxs-lookup"><span data-stu-id="efb10-132">Date</span></span>   | <span data-ttu-id="efb10-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="efb10-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="efb10-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="efb10-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="efb10-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="efb10-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="efb10-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="efb10-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="efb10-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="efb10-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="efb10-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="efb10-138">The default output type is text/csv.</span></span> <span data-ttu-id="efb10-139">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="efb10-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efb10-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="efb10-140">Request headers</span></span>

| <span data-ttu-id="efb10-141">名称</span><span class="sxs-lookup"><span data-stu-id="efb10-141">Name</span></span>          | <span data-ttu-id="efb10-142">说明</span><span class="sxs-lookup"><span data-stu-id="efb10-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="efb10-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb10-143">Authorization</span></span> | <span data-ttu-id="efb10-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efb10-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="efb10-146">响应</span><span class="sxs-lookup"><span data-stu-id="efb10-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="efb10-147">CSV</span><span class="sxs-lookup"><span data-stu-id="efb10-147">CSV</span></span>

<span data-ttu-id="efb10-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="efb10-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="efb10-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="efb10-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="efb10-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="efb10-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="efb10-151">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="efb10-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="efb10-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="efb10-152">Report Refresh Date</span></span>
- <span data-ttu-id="efb10-153">网站 ID</span><span class="sxs-lookup"><span data-stu-id="efb10-153">Site Id</span></span>
- <span data-ttu-id="efb10-154">网站 URL</span><span class="sxs-lookup"><span data-stu-id="efb10-154">Site URL</span></span>
- <span data-ttu-id="efb10-155">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="efb10-155">Owner Display Name</span></span>
- <span data-ttu-id="efb10-156">已删除</span><span class="sxs-lookup"><span data-stu-id="efb10-156">Is Deleted</span></span>
- <span data-ttu-id="efb10-157">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="efb10-157">Last Activity Date</span></span>
- <span data-ttu-id="efb10-158">网站敏感度标签 ID</span><span class="sxs-lookup"><span data-stu-id="efb10-158">Site Sensitivity Label Id</span></span>
- <span data-ttu-id="efb10-159">外部共享</span><span class="sxs-lookup"><span data-stu-id="efb10-159">External Sharing</span></span>
- <span data-ttu-id="efb10-160">非托管设备策略</span><span class="sxs-lookup"><span data-stu-id="efb10-160">Unmanaged Device Policy</span></span>
- <span data-ttu-id="efb10-161">地理位置</span><span class="sxs-lookup"><span data-stu-id="efb10-161">Geo Location</span></span>
- <span data-ttu-id="efb10-162">文件数</span><span class="sxs-lookup"><span data-stu-id="efb10-162">File Count</span></span>
- <span data-ttu-id="efb10-163">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="efb10-163">Active File Count</span></span>
- <span data-ttu-id="efb10-164">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="efb10-164">Page View Count</span></span>
- <span data-ttu-id="efb10-165">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="efb10-165">Visited Page Count</span></span>
- <span data-ttu-id="efb10-166">匿名链接计数</span><span class="sxs-lookup"><span data-stu-id="efb10-166">Anonymous Link Count</span></span>
- <span data-ttu-id="efb10-167">公司链接计数</span><span class="sxs-lookup"><span data-stu-id="efb10-167">Company Link Count</span></span>
- <span data-ttu-id="efb10-168">来宾计数的安全链接</span><span class="sxs-lookup"><span data-stu-id="efb10-168">Secure Link For Guest Count</span></span>
- <span data-ttu-id="efb10-169">成员计数的安全链接</span><span class="sxs-lookup"><span data-stu-id="efb10-169">Secure Link For Member Count</span></span>
- <span data-ttu-id="efb10-170">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="efb10-170">Storage Used (Byte)</span></span>
- <span data-ttu-id="efb10-171">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="efb10-171">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="efb10-172">根网站模板</span><span class="sxs-lookup"><span data-stu-id="efb10-172">Root Web Template</span></span>
- <span data-ttu-id="efb10-173">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="efb10-173">Owner Principal Name</span></span>
- <span data-ttu-id="efb10-174">报表周期</span><span class="sxs-lookup"><span data-stu-id="efb10-174">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="efb10-175">JSON</span><span class="sxs-lookup"><span data-stu-id="efb10-175">JSON</span></span>

<span data-ttu-id="efb10-176">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="efb10-176">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="efb10-177">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="efb10-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="efb10-178">示例</span><span class="sxs-lookup"><span data-stu-id="efb10-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="efb10-179">CSV</span><span class="sxs-lookup"><span data-stu-id="efb10-179">CSV</span></span>

<span data-ttu-id="efb10-180">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="efb10-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="efb10-181">请求</span><span class="sxs-lookup"><span data-stu-id="efb10-181">Request</span></span>

<span data-ttu-id="efb10-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="efb10-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="efb10-183">响应</span><span class="sxs-lookup"><span data-stu-id="efb10-183">Response</span></span>

<span data-ttu-id="efb10-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="efb10-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="efb10-185">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="efb10-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,Site Sensitivity Label Id,External Sharing,Unmanaged Device Policy,Geo Location,File Count,Active File Count,Page View Count,Visited Page Count,Anonymous Link Count,Company Link Count,Secure Link For Guest Count,Secure Link For Member Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="efb10-186">JSON</span><span class="sxs-lookup"><span data-stu-id="efb10-186">JSON</span></span>

<span data-ttu-id="efb10-187">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="efb10-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="efb10-188">请求</span><span class="sxs-lookup"><span data-stu-id="efb10-188">Request</span></span>

<span data-ttu-id="efb10-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="efb10-189">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="efb10-190">响应</span><span class="sxs-lookup"><span data-stu-id="efb10-190">Response</span></span>

<span data-ttu-id="efb10-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="efb10-191">The following is an example of the response.</span></span>

> <span data-ttu-id="efb10-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="efb10-192">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "SiteSensitivityLabelId": "SiteSensitivityLabelId-value",
      "ExternalSharing": false,
      "UnmanagedDevicePolicy": "UnmanagedDevicePolicy-value",
      "GeoLocation": "GeoLocation-value",
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "AnonymousLinkCount": 5,
      "CompanyLinkCount": 8,
      "SecureLinkForGuestCount": 13,
      "SecureLinkForMemberCount": 11,
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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


