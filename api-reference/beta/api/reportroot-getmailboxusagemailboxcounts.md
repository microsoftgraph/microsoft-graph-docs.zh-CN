---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2e2f75ac030ed62c00d230015e088fa08f616852
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639493"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="f7f47-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="f7f47-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7f47-105">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="f7f47-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="f7f47-106">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="f7f47-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="f7f47-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="f7f47-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7f47-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7f47-108">Permissions</span></span>

<span data-ttu-id="f7f47-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7f47-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7f47-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7f47-111">Permission type</span></span>                        | <span data-ttu-id="f7f47-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7f47-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f7f47-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7f47-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7f47-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7f47-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f7f47-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7f47-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7f47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7f47-116">Not supported.</span></span>                           |
| <span data-ttu-id="f7f47-117">应用</span><span class="sxs-lookup"><span data-stu-id="f7f47-117">Application</span></span>                            | <span data-ttu-id="f7f47-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7f47-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f7f47-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7f47-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f7f47-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="f7f47-120">Function parameters</span></span>

<span data-ttu-id="f7f47-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f7f47-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f7f47-122">参数</span><span class="sxs-lookup"><span data-stu-id="f7f47-122">Parameter</span></span> | <span data-ttu-id="f7f47-123">类型</span><span class="sxs-lookup"><span data-stu-id="f7f47-123">Type</span></span>   | <span data-ttu-id="f7f47-124">说明</span><span class="sxs-lookup"><span data-stu-id="f7f47-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f7f47-125">period</span><span class="sxs-lookup"><span data-stu-id="f7f47-125">period</span></span>    | <span data-ttu-id="f7f47-126">string</span><span class="sxs-lookup"><span data-stu-id="f7f47-126">string</span></span> | <span data-ttu-id="f7f47-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f7f47-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f7f47-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f7f47-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f7f47-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f7f47-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f7f47-130">必需。</span><span class="sxs-lookup"><span data-stu-id="f7f47-130">Required.</span></span> |

<span data-ttu-id="f7f47-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7f47-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f7f47-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="f7f47-132">The default output type is text/csv.</span></span> <span data-ttu-id="f7f47-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="f7f47-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7f47-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7f47-134">Request headers</span></span>

| <span data-ttu-id="f7f47-135">名称</span><span class="sxs-lookup"><span data-stu-id="f7f47-135">Name</span></span>          | <span data-ttu-id="f7f47-136">说明</span><span class="sxs-lookup"><span data-stu-id="f7f47-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f7f47-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7f47-137">Authorization</span></span> | <span data-ttu-id="f7f47-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7f47-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f7f47-140">响应</span><span class="sxs-lookup"><span data-stu-id="f7f47-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f7f47-141">CSV</span><span class="sxs-lookup"><span data-stu-id="f7f47-141">CSV</span></span>

<span data-ttu-id="f7f47-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f7f47-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f7f47-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f7f47-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f7f47-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f7f47-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f7f47-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f7f47-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f7f47-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f7f47-146">Report Refresh Date</span></span>
- <span data-ttu-id="f7f47-147">总计</span><span class="sxs-lookup"><span data-stu-id="f7f47-147">Total</span></span>
- <span data-ttu-id="f7f47-148">活跃</span><span class="sxs-lookup"><span data-stu-id="f7f47-148">Active</span></span>
- <span data-ttu-id="f7f47-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="f7f47-149">Report Date</span></span>
- <span data-ttu-id="f7f47-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="f7f47-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f7f47-151">JSON</span><span class="sxs-lookup"><span data-stu-id="f7f47-151">JSON</span></span>

<span data-ttu-id="f7f47-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="f7f47-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7f47-153">示例</span><span class="sxs-lookup"><span data-stu-id="f7f47-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f7f47-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f7f47-154">CSV</span></span>

<span data-ttu-id="f7f47-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7f47-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f7f47-156">请求</span><span class="sxs-lookup"><span data-stu-id="f7f47-156">Request</span></span>

<span data-ttu-id="f7f47-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7f47-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f7f47-158">响应</span><span class="sxs-lookup"><span data-stu-id="f7f47-158">Response</span></span>

<span data-ttu-id="f7f47-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7f47-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7f47-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f7f47-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7f47-161">语言</span><span class="sxs-lookup"><span data-stu-id="f7f47-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7f47-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7f47-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f7f47-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f7f47-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f7f47-164">JSON</span><span class="sxs-lookup"><span data-stu-id="f7f47-164">JSON</span></span>

<span data-ttu-id="f7f47-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7f47-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f7f47-166">请求</span><span class="sxs-lookup"><span data-stu-id="f7f47-166">Request</span></span>

<span data-ttu-id="f7f47-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7f47-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f7f47-168">响应</span><span class="sxs-lookup"><span data-stu-id="f7f47-168">Response</span></span>

<span data-ttu-id="f7f47-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7f47-169">The following is an example of the response.</span></span>

> <span data-ttu-id="f7f47-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7f47-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7f47-172">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f7f47-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7f47-173">语言</span><span class="sxs-lookup"><span data-stu-id="f7f47-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7f47-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7f47-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagemailboxcounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagemailboxcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
