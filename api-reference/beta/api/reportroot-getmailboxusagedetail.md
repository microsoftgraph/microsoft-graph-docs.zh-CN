---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f22fcff82f3ccba4f0bd5e7a486d7a2422b91db5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454456"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="f0784-103">reportRoot：getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="f0784-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="f0784-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0784-105">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f0784-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="f0784-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="f0784-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0784-107">权限</span><span class="sxs-lookup"><span data-stu-id="f0784-107">Permissions</span></span>

<span data-ttu-id="f0784-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0784-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0784-110">Permission type</span></span>                        | <span data-ttu-id="f0784-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0784-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f0784-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0784-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0784-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0784-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f0784-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0784-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0784-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0784-115">Not supported.</span></span>                           |
| <span data-ttu-id="f0784-116">应用</span><span class="sxs-lookup"><span data-stu-id="f0784-116">Application</span></span>                            | <span data-ttu-id="f0784-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0784-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="f0784-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f0784-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f0784-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="f0784-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f0784-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0784-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f0784-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="f0784-121">Function parameters</span></span>

<span data-ttu-id="f0784-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f0784-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f0784-123">参数</span><span class="sxs-lookup"><span data-stu-id="f0784-123">Parameter</span></span> | <span data-ttu-id="f0784-124">类型</span><span class="sxs-lookup"><span data-stu-id="f0784-124">Type</span></span>   | <span data-ttu-id="f0784-125">说明</span><span class="sxs-lookup"><span data-stu-id="f0784-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f0784-126">period</span><span class="sxs-lookup"><span data-stu-id="f0784-126">period</span></span>    | <span data-ttu-id="f0784-127">string</span><span class="sxs-lookup"><span data-stu-id="f0784-127">string</span></span> | <span data-ttu-id="f0784-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f0784-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f0784-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f0784-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f0784-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f0784-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f0784-131">必需。</span><span class="sxs-lookup"><span data-stu-id="f0784-131">Required.</span></span> |

<span data-ttu-id="f0784-132">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0784-132">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f0784-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="f0784-133">The default output type is text/csv.</span></span> <span data-ttu-id="f0784-134">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="f0784-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0784-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0784-135">Request headers</span></span>

| <span data-ttu-id="f0784-136">名称</span><span class="sxs-lookup"><span data-stu-id="f0784-136">Name</span></span>          | <span data-ttu-id="f0784-137">说明</span><span class="sxs-lookup"><span data-stu-id="f0784-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f0784-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0784-138">Authorization</span></span> | <span data-ttu-id="f0784-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0784-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f0784-141">响应</span><span class="sxs-lookup"><span data-stu-id="f0784-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f0784-142">CSV</span><span class="sxs-lookup"><span data-stu-id="f0784-142">CSV</span></span>

<span data-ttu-id="f0784-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f0784-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f0784-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f0784-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f0784-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f0784-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f0784-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f0784-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f0784-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f0784-147">Report Refresh Date</span></span>
- <span data-ttu-id="f0784-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f0784-148">User Principal Name</span></span>
- <span data-ttu-id="f0784-149">显示名称</span><span class="sxs-lookup"><span data-stu-id="f0784-149">Display Name</span></span>
- <span data-ttu-id="f0784-150">已删除</span><span class="sxs-lookup"><span data-stu-id="f0784-150">Is Deleted</span></span>
- <span data-ttu-id="f0784-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="f0784-151">Deleted Date</span></span>
- <span data-ttu-id="f0784-152">创建日期</span><span class="sxs-lookup"><span data-stu-id="f0784-152">Created Date</span></span>
- <span data-ttu-id="f0784-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="f0784-153">Last Activity Date</span></span>
- <span data-ttu-id="f0784-154">项数</span><span class="sxs-lookup"><span data-stu-id="f0784-154">Item Count</span></span>
- <span data-ttu-id="f0784-155">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="f0784-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="f0784-156">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="f0784-156">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="f0784-157">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="f0784-157">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="f0784-158">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="f0784-158">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="f0784-159">删除项目计数</span><span class="sxs-lookup"><span data-stu-id="f0784-159">Deleted Item Count</span></span>
- <span data-ttu-id="f0784-160">删除项目大小（字节）</span><span class="sxs-lookup"><span data-stu-id="f0784-160">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="f0784-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="f0784-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f0784-162">JSON</span><span class="sxs-lookup"><span data-stu-id="f0784-162">JSON</span></span>

<span data-ttu-id="f0784-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="f0784-163">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="f0784-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="f0784-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="f0784-165">示例</span><span class="sxs-lookup"><span data-stu-id="f0784-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f0784-166">CSV</span><span class="sxs-lookup"><span data-stu-id="f0784-166">CSV</span></span>

<span data-ttu-id="f0784-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="f0784-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f0784-168">请求</span><span class="sxs-lookup"><span data-stu-id="f0784-168">Request</span></span>

<span data-ttu-id="f0784-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0784-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0784-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0784-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="f0784-171">C#</span><span class="sxs-lookup"><span data-stu-id="f0784-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0784-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0784-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0784-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0784-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0784-174">响应</span><span class="sxs-lookup"><span data-stu-id="f0784-174">Response</span></span>

<span data-ttu-id="f0784-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0784-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f0784-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f0784-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f0784-177">JSON</span><span class="sxs-lookup"><span data-stu-id="f0784-177">JSON</span></span>

<span data-ttu-id="f0784-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="f0784-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f0784-179">请求</span><span class="sxs-lookup"><span data-stu-id="f0784-179">Request</span></span>

<span data-ttu-id="f0784-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0784-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0784-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0784-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="f0784-182">C#</span><span class="sxs-lookup"><span data-stu-id="f0784-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0784-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0784-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0784-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0784-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0784-185">响应</span><span class="sxs-lookup"><span data-stu-id="f0784-185">Response</span></span>

<span data-ttu-id="f0784-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f0784-186">The following is an example of the response.</span></span>

> <span data-ttu-id="f0784-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f0784-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
