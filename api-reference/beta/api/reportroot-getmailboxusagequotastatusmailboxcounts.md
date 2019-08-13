---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 获取每个配额类别中的用户邮箱数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f4559e24db371495399a0a2a4c298cb4c17ac2de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360587"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="b4ce1-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="b4ce1-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ce1-104">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="b4ce1-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ce1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4ce1-106">Permissions</span></span>

<span data-ttu-id="b4ce1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4ce1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4ce1-109">Permission type</span></span>                        | <span data-ttu-id="b4ce1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4ce1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b4ce1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ce1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4ce1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4ce1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b4ce1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ce1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ce1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-114">Not supported.</span></span>                           |
| <span data-ttu-id="b4ce1-115">应用</span><span class="sxs-lookup"><span data-stu-id="b4ce1-115">Application</span></span>                            | <span data-ttu-id="b4ce1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4ce1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b4ce1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4ce1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b4ce1-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="b4ce1-118">Function parameters</span></span>

<span data-ttu-id="b4ce1-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b4ce1-120">参数</span><span class="sxs-lookup"><span data-stu-id="b4ce1-120">Parameter</span></span> | <span data-ttu-id="b4ce1-121">类型</span><span class="sxs-lookup"><span data-stu-id="b4ce1-121">Type</span></span>   | <span data-ttu-id="b4ce1-122">说明</span><span class="sxs-lookup"><span data-stu-id="b4ce1-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b4ce1-123">period</span><span class="sxs-lookup"><span data-stu-id="b4ce1-123">period</span></span>    | <span data-ttu-id="b4ce1-124">string</span><span class="sxs-lookup"><span data-stu-id="b4ce1-124">string</span></span> | <span data-ttu-id="b4ce1-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b4ce1-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b4ce1-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b4ce1-128">必需。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-128">Required.</span></span> |

<span data-ttu-id="b4ce1-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b4ce1-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-130">The default output type is text/csv.</span></span> <span data-ttu-id="b4ce1-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4ce1-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4ce1-132">Request headers</span></span>

| <span data-ttu-id="b4ce1-133">名称</span><span class="sxs-lookup"><span data-stu-id="b4ce1-133">Name</span></span>          | <span data-ttu-id="b4ce1-134">说明</span><span class="sxs-lookup"><span data-stu-id="b4ce1-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b4ce1-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ce1-135">Authorization</span></span> | <span data-ttu-id="b4ce1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b4ce1-138">响应</span><span class="sxs-lookup"><span data-stu-id="b4ce1-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b4ce1-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b4ce1-139">CSV</span></span>

<span data-ttu-id="b4ce1-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b4ce1-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b4ce1-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b4ce1-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b4ce1-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b4ce1-144">Report Refresh Date</span></span>
- <span data-ttu-id="b4ce1-145">未达限制</span><span class="sxs-lookup"><span data-stu-id="b4ce1-145">Under Limit</span></span>
- <span data-ttu-id="b4ce1-146">已发出警告</span><span class="sxs-lookup"><span data-stu-id="b4ce1-146">Warning Issued</span></span>
- <span data-ttu-id="b4ce1-147">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="b4ce1-147">Send Prohibited</span></span>
- <span data-ttu-id="b4ce1-148">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="b4ce1-148">Send/Receive Prohibited</span></span>
- <span data-ttu-id="b4ce1-149">不确定</span><span class="sxs-lookup"><span data-stu-id="b4ce1-149">Indeterminate</span></span>
- <span data-ttu-id="b4ce1-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="b4ce1-150">Report Date</span></span>
- <span data-ttu-id="b4ce1-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="b4ce1-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b4ce1-152">JSON</span><span class="sxs-lookup"><span data-stu-id="b4ce1-152">JSON</span></span>

<span data-ttu-id="b4ce1-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-153">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ce1-154">示例</span><span class="sxs-lookup"><span data-stu-id="b4ce1-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b4ce1-155">CSV</span><span class="sxs-lookup"><span data-stu-id="b4ce1-155">CSV</span></span>

<span data-ttu-id="b4ce1-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b4ce1-157">请求</span><span class="sxs-lookup"><span data-stu-id="b4ce1-157">Request</span></span>

<span data-ttu-id="b4ce1-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4ce1-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b4ce1-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4ce1-160">C#</span><span class="sxs-lookup"><span data-stu-id="b4ce1-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4ce1-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ce1-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4ce1-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4ce1-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4ce1-163">Java</span><span class="sxs-lookup"><span data-stu-id="b4ce1-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4ce1-164">响应</span><span class="sxs-lookup"><span data-stu-id="b4ce1-164">Response</span></span>

<span data-ttu-id="b4ce1-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b4ce1-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b4ce1-167">JSON</span><span class="sxs-lookup"><span data-stu-id="b4ce1-167">JSON</span></span>

<span data-ttu-id="b4ce1-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b4ce1-169">请求</span><span class="sxs-lookup"><span data-stu-id="b4ce1-169">Request</span></span>

<span data-ttu-id="b4ce1-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4ce1-171">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b4ce1-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4ce1-172">C#</span><span class="sxs-lookup"><span data-stu-id="b4ce1-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4ce1-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ce1-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4ce1-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4ce1-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4ce1-175">Java</span><span class="sxs-lookup"><span data-stu-id="b4ce1-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4ce1-176">响应</span><span class="sxs-lookup"><span data-stu-id="b4ce1-176">Response</span></span>

<span data-ttu-id="b4ce1-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-177">The following is an example of the response.</span></span>

> <span data-ttu-id="b4ce1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4ce1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageQuotaMailboxStatusCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "underLimit": 155, 
      "warningIssued": 0, 
      "sendProhibited": 0, 
      "sendReceiveProhibited": 0, 
      "indeterminate": 14, 
      "reportDate": "2017-09-01", 
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
