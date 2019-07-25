---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a0fa3f60d981057cf2dc14cbf459cccc8eeb4dfe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894377"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="c470d-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="c470d-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="c470d-105">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="c470d-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="c470d-106">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="c470d-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="c470d-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="c470d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="c470d-108">权限</span><span class="sxs-lookup"><span data-stu-id="c470d-108">Permissions</span></span>

<span data-ttu-id="c470d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c470d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c470d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c470d-111">Permission type</span></span>                        | <span data-ttu-id="c470d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c470d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c470d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c470d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c470d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c470d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c470d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c470d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c470d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c470d-116">Not supported.</span></span>                           |
| <span data-ttu-id="c470d-117">应用</span><span class="sxs-lookup"><span data-stu-id="c470d-117">Application</span></span>                            | <span data-ttu-id="c470d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c470d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c470d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c470d-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c470d-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c470d-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c470d-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="c470d-121">Function parameters</span></span>

<span data-ttu-id="c470d-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c470d-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c470d-123">参数</span><span class="sxs-lookup"><span data-stu-id="c470d-123">Parameter</span></span> | <span data-ttu-id="c470d-124">类型</span><span class="sxs-lookup"><span data-stu-id="c470d-124">Type</span></span>   | <span data-ttu-id="c470d-125">说明</span><span class="sxs-lookup"><span data-stu-id="c470d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c470d-126">period</span><span class="sxs-lookup"><span data-stu-id="c470d-126">period</span></span>    | <span data-ttu-id="c470d-127">string</span><span class="sxs-lookup"><span data-stu-id="c470d-127">string</span></span> | <span data-ttu-id="c470d-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c470d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c470d-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c470d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c470d-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c470d-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c470d-131">必需。</span><span class="sxs-lookup"><span data-stu-id="c470d-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c470d-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="c470d-132">Request headers</span></span>

| <span data-ttu-id="c470d-133">名称</span><span class="sxs-lookup"><span data-stu-id="c470d-133">Name</span></span>          | <span data-ttu-id="c470d-134">说明</span><span class="sxs-lookup"><span data-stu-id="c470d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c470d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c470d-135">Authorization</span></span> | <span data-ttu-id="c470d-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="c470d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c470d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c470d-138">If-None-Match</span></span> | <span data-ttu-id="c470d-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c470d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c470d-140">可选。</span><span class="sxs-lookup"><span data-stu-id="c470d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c470d-141">响应</span><span class="sxs-lookup"><span data-stu-id="c470d-141">Response</span></span>

<span data-ttu-id="c470d-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c470d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c470d-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c470d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c470d-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="c470d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c470d-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="c470d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c470d-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c470d-146">Report Refresh Date</span></span>
- <span data-ttu-id="c470d-147">总计</span><span class="sxs-lookup"><span data-stu-id="c470d-147">Total</span></span>
- <span data-ttu-id="c470d-148">活跃</span><span class="sxs-lookup"><span data-stu-id="c470d-148">Active</span></span>
- <span data-ttu-id="c470d-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="c470d-149">Report Date</span></span>
- <span data-ttu-id="c470d-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="c470d-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c470d-151">示例</span><span class="sxs-lookup"><span data-stu-id="c470d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c470d-152">请求</span><span class="sxs-lookup"><span data-stu-id="c470d-152">Request</span></span>

<span data-ttu-id="c470d-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c470d-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c470d-154">C#</span><span class="sxs-lookup"><span data-stu-id="c470d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c470d-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="c470d-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c470d-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="c470d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c470d-157">Java</span><span class="sxs-lookup"><span data-stu-id="c470d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c470d-158">响应</span><span class="sxs-lookup"><span data-stu-id="c470d-158">Response</span></span>

<span data-ttu-id="c470d-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c470d-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="c470d-160">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c470d-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
