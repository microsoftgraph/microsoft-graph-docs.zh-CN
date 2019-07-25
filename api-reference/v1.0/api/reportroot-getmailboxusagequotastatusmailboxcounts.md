---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 获取每个配额类别中的用户邮箱数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5d57690bfd12b9c54f851f21cd851d84a843cc6d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894355"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="71bf8-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="71bf8-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="71bf8-104">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="71bf8-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="71bf8-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="71bf8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="71bf8-106">权限</span><span class="sxs-lookup"><span data-stu-id="71bf8-106">Permissions</span></span>

<span data-ttu-id="71bf8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71bf8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71bf8-109">Permission type</span></span>                        | <span data-ttu-id="71bf8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71bf8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="71bf8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71bf8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71bf8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71bf8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="71bf8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71bf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bf8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="71bf8-114">Not supported.</span></span>                           |
| <span data-ttu-id="71bf8-115">应用</span><span class="sxs-lookup"><span data-stu-id="71bf8-115">Application</span></span>                            | <span data-ttu-id="71bf8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71bf8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="71bf8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71bf8-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71bf8-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="71bf8-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="71bf8-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="71bf8-119">Function parameters</span></span>

<span data-ttu-id="71bf8-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="71bf8-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="71bf8-121">参数</span><span class="sxs-lookup"><span data-stu-id="71bf8-121">Parameter</span></span> | <span data-ttu-id="71bf8-122">类型</span><span class="sxs-lookup"><span data-stu-id="71bf8-122">Type</span></span>   | <span data-ttu-id="71bf8-123">说明</span><span class="sxs-lookup"><span data-stu-id="71bf8-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="71bf8-124">period</span><span class="sxs-lookup"><span data-stu-id="71bf8-124">period</span></span>    | <span data-ttu-id="71bf8-125">string</span><span class="sxs-lookup"><span data-stu-id="71bf8-125">string</span></span> | <span data-ttu-id="71bf8-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="71bf8-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="71bf8-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="71bf8-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="71bf8-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="71bf8-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="71bf8-129">必需。</span><span class="sxs-lookup"><span data-stu-id="71bf8-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="71bf8-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="71bf8-130">Request headers</span></span>

| <span data-ttu-id="71bf8-131">名称</span><span class="sxs-lookup"><span data-stu-id="71bf8-131">Name</span></span>          | <span data-ttu-id="71bf8-132">说明</span><span class="sxs-lookup"><span data-stu-id="71bf8-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="71bf8-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bf8-133">Authorization</span></span> | <span data-ttu-id="71bf8-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="71bf8-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="71bf8-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="71bf8-136">If-None-Match</span></span> | <span data-ttu-id="71bf8-137">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="71bf8-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="71bf8-138">可选。</span><span class="sxs-lookup"><span data-stu-id="71bf8-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="71bf8-139">响应</span><span class="sxs-lookup"><span data-stu-id="71bf8-139">Response</span></span>

<span data-ttu-id="71bf8-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="71bf8-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="71bf8-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="71bf8-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="71bf8-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="71bf8-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="71bf8-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="71bf8-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="71bf8-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="71bf8-144">Report Refresh Date</span></span>
- <span data-ttu-id="71bf8-145">未达限制</span><span class="sxs-lookup"><span data-stu-id="71bf8-145">Under Limit</span></span>
- <span data-ttu-id="71bf8-146">已发出警告</span><span class="sxs-lookup"><span data-stu-id="71bf8-146">Warning Issued</span></span>
- <span data-ttu-id="71bf8-147">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="71bf8-147">Send Prohibited</span></span>
- <span data-ttu-id="71bf8-148">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="71bf8-148">Send/Receive Prohibited</span></span>
- <span data-ttu-id="71bf8-149">不确定</span><span class="sxs-lookup"><span data-stu-id="71bf8-149">Indeterminate</span></span>
- <span data-ttu-id="71bf8-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="71bf8-150">Report Date</span></span>
- <span data-ttu-id="71bf8-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="71bf8-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="71bf8-152">示例</span><span class="sxs-lookup"><span data-stu-id="71bf8-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="71bf8-153">请求</span><span class="sxs-lookup"><span data-stu-id="71bf8-153">Request</span></span>

<span data-ttu-id="71bf8-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71bf8-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71bf8-155">C#</span><span class="sxs-lookup"><span data-stu-id="71bf8-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71bf8-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="71bf8-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71bf8-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="71bf8-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="71bf8-158">Java</span><span class="sxs-lookup"><span data-stu-id="71bf8-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71bf8-159">响应</span><span class="sxs-lookup"><span data-stu-id="71bf8-159">Response</span></span>

<span data-ttu-id="71bf8-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71bf8-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="71bf8-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="71bf8-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
