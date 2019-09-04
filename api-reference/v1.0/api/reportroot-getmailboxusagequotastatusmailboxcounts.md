---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 获取每个配额类别中的用户邮箱数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f682f374e1aa1b7d36a8a49768423e3a64c84dc5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729761"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="16422-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="16422-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="16422-104">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="16422-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="16422-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="16422-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="16422-106">权限</span><span class="sxs-lookup"><span data-stu-id="16422-106">Permissions</span></span>

<span data-ttu-id="16422-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16422-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16422-109">Permission type</span></span>                        | <span data-ttu-id="16422-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16422-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="16422-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16422-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16422-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16422-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="16422-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16422-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16422-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16422-114">Not supported.</span></span>                           |
| <span data-ttu-id="16422-115">应用</span><span class="sxs-lookup"><span data-stu-id="16422-115">Application</span></span>                            | <span data-ttu-id="16422-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16422-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="16422-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16422-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="16422-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="16422-118">Function parameters</span></span>

<span data-ttu-id="16422-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="16422-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="16422-120">参数</span><span class="sxs-lookup"><span data-stu-id="16422-120">Parameter</span></span> | <span data-ttu-id="16422-121">类型</span><span class="sxs-lookup"><span data-stu-id="16422-121">Type</span></span>   | <span data-ttu-id="16422-122">说明</span><span class="sxs-lookup"><span data-stu-id="16422-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="16422-123">period</span><span class="sxs-lookup"><span data-stu-id="16422-123">period</span></span>    | <span data-ttu-id="16422-124">string</span><span class="sxs-lookup"><span data-stu-id="16422-124">string</span></span> | <span data-ttu-id="16422-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="16422-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="16422-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="16422-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="16422-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="16422-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="16422-128">必需。</span><span class="sxs-lookup"><span data-stu-id="16422-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="16422-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="16422-129">Request headers</span></span>

| <span data-ttu-id="16422-130">名称</span><span class="sxs-lookup"><span data-stu-id="16422-130">Name</span></span>          | <span data-ttu-id="16422-131">说明</span><span class="sxs-lookup"><span data-stu-id="16422-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="16422-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="16422-132">Authorization</span></span> | <span data-ttu-id="16422-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="16422-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="16422-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="16422-135">If-None-Match</span></span> | <span data-ttu-id="16422-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="16422-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="16422-137">可选。</span><span class="sxs-lookup"><span data-stu-id="16422-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="16422-138">响应</span><span class="sxs-lookup"><span data-stu-id="16422-138">Response</span></span>

<span data-ttu-id="16422-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="16422-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="16422-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="16422-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="16422-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="16422-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="16422-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="16422-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="16422-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="16422-143">Report Refresh Date</span></span>
- <span data-ttu-id="16422-144">未达限制</span><span class="sxs-lookup"><span data-stu-id="16422-144">Under Limit</span></span>
- <span data-ttu-id="16422-145">已发出警告</span><span class="sxs-lookup"><span data-stu-id="16422-145">Warning Issued</span></span>
- <span data-ttu-id="16422-146">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="16422-146">Send Prohibited</span></span>
- <span data-ttu-id="16422-147">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="16422-147">Send/Receive Prohibited</span></span>
- <span data-ttu-id="16422-148">不确定</span><span class="sxs-lookup"><span data-stu-id="16422-148">Indeterminate</span></span>
- <span data-ttu-id="16422-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="16422-149">Report Date</span></span>
- <span data-ttu-id="16422-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="16422-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="16422-151">示例</span><span class="sxs-lookup"><span data-stu-id="16422-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="16422-152">请求</span><span class="sxs-lookup"><span data-stu-id="16422-152">Request</span></span>

<span data-ttu-id="16422-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16422-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16422-154">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="16422-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16422-155">C#</span><span class="sxs-lookup"><span data-stu-id="16422-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16422-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16422-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16422-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="16422-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="16422-158">Java</span><span class="sxs-lookup"><span data-stu-id="16422-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="16422-159">响应</span><span class="sxs-lookup"><span data-stu-id="16422-159">Response</span></span>

<span data-ttu-id="16422-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16422-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="16422-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="16422-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
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
