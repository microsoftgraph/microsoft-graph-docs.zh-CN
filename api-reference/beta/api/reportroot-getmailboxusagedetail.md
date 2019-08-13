---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 286d29ccfcd00793f83d4e09cbbba4acf937140b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360560"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="df08c-103">reportRoot：getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="df08c-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df08c-104">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="df08c-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="df08c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="df08c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="df08c-106">权限</span><span class="sxs-lookup"><span data-stu-id="df08c-106">Permissions</span></span>

<span data-ttu-id="df08c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df08c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df08c-109">Permission type</span></span>                        | <span data-ttu-id="df08c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df08c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="df08c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df08c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df08c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df08c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="df08c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df08c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df08c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df08c-114">Not supported.</span></span>                           |
| <span data-ttu-id="df08c-115">应用</span><span class="sxs-lookup"><span data-stu-id="df08c-115">Application</span></span>                            | <span data-ttu-id="df08c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df08c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="df08c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df08c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="df08c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="df08c-118">Function parameters</span></span>

<span data-ttu-id="df08c-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="df08c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="df08c-120">参数</span><span class="sxs-lookup"><span data-stu-id="df08c-120">Parameter</span></span> | <span data-ttu-id="df08c-121">类型</span><span class="sxs-lookup"><span data-stu-id="df08c-121">Type</span></span>   | <span data-ttu-id="df08c-122">说明</span><span class="sxs-lookup"><span data-stu-id="df08c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="df08c-123">period</span><span class="sxs-lookup"><span data-stu-id="df08c-123">period</span></span>    | <span data-ttu-id="df08c-124">string</span><span class="sxs-lookup"><span data-stu-id="df08c-124">string</span></span> | <span data-ttu-id="df08c-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="df08c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="df08c-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="df08c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="df08c-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="df08c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="df08c-128">必需。</span><span class="sxs-lookup"><span data-stu-id="df08c-128">Required.</span></span> |

<span data-ttu-id="df08c-129">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df08c-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="df08c-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="df08c-130">The default output type is text/csv.</span></span> <span data-ttu-id="df08c-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="df08c-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df08c-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="df08c-132">Request headers</span></span>

| <span data-ttu-id="df08c-133">名称</span><span class="sxs-lookup"><span data-stu-id="df08c-133">Name</span></span>          | <span data-ttu-id="df08c-134">说明</span><span class="sxs-lookup"><span data-stu-id="df08c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="df08c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="df08c-135">Authorization</span></span> | <span data-ttu-id="df08c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df08c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="df08c-138">响应</span><span class="sxs-lookup"><span data-stu-id="df08c-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="df08c-139">CSV</span><span class="sxs-lookup"><span data-stu-id="df08c-139">CSV</span></span>

<span data-ttu-id="df08c-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="df08c-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="df08c-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="df08c-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="df08c-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="df08c-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="df08c-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="df08c-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="df08c-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="df08c-144">Report Refresh Date</span></span>
- <span data-ttu-id="df08c-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="df08c-145">User Principal Name</span></span>
- <span data-ttu-id="df08c-146">显示名称</span><span class="sxs-lookup"><span data-stu-id="df08c-146">Display Name</span></span>
- <span data-ttu-id="df08c-147">已删除</span><span class="sxs-lookup"><span data-stu-id="df08c-147">Is Deleted</span></span>
- <span data-ttu-id="df08c-148">删除日期</span><span class="sxs-lookup"><span data-stu-id="df08c-148">Deleted Date</span></span>
- <span data-ttu-id="df08c-149">创建日期</span><span class="sxs-lookup"><span data-stu-id="df08c-149">Created Date</span></span>
- <span data-ttu-id="df08c-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="df08c-150">Last Activity Date</span></span>
- <span data-ttu-id="df08c-151">项数</span><span class="sxs-lookup"><span data-stu-id="df08c-151">Item Count</span></span>
- <span data-ttu-id="df08c-152">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="df08c-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="df08c-153">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="df08c-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="df08c-154">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="df08c-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="df08c-155">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="df08c-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="df08c-156">已删除邮件数</span><span class="sxs-lookup"><span data-stu-id="df08c-156">Deleted Item Count</span></span>
- <span data-ttu-id="df08c-157">删除的项目大小 (字节)</span><span class="sxs-lookup"><span data-stu-id="df08c-157">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="df08c-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="df08c-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="df08c-159">JSON</span><span class="sxs-lookup"><span data-stu-id="df08c-159">JSON</span></span>

<span data-ttu-id="df08c-160">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="df08c-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="df08c-161">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="df08c-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="df08c-162">示例</span><span class="sxs-lookup"><span data-stu-id="df08c-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="df08c-163">CSV</span><span class="sxs-lookup"><span data-stu-id="df08c-163">CSV</span></span>

<span data-ttu-id="df08c-164">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="df08c-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="df08c-165">请求</span><span class="sxs-lookup"><span data-stu-id="df08c-165">Request</span></span>

<span data-ttu-id="df08c-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df08c-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="df08c-167">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="df08c-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df08c-168">C#</span><span class="sxs-lookup"><span data-stu-id="df08c-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df08c-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df08c-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df08c-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="df08c-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="df08c-171">Java</span><span class="sxs-lookup"><span data-stu-id="df08c-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagedetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df08c-172">响应</span><span class="sxs-lookup"><span data-stu-id="df08c-172">Response</span></span>

<span data-ttu-id="df08c-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df08c-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="df08c-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="df08c-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="df08c-175">JSON</span><span class="sxs-lookup"><span data-stu-id="df08c-175">JSON</span></span>

<span data-ttu-id="df08c-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="df08c-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="df08c-177">请求</span><span class="sxs-lookup"><span data-stu-id="df08c-177">Request</span></span>

<span data-ttu-id="df08c-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df08c-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="df08c-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="df08c-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df08c-180">C#</span><span class="sxs-lookup"><span data-stu-id="df08c-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df08c-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df08c-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df08c-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="df08c-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="df08c-183">Java</span><span class="sxs-lookup"><span data-stu-id="df08c-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagedetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df08c-184">响应</span><span class="sxs-lookup"><span data-stu-id="df08c-184">Response</span></span>

<span data-ttu-id="df08c-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="df08c-185">The following is an example of the response.</span></span>

> <span data-ttu-id="df08c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df08c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
