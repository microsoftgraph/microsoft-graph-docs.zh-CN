---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 获取组执行的 Office 365 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3d99cd7c80dd16c6ded518f7e1cbe9fecd0b3230
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515445"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="e7c30-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e7c30-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7c30-104">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e7c30-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="e7c30-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="e7c30-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7c30-106">权限</span><span class="sxs-lookup"><span data-stu-id="e7c30-106">Permissions</span></span>

<span data-ttu-id="e7c30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7c30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7c30-109">Permission type</span></span>                        | <span data-ttu-id="e7c30-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7c30-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e7c30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c30-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7c30-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c30-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e7c30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7c30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7c30-114">Not supported.</span></span>                           |
| <span data-ttu-id="e7c30-115">应用</span><span class="sxs-lookup"><span data-stu-id="e7c30-115">Application</span></span>                            | <span data-ttu-id="e7c30-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c30-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e7c30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7c30-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e7c30-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="e7c30-118">Function parameters</span></span>

<span data-ttu-id="e7c30-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="e7c30-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e7c30-120">参数</span><span class="sxs-lookup"><span data-stu-id="e7c30-120">Parameter</span></span> | <span data-ttu-id="e7c30-121">类型</span><span class="sxs-lookup"><span data-stu-id="e7c30-121">Type</span></span>   | <span data-ttu-id="e7c30-122">说明</span><span class="sxs-lookup"><span data-stu-id="e7c30-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e7c30-123">period</span><span class="sxs-lookup"><span data-stu-id="e7c30-123">period</span></span>    | <span data-ttu-id="e7c30-124">string</span><span class="sxs-lookup"><span data-stu-id="e7c30-124">string</span></span> | <span data-ttu-id="e7c30-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e7c30-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e7c30-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e7c30-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e7c30-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e7c30-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e7c30-128">date</span><span class="sxs-lookup"><span data-stu-id="e7c30-128">date</span></span>      | <span data-ttu-id="e7c30-129">Date</span><span class="sxs-lookup"><span data-stu-id="e7c30-129">Date</span></span>   | <span data-ttu-id="e7c30-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="e7c30-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e7c30-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="e7c30-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e7c30-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="e7c30-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e7c30-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="e7c30-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e7c30-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e7c30-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e7c30-135">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="e7c30-135">The default output type is text/csv.</span></span> <span data-ttu-id="e7c30-136">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="e7c30-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7c30-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7c30-137">Request headers</span></span>

| <span data-ttu-id="e7c30-138">名称</span><span class="sxs-lookup"><span data-stu-id="e7c30-138">Name</span></span>          | <span data-ttu-id="e7c30-139">说明</span><span class="sxs-lookup"><span data-stu-id="e7c30-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e7c30-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c30-140">Authorization</span></span> | <span data-ttu-id="e7c30-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7c30-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e7c30-143">响应</span><span class="sxs-lookup"><span data-stu-id="e7c30-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e7c30-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e7c30-144">CSV</span></span>

<span data-ttu-id="e7c30-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e7c30-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e7c30-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e7c30-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e7c30-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e7c30-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e7c30-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e7c30-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e7c30-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e7c30-149">Report Refresh Date</span></span>
- <span data-ttu-id="e7c30-150">组显示名称</span><span class="sxs-lookup"><span data-stu-id="e7c30-150">Group Display Name</span></span>
- <span data-ttu-id="e7c30-151">已删除</span><span class="sxs-lookup"><span data-stu-id="e7c30-151">Is Deleted</span></span>
- <span data-ttu-id="e7c30-152">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="e7c30-152">Owner Principal Name</span></span>
- <span data-ttu-id="e7c30-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e7c30-153">Last Activity Date</span></span>
- <span data-ttu-id="e7c30-154">组类型</span><span class="sxs-lookup"><span data-stu-id="e7c30-154">Group Type</span></span>
- <span data-ttu-id="e7c30-155">成员数</span><span class="sxs-lookup"><span data-stu-id="e7c30-155">Member Count</span></span>
- <span data-ttu-id="e7c30-156">外部成员数</span><span class="sxs-lookup"><span data-stu-id="e7c30-156">External Member Count</span></span>
- <span data-ttu-id="e7c30-157">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="e7c30-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="e7c30-158">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="e7c30-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="e7c30-159">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="e7c30-160">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="e7c30-161">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="e7c30-162">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="e7c30-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="e7c30-163">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="e7c30-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="e7c30-164">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="e7c30-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="e7c30-165">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="e7c30-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="e7c30-166">报表周期</span><span class="sxs-lookup"><span data-stu-id="e7c30-166">Report Period</span></span>

<span data-ttu-id="e7c30-167">在 Microsoft Graph 中国由 21Vianet 不支持下列：</span><span class="sxs-lookup"><span data-stu-id="e7c30-167">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e7c30-168">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-168">Yammer Posted Message Count</span></span>
- <span data-ttu-id="e7c30-169">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-169">Yammer Read Message Count</span></span>
- <span data-ttu-id="e7c30-170">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="e7c30-170">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="e7c30-171">JSON</span><span class="sxs-lookup"><span data-stu-id="e7c30-171">JSON</span></span>

<span data-ttu-id="e7c30-172">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e7c30-172">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="e7c30-173">在 Microsoft Graph 中国由 21Vianet 不支持**[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="e7c30-173">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="e7c30-174">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="e7c30-174">yammerPostedMessageCount</span></span>
- <span data-ttu-id="e7c30-175">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="e7c30-175">yammerReadMessageCount</span></span>
- <span data-ttu-id="e7c30-176">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="e7c30-176">yammerLikedMessageCount</span></span>

<span data-ttu-id="e7c30-177">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="e7c30-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e7c30-178">示例</span><span class="sxs-lookup"><span data-stu-id="e7c30-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e7c30-179">CSV</span><span class="sxs-lookup"><span data-stu-id="e7c30-179">CSV</span></span>

<span data-ttu-id="e7c30-180">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="e7c30-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e7c30-181">请求</span><span class="sxs-lookup"><span data-stu-id="e7c30-181">Request</span></span>

<span data-ttu-id="e7c30-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e7c30-182">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e7c30-183">响应</span><span class="sxs-lookup"><span data-stu-id="e7c30-183">Response</span></span>

<span data-ttu-id="e7c30-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e7c30-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e7c30-185">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e7c30-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="e7c30-186">JSON</span><span class="sxs-lookup"><span data-stu-id="e7c30-186">JSON</span></span>

<span data-ttu-id="e7c30-187">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e7c30-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e7c30-188">请求</span><span class="sxs-lookup"><span data-stu-id="e7c30-188">Request</span></span>

<span data-ttu-id="e7c30-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e7c30-189">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e7c30-190">响应</span><span class="sxs-lookup"><span data-stu-id="e7c30-190">Response</span></span>

<span data-ttu-id="e7c30-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e7c30-191">The following is an example of the response.</span></span>

> <span data-ttu-id="e7c30-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e7c30-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
