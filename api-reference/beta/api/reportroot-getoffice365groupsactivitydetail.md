---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 获取有关按组Microsoft 365组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: dde570c4cdfb55adb6ccf72ff3702e928b8f2944
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036665"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="6e084-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="6e084-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="6e084-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e084-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e084-105">获取有关按组Microsoft 365组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6e084-105">Get details about Microsoft 365 groups activity by group.</span></span>

> <span data-ttu-id="6e084-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 -](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="6e084-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e084-107">权限</span><span class="sxs-lookup"><span data-stu-id="6e084-107">Permissions</span></span>

<span data-ttu-id="6e084-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e084-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e084-110">Permission type</span></span>                        | <span data-ttu-id="6e084-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e084-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6e084-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e084-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e084-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e084-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6e084-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e084-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e084-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e084-115">Not supported.</span></span>                           |
| <span data-ttu-id="6e084-116">应用</span><span class="sxs-lookup"><span data-stu-id="6e084-116">Application</span></span>                            | <span data-ttu-id="6e084-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e084-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="6e084-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6e084-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6e084-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="6e084-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6e084-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e084-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6e084-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="6e084-121">Function parameters</span></span>

<span data-ttu-id="6e084-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6e084-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6e084-123">参数</span><span class="sxs-lookup"><span data-stu-id="6e084-123">Parameter</span></span> | <span data-ttu-id="6e084-124">类型</span><span class="sxs-lookup"><span data-stu-id="6e084-124">Type</span></span>   | <span data-ttu-id="6e084-125">说明</span><span class="sxs-lookup"><span data-stu-id="6e084-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6e084-126">period</span><span class="sxs-lookup"><span data-stu-id="6e084-126">period</span></span>    | <span data-ttu-id="6e084-127">string</span><span class="sxs-lookup"><span data-stu-id="6e084-127">string</span></span> | <span data-ttu-id="6e084-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e084-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6e084-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6e084-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6e084-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6e084-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6e084-131">date</span><span class="sxs-lookup"><span data-stu-id="6e084-131">date</span></span>      | <span data-ttu-id="6e084-132">Date</span><span class="sxs-lookup"><span data-stu-id="6e084-132">Date</span></span>   | <span data-ttu-id="6e084-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="6e084-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6e084-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="6e084-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6e084-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="6e084-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6e084-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="6e084-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6e084-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e084-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6e084-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="6e084-138">The default output type is text/csv.</span></span> <span data-ttu-id="6e084-139">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="6e084-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e084-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e084-140">Request headers</span></span>

| <span data-ttu-id="6e084-141">名称</span><span class="sxs-lookup"><span data-stu-id="6e084-141">Name</span></span>          | <span data-ttu-id="6e084-142">说明</span><span class="sxs-lookup"><span data-stu-id="6e084-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6e084-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e084-143">Authorization</span></span> | <span data-ttu-id="6e084-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e084-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6e084-146">响应</span><span class="sxs-lookup"><span data-stu-id="6e084-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6e084-147">CSV</span><span class="sxs-lookup"><span data-stu-id="6e084-147">CSV</span></span>

<span data-ttu-id="6e084-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6e084-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6e084-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6e084-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6e084-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6e084-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6e084-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6e084-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6e084-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6e084-152">Report Refresh Date</span></span>
- <span data-ttu-id="6e084-153">组显示名称</span><span class="sxs-lookup"><span data-stu-id="6e084-153">Group Display Name</span></span>
- <span data-ttu-id="6e084-154">已删除</span><span class="sxs-lookup"><span data-stu-id="6e084-154">Is Deleted</span></span>
- <span data-ttu-id="6e084-155">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="6e084-155">Owner Principal Name</span></span>
- <span data-ttu-id="6e084-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6e084-156">Last Activity Date</span></span>
- <span data-ttu-id="6e084-157">组类型</span><span class="sxs-lookup"><span data-stu-id="6e084-157">Group Type</span></span>
- <span data-ttu-id="6e084-158">成员数</span><span class="sxs-lookup"><span data-stu-id="6e084-158">Member Count</span></span>
- <span data-ttu-id="6e084-159">外部成员数</span><span class="sxs-lookup"><span data-stu-id="6e084-159">External Member Count</span></span>
- <span data-ttu-id="6e084-160">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="6e084-160">Exchange Received Email Count</span></span>
- <span data-ttu-id="6e084-161">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="6e084-161">SharePoint Active File Count</span></span>
- <span data-ttu-id="6e084-162">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-162">Yammer Posted Message Count</span></span>
- <span data-ttu-id="6e084-163">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-163">Yammer Read Message Count</span></span>
- <span data-ttu-id="6e084-164">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-164">Yammer Liked Message Count</span></span>
- <span data-ttu-id="6e084-165">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="6e084-165">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="6e084-166">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="6e084-166">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="6e084-167">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="6e084-167">SharePoint Total File Count</span></span>
- <span data-ttu-id="6e084-168">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="6e084-168">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="6e084-169">组 ID</span><span class="sxs-lookup"><span data-stu-id="6e084-169">Group Id</span></span>
- <span data-ttu-id="6e084-170">报表周期</span><span class="sxs-lookup"><span data-stu-id="6e084-170">Report Period</span></span>

<span data-ttu-id="6e084-171">由世纪Graph运营的 Microsoft Graph不支持以下列：</span><span class="sxs-lookup"><span data-stu-id="6e084-171">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6e084-172">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-172">Yammer Posted Message Count</span></span>
- <span data-ttu-id="6e084-173">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-173">Yammer Read Message Count</span></span>
- <span data-ttu-id="6e084-174">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6e084-174">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="6e084-175">JSON</span><span class="sxs-lookup"><span data-stu-id="6e084-175">JSON</span></span>

<span data-ttu-id="6e084-176">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6e084-176">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="6e084-177">由世纪银行运营的 Microsoft Graph不支持 **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="6e084-177">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6e084-178">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="6e084-178">yammerPostedMessageCount</span></span>
- <span data-ttu-id="6e084-179">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="6e084-179">yammerReadMessageCount</span></span>
- <span data-ttu-id="6e084-180">yammer在 Yammer的 YamEdMessageCount</span><span class="sxs-lookup"><span data-stu-id="6e084-180">yammerLikedMessageCount</span></span>

<span data-ttu-id="6e084-181">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="6e084-181">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="6e084-182">示例</span><span class="sxs-lookup"><span data-stu-id="6e084-182">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6e084-183">CSV</span><span class="sxs-lookup"><span data-stu-id="6e084-183">CSV</span></span>

<span data-ttu-id="6e084-184">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="6e084-184">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6e084-185">请求</span><span class="sxs-lookup"><span data-stu-id="6e084-185">Request</span></span>

<span data-ttu-id="6e084-186">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e084-186">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="6e084-187">响应</span><span class="sxs-lookup"><span data-stu-id="6e084-187">Response</span></span>

<span data-ttu-id="6e084-188">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e084-188">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6e084-189">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6e084-189">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
```

### <a name="json"></a><span data-ttu-id="6e084-190">JSON</span><span class="sxs-lookup"><span data-stu-id="6e084-190">JSON</span></span>

<span data-ttu-id="6e084-191">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6e084-191">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6e084-192">请求</span><span class="sxs-lookup"><span data-stu-id="6e084-192">Request</span></span>

<span data-ttu-id="6e084-193">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e084-193">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="6e084-194">响应</span><span class="sxs-lookup"><span data-stu-id="6e084-194">Response</span></span>

<span data-ttu-id="6e084-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e084-195">The following is an example of the response.</span></span>

> <span data-ttu-id="6e084-196">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6e084-196">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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


