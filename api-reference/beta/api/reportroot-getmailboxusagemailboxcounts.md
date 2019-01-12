---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 925ec8ebd6a0114f78e69c14480bba9d8ca3987f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924095"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="95807-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="95807-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

> <span data-ttu-id="95807-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95807-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95807-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95807-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95807-107">获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。</span><span class="sxs-lookup"><span data-stu-id="95807-107">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="95807-108">如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。</span><span class="sxs-lookup"><span data-stu-id="95807-108">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="95807-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="95807-109">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="95807-110">权限</span><span class="sxs-lookup"><span data-stu-id="95807-110">Permissions</span></span>

<span data-ttu-id="95807-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95807-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95807-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="95807-113">Permission type</span></span>                        | <span data-ttu-id="95807-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95807-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="95807-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95807-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="95807-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="95807-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="95807-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95807-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95807-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="95807-118">Not supported.</span></span>                           |
| <span data-ttu-id="95807-119">应用</span><span class="sxs-lookup"><span data-stu-id="95807-119">Application</span></span>                            | <span data-ttu-id="95807-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="95807-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="95807-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95807-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="95807-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="95807-122">Function parameters</span></span>

<span data-ttu-id="95807-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="95807-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="95807-124">参数</span><span class="sxs-lookup"><span data-stu-id="95807-124">Parameter</span></span> | <span data-ttu-id="95807-125">类型</span><span class="sxs-lookup"><span data-stu-id="95807-125">Type</span></span>   | <span data-ttu-id="95807-126">说明</span><span class="sxs-lookup"><span data-stu-id="95807-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="95807-127">period</span><span class="sxs-lookup"><span data-stu-id="95807-127">period</span></span>    | <span data-ttu-id="95807-128">string</span><span class="sxs-lookup"><span data-stu-id="95807-128">string</span></span> | <span data-ttu-id="95807-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="95807-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="95807-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="95807-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="95807-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="95807-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="95807-132">必需。</span><span class="sxs-lookup"><span data-stu-id="95807-132">Required.</span></span> |

<span data-ttu-id="95807-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="95807-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="95807-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="95807-134">The default output type is text/csv.</span></span> <span data-ttu-id="95807-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="95807-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95807-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="95807-136">Request headers</span></span>

| <span data-ttu-id="95807-137">名称</span><span class="sxs-lookup"><span data-stu-id="95807-137">Name</span></span>          | <span data-ttu-id="95807-138">说明</span><span class="sxs-lookup"><span data-stu-id="95807-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="95807-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="95807-139">Authorization</span></span> | <span data-ttu-id="95807-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95807-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="95807-142">响应</span><span class="sxs-lookup"><span data-stu-id="95807-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="95807-143">CSV</span><span class="sxs-lookup"><span data-stu-id="95807-143">CSV</span></span>

<span data-ttu-id="95807-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="95807-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="95807-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="95807-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="95807-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="95807-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="95807-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="95807-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="95807-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="95807-148">Report Refresh Date</span></span>
- <span data-ttu-id="95807-149">总计</span><span class="sxs-lookup"><span data-stu-id="95807-149">Total</span></span>
- <span data-ttu-id="95807-150">活跃</span><span class="sxs-lookup"><span data-stu-id="95807-150">Active</span></span>
- <span data-ttu-id="95807-151">报表日期</span><span class="sxs-lookup"><span data-stu-id="95807-151">Report Date</span></span>
- <span data-ttu-id="95807-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="95807-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="95807-153">JSON</span><span class="sxs-lookup"><span data-stu-id="95807-153">JSON</span></span>

<span data-ttu-id="95807-154">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="95807-154">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95807-155">示例</span><span class="sxs-lookup"><span data-stu-id="95807-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="95807-156">CSV</span><span class="sxs-lookup"><span data-stu-id="95807-156">CSV</span></span>

<span data-ttu-id="95807-157">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="95807-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="95807-158">请求</span><span class="sxs-lookup"><span data-stu-id="95807-158">Request</span></span>

<span data-ttu-id="95807-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="95807-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="95807-160">响应</span><span class="sxs-lookup"><span data-stu-id="95807-160">Response</span></span>

<span data-ttu-id="95807-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="95807-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="95807-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="95807-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="95807-163">JSON</span><span class="sxs-lookup"><span data-stu-id="95807-163">JSON</span></span>

<span data-ttu-id="95807-164">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="95807-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="95807-165">请求</span><span class="sxs-lookup"><span data-stu-id="95807-165">Request</span></span>

<span data-ttu-id="95807-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="95807-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="95807-167">响应</span><span class="sxs-lookup"><span data-stu-id="95807-167">Response</span></span>

<span data-ttu-id="95807-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="95807-168">The following is an example of the response.</span></span>

> <span data-ttu-id="95807-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="95807-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
