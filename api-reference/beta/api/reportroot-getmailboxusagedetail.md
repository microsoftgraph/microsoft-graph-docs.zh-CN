---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bde7f1a5b9416c80ab362effb6a3b063f2e66919
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589089"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="b01b7-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="b01b7-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="b01b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01b7-105">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b01b7-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="b01b7-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="b01b7-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="b01b7-107">权限</span><span class="sxs-lookup"><span data-stu-id="b01b7-107">Permissions</span></span>

<span data-ttu-id="b01b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b01b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b01b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b01b7-110">Permission type</span></span>                        | <span data-ttu-id="b01b7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b01b7-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b01b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b01b7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b01b7-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01b7-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b01b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b01b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b01b7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b01b7-115">Not supported.</span></span>                           |
| <span data-ttu-id="b01b7-116">应用</span><span class="sxs-lookup"><span data-stu-id="b01b7-116">Application</span></span>                            | <span data-ttu-id="b01b7-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b01b7-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="b01b7-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="b01b7-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b01b7-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="b01b7-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b01b7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b01b7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b01b7-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="b01b7-121">Function parameters</span></span>

<span data-ttu-id="b01b7-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b01b7-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b01b7-123">参数</span><span class="sxs-lookup"><span data-stu-id="b01b7-123">Parameter</span></span> | <span data-ttu-id="b01b7-124">类型</span><span class="sxs-lookup"><span data-stu-id="b01b7-124">Type</span></span>   | <span data-ttu-id="b01b7-125">说明</span><span class="sxs-lookup"><span data-stu-id="b01b7-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b01b7-126">period</span><span class="sxs-lookup"><span data-stu-id="b01b7-126">period</span></span>    | <span data-ttu-id="b01b7-127">string</span><span class="sxs-lookup"><span data-stu-id="b01b7-127">string</span></span> | <span data-ttu-id="b01b7-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b01b7-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b01b7-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b01b7-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b01b7-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b01b7-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b01b7-131">必需。</span><span class="sxs-lookup"><span data-stu-id="b01b7-131">Required.</span></span> |

<span data-ttu-id="b01b7-132">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b01b7-132">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b01b7-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="b01b7-133">The default output type is text/csv.</span></span> <span data-ttu-id="b01b7-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="b01b7-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b01b7-135">请求头</span><span class="sxs-lookup"><span data-stu-id="b01b7-135">Request headers</span></span>

| <span data-ttu-id="b01b7-136">名称</span><span class="sxs-lookup"><span data-stu-id="b01b7-136">Name</span></span>          | <span data-ttu-id="b01b7-137">说明</span><span class="sxs-lookup"><span data-stu-id="b01b7-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b01b7-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b01b7-138">Authorization</span></span> | <span data-ttu-id="b01b7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b01b7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b01b7-141">响应</span><span class="sxs-lookup"><span data-stu-id="b01b7-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b01b7-142">CSV</span><span class="sxs-lookup"><span data-stu-id="b01b7-142">CSV</span></span>

<span data-ttu-id="b01b7-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b01b7-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b01b7-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b01b7-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b01b7-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b01b7-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b01b7-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b01b7-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b01b7-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b01b7-147">Report Refresh Date</span></span>
- <span data-ttu-id="b01b7-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="b01b7-148">User Principal Name</span></span>
- <span data-ttu-id="b01b7-149">显示名称</span><span class="sxs-lookup"><span data-stu-id="b01b7-149">Display Name</span></span>
- <span data-ttu-id="b01b7-150">已删除</span><span class="sxs-lookup"><span data-stu-id="b01b7-150">Is Deleted</span></span>
- <span data-ttu-id="b01b7-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="b01b7-151">Deleted Date</span></span>
- <span data-ttu-id="b01b7-152">创建日期</span><span class="sxs-lookup"><span data-stu-id="b01b7-152">Created Date</span></span>
- <span data-ttu-id="b01b7-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b01b7-153">Last Activity Date</span></span>
- <span data-ttu-id="b01b7-154">项数</span><span class="sxs-lookup"><span data-stu-id="b01b7-154">Item Count</span></span>
- <span data-ttu-id="b01b7-155">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="b01b7-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="b01b7-156">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="b01b7-156">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="b01b7-157">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="b01b7-157">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="b01b7-158">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="b01b7-158">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="b01b7-159">删除项目计数</span><span class="sxs-lookup"><span data-stu-id="b01b7-159">Deleted Item Count</span></span>
- <span data-ttu-id="b01b7-160">删除项目大小（字节）</span><span class="sxs-lookup"><span data-stu-id="b01b7-160">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="b01b7-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="b01b7-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b01b7-162">JSON</span><span class="sxs-lookup"><span data-stu-id="b01b7-162">JSON</span></span>

<span data-ttu-id="b01b7-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b01b7-163">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="b01b7-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="b01b7-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b01b7-165">示例</span><span class="sxs-lookup"><span data-stu-id="b01b7-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b01b7-166">CSV</span><span class="sxs-lookup"><span data-stu-id="b01b7-166">CSV</span></span>

<span data-ttu-id="b01b7-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="b01b7-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b01b7-168">请求</span><span class="sxs-lookup"><span data-stu-id="b01b7-168">Request</span></span>

<span data-ttu-id="b01b7-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01b7-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="b01b7-170">响应</span><span class="sxs-lookup"><span data-stu-id="b01b7-170">Response</span></span>

<span data-ttu-id="b01b7-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b01b7-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b01b7-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b01b7-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="b01b7-173">JSON</span><span class="sxs-lookup"><span data-stu-id="b01b7-173">JSON</span></span>

<span data-ttu-id="b01b7-174">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b01b7-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b01b7-175">请求</span><span class="sxs-lookup"><span data-stu-id="b01b7-175">Request</span></span>

<span data-ttu-id="b01b7-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b01b7-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="b01b7-177">响应</span><span class="sxs-lookup"><span data-stu-id="b01b7-177">Response</span></span>

<span data-ttu-id="b01b7-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b01b7-178">The following is an example of the response.</span></span>

> <span data-ttu-id="b01b7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b01b7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "deletedItemCount": 138481,
      "deletedItemSizeInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
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
