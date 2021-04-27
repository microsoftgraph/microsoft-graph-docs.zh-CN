---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8c885cf85253b8c170d82110bed0170ee82ebdd5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050918"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="7e0be-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="7e0be-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="7e0be-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e0be-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e0be-106">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="7e0be-106">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="7e0be-107">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="7e0be-107">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="7e0be-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="7e0be-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e0be-109">权限</span><span class="sxs-lookup"><span data-stu-id="7e0be-109">Permissions</span></span>

<span data-ttu-id="7e0be-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e0be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e0be-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e0be-112">Permission type</span></span>                        | <span data-ttu-id="7e0be-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e0be-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7e0be-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e0be-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e0be-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e0be-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7e0be-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e0be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e0be-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e0be-117">Not supported.</span></span>                           |
| <span data-ttu-id="7e0be-118">应用</span><span class="sxs-lookup"><span data-stu-id="7e0be-118">Application</span></span>                            | <span data-ttu-id="7e0be-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e0be-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="7e0be-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="7e0be-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7e0be-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="7e0be-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7e0be-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e0be-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7e0be-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="7e0be-123">Function parameters</span></span>

<span data-ttu-id="7e0be-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7e0be-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7e0be-125">参数</span><span class="sxs-lookup"><span data-stu-id="7e0be-125">Parameter</span></span> | <span data-ttu-id="7e0be-126">类型</span><span class="sxs-lookup"><span data-stu-id="7e0be-126">Type</span></span>   | <span data-ttu-id="7e0be-127">说明</span><span class="sxs-lookup"><span data-stu-id="7e0be-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7e0be-128">period</span><span class="sxs-lookup"><span data-stu-id="7e0be-128">period</span></span>    | <span data-ttu-id="7e0be-129">string</span><span class="sxs-lookup"><span data-stu-id="7e0be-129">string</span></span> | <span data-ttu-id="7e0be-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e0be-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7e0be-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7e0be-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7e0be-132">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7e0be-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7e0be-133">必需。</span><span class="sxs-lookup"><span data-stu-id="7e0be-133">Required.</span></span> |

<span data-ttu-id="7e0be-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7e0be-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7e0be-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="7e0be-135">The default output type is text/csv.</span></span> <span data-ttu-id="7e0be-136">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="7e0be-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e0be-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e0be-137">Request headers</span></span>

| <span data-ttu-id="7e0be-138">名称</span><span class="sxs-lookup"><span data-stu-id="7e0be-138">Name</span></span>          | <span data-ttu-id="7e0be-139">说明</span><span class="sxs-lookup"><span data-stu-id="7e0be-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7e0be-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e0be-140">Authorization</span></span> | <span data-ttu-id="7e0be-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e0be-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7e0be-143">响应</span><span class="sxs-lookup"><span data-stu-id="7e0be-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7e0be-144">CSV</span><span class="sxs-lookup"><span data-stu-id="7e0be-144">CSV</span></span>

<span data-ttu-id="7e0be-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7e0be-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7e0be-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7e0be-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7e0be-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7e0be-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7e0be-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7e0be-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7e0be-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7e0be-149">Report Refresh Date</span></span>
- <span data-ttu-id="7e0be-150">总计</span><span class="sxs-lookup"><span data-stu-id="7e0be-150">Total</span></span>
- <span data-ttu-id="7e0be-151">活跃</span><span class="sxs-lookup"><span data-stu-id="7e0be-151">Active</span></span>
- <span data-ttu-id="7e0be-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="7e0be-152">Report Date</span></span>
- <span data-ttu-id="7e0be-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="7e0be-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7e0be-154">JSON</span><span class="sxs-lookup"><span data-stu-id="7e0be-154">JSON</span></span>

<span data-ttu-id="7e0be-155">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7e0be-155">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e0be-156">示例</span><span class="sxs-lookup"><span data-stu-id="7e0be-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7e0be-157">CSV</span><span class="sxs-lookup"><span data-stu-id="7e0be-157">CSV</span></span>

<span data-ttu-id="7e0be-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="7e0be-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7e0be-159">请求</span><span class="sxs-lookup"><span data-stu-id="7e0be-159">Request</span></span>

<span data-ttu-id="7e0be-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e0be-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7e0be-161">响应</span><span class="sxs-lookup"><span data-stu-id="7e0be-161">Response</span></span>

<span data-ttu-id="7e0be-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e0be-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7e0be-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7e0be-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7e0be-164">JSON</span><span class="sxs-lookup"><span data-stu-id="7e0be-164">JSON</span></span>

<span data-ttu-id="7e0be-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7e0be-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7e0be-166">请求</span><span class="sxs-lookup"><span data-stu-id="7e0be-166">Request</span></span>

<span data-ttu-id="7e0be-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e0be-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7e0be-168">响应</span><span class="sxs-lookup"><span data-stu-id="7e0be-168">Response</span></span>

<span data-ttu-id="7e0be-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e0be-169">The following is an example of the response.</span></span>

> <span data-ttu-id="7e0be-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7e0be-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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


