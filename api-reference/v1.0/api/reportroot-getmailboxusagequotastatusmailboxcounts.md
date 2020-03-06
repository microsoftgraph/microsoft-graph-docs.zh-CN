---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 获取每个配额类别中的用户邮箱数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ad098d931fbb75178ce8cbfc3b9e97dc30c6f2ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510387"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="f9afb-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="f9afb-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="f9afb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9afb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9afb-105">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="f9afb-105">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="f9afb-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="f9afb-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9afb-107">权限</span><span class="sxs-lookup"><span data-stu-id="f9afb-107">Permissions</span></span>

<span data-ttu-id="f9afb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9afb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9afb-110">Permission type</span></span>                        | <span data-ttu-id="f9afb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9afb-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f9afb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9afb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9afb-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9afb-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f9afb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9afb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9afb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9afb-115">Not supported.</span></span>                           |
| <span data-ttu-id="f9afb-116">应用</span><span class="sxs-lookup"><span data-stu-id="f9afb-116">Application</span></span>                            | <span data-ttu-id="f9afb-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9afb-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="f9afb-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f9afb-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f9afb-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="f9afb-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f9afb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9afb-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f9afb-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="f9afb-121">Function parameters</span></span>

<span data-ttu-id="f9afb-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f9afb-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f9afb-123">参数</span><span class="sxs-lookup"><span data-stu-id="f9afb-123">Parameter</span></span> | <span data-ttu-id="f9afb-124">类型</span><span class="sxs-lookup"><span data-stu-id="f9afb-124">Type</span></span>   | <span data-ttu-id="f9afb-125">说明</span><span class="sxs-lookup"><span data-stu-id="f9afb-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f9afb-126">period</span><span class="sxs-lookup"><span data-stu-id="f9afb-126">period</span></span>    | <span data-ttu-id="f9afb-127">string</span><span class="sxs-lookup"><span data-stu-id="f9afb-127">string</span></span> | <span data-ttu-id="f9afb-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f9afb-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f9afb-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f9afb-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f9afb-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f9afb-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f9afb-131">必需。</span><span class="sxs-lookup"><span data-stu-id="f9afb-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f9afb-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9afb-132">Request headers</span></span>

| <span data-ttu-id="f9afb-133">名称</span><span class="sxs-lookup"><span data-stu-id="f9afb-133">Name</span></span>          | <span data-ttu-id="f9afb-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9afb-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f9afb-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9afb-135">Authorization</span></span> | <span data-ttu-id="f9afb-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9afb-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f9afb-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f9afb-138">If-None-Match</span></span> | <span data-ttu-id="f9afb-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f9afb-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f9afb-140">可选。</span><span class="sxs-lookup"><span data-stu-id="f9afb-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f9afb-141">响应</span><span class="sxs-lookup"><span data-stu-id="f9afb-141">Response</span></span>

<span data-ttu-id="f9afb-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f9afb-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f9afb-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f9afb-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f9afb-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f9afb-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f9afb-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f9afb-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f9afb-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f9afb-146">Report Refresh Date</span></span>
- <span data-ttu-id="f9afb-147">未达限制</span><span class="sxs-lookup"><span data-stu-id="f9afb-147">Under Limit</span></span>
- <span data-ttu-id="f9afb-148">已发出警告</span><span class="sxs-lookup"><span data-stu-id="f9afb-148">Warning Issued</span></span>
- <span data-ttu-id="f9afb-149">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="f9afb-149">Send Prohibited</span></span>
- <span data-ttu-id="f9afb-150">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="f9afb-150">Send/Receive Prohibited</span></span>
- <span data-ttu-id="f9afb-151">不确定</span><span class="sxs-lookup"><span data-stu-id="f9afb-151">Indeterminate</span></span>
- <span data-ttu-id="f9afb-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="f9afb-152">Report Date</span></span>
- <span data-ttu-id="f9afb-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="f9afb-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f9afb-154">示例</span><span class="sxs-lookup"><span data-stu-id="f9afb-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f9afb-155">请求</span><span class="sxs-lookup"><span data-stu-id="f9afb-155">Request</span></span>

<span data-ttu-id="f9afb-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f9afb-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9afb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9afb-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="f9afb-158">C#</span><span class="sxs-lookup"><span data-stu-id="f9afb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9afb-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9afb-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9afb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9afb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9afb-161">Java</span><span class="sxs-lookup"><span data-stu-id="f9afb-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f9afb-162">响应</span><span class="sxs-lookup"><span data-stu-id="f9afb-162">Response</span></span>

<span data-ttu-id="f9afb-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f9afb-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="f9afb-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f9afb-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
