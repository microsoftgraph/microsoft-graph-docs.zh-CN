---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 82c152c8041ddfa7a1a0a105821ac272712636d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050925"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="40649-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="40649-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="40649-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40649-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40649-105">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="40649-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="40649-106">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="40649-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="40649-107">权限</span><span class="sxs-lookup"><span data-stu-id="40649-107">Permissions</span></span>

<span data-ttu-id="40649-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40649-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="40649-110">Permission type</span></span>                        | <span data-ttu-id="40649-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40649-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="40649-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40649-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="40649-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40649-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="40649-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40649-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40649-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40649-115">Not supported.</span></span>                           |
| <span data-ttu-id="40649-116">应用</span><span class="sxs-lookup"><span data-stu-id="40649-116">Application</span></span>                            | <span data-ttu-id="40649-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="40649-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="40649-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="40649-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="40649-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="40649-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="40649-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40649-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="40649-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="40649-121">Function parameters</span></span>

<span data-ttu-id="40649-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="40649-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="40649-123">参数</span><span class="sxs-lookup"><span data-stu-id="40649-123">Parameter</span></span> | <span data-ttu-id="40649-124">类型</span><span class="sxs-lookup"><span data-stu-id="40649-124">Type</span></span>   | <span data-ttu-id="40649-125">说明</span><span class="sxs-lookup"><span data-stu-id="40649-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="40649-126">period</span><span class="sxs-lookup"><span data-stu-id="40649-126">period</span></span>    | <span data-ttu-id="40649-127">string</span><span class="sxs-lookup"><span data-stu-id="40649-127">string</span></span> | <span data-ttu-id="40649-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="40649-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="40649-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="40649-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="40649-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="40649-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="40649-131">必需。</span><span class="sxs-lookup"><span data-stu-id="40649-131">Required.</span></span> |

<span data-ttu-id="40649-132">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="40649-132">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="40649-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="40649-133">The default output type is text/csv.</span></span> <span data-ttu-id="40649-134">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="40649-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40649-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="40649-135">Request headers</span></span>

| <span data-ttu-id="40649-136">名称</span><span class="sxs-lookup"><span data-stu-id="40649-136">Name</span></span>          | <span data-ttu-id="40649-137">说明</span><span class="sxs-lookup"><span data-stu-id="40649-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="40649-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="40649-138">Authorization</span></span> | <span data-ttu-id="40649-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40649-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="40649-141">响应</span><span class="sxs-lookup"><span data-stu-id="40649-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="40649-142">CSV</span><span class="sxs-lookup"><span data-stu-id="40649-142">CSV</span></span>

<span data-ttu-id="40649-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="40649-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="40649-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="40649-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="40649-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="40649-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="40649-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="40649-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="40649-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="40649-147">Report Refresh Date</span></span>
- <span data-ttu-id="40649-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="40649-148">User Principal Name</span></span>
- <span data-ttu-id="40649-149">显示名称</span><span class="sxs-lookup"><span data-stu-id="40649-149">Display Name</span></span>
- <span data-ttu-id="40649-150">已删除</span><span class="sxs-lookup"><span data-stu-id="40649-150">Is Deleted</span></span>
- <span data-ttu-id="40649-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="40649-151">Deleted Date</span></span>
- <span data-ttu-id="40649-152">创建日期</span><span class="sxs-lookup"><span data-stu-id="40649-152">Created Date</span></span>
- <span data-ttu-id="40649-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="40649-153">Last Activity Date</span></span>
- <span data-ttu-id="40649-154">项数</span><span class="sxs-lookup"><span data-stu-id="40649-154">Item Count</span></span>
- <span data-ttu-id="40649-155">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="40649-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="40649-156">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="40649-156">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="40649-157">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="40649-157">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="40649-158">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="40649-158">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="40649-159">删除项目计数</span><span class="sxs-lookup"><span data-stu-id="40649-159">Deleted Item Count</span></span>
- <span data-ttu-id="40649-160">删除项目大小（字节）</span><span class="sxs-lookup"><span data-stu-id="40649-160">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="40649-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="40649-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="40649-162">JSON</span><span class="sxs-lookup"><span data-stu-id="40649-162">JSON</span></span>

<span data-ttu-id="40649-163">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="40649-163">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="40649-164">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="40649-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="40649-165">示例</span><span class="sxs-lookup"><span data-stu-id="40649-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="40649-166">CSV</span><span class="sxs-lookup"><span data-stu-id="40649-166">CSV</span></span>

<span data-ttu-id="40649-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="40649-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="40649-168">请求</span><span class="sxs-lookup"><span data-stu-id="40649-168">Request</span></span>

<span data-ttu-id="40649-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40649-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="40649-170">响应</span><span class="sxs-lookup"><span data-stu-id="40649-170">Response</span></span>

<span data-ttu-id="40649-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40649-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="40649-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="40649-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="40649-173">JSON</span><span class="sxs-lookup"><span data-stu-id="40649-173">JSON</span></span>

<span data-ttu-id="40649-174">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="40649-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="40649-175">请求</span><span class="sxs-lookup"><span data-stu-id="40649-175">Request</span></span>

<span data-ttu-id="40649-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40649-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="40649-177">响应</span><span class="sxs-lookup"><span data-stu-id="40649-177">Response</span></span>

<span data-ttu-id="40649-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40649-178">The following is an example of the response.</span></span>

> <span data-ttu-id="40649-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="40649-179">**Note:** The response object shown here might be shortened for readability.</span></span>

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


