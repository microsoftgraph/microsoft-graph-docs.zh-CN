---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: 获取每个配额类别中的用户邮箱数。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d14e494ca29e80397e6c7d8278c74f1753ec2e55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946285"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="07bb1-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="07bb1-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

> <span data-ttu-id="07bb1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="07bb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07bb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07bb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07bb1-106">获取每个配额类别中的用户邮箱数。</span><span class="sxs-lookup"><span data-stu-id="07bb1-106">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="07bb1-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="07bb1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="07bb1-108">权限</span><span class="sxs-lookup"><span data-stu-id="07bb1-108">Permissions</span></span>

<span data-ttu-id="07bb1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07bb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07bb1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07bb1-111">Permission type</span></span>                        | <span data-ttu-id="07bb1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07bb1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="07bb1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07bb1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="07bb1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="07bb1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="07bb1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07bb1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07bb1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07bb1-116">Not supported.</span></span>                           |
| <span data-ttu-id="07bb1-117">应用</span><span class="sxs-lookup"><span data-stu-id="07bb1-117">Application</span></span>                            | <span data-ttu-id="07bb1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="07bb1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="07bb1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07bb1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="07bb1-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="07bb1-120">Function parameters</span></span>

<span data-ttu-id="07bb1-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="07bb1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="07bb1-122">参数</span><span class="sxs-lookup"><span data-stu-id="07bb1-122">Parameter</span></span> | <span data-ttu-id="07bb1-123">类型</span><span class="sxs-lookup"><span data-stu-id="07bb1-123">Type</span></span>   | <span data-ttu-id="07bb1-124">说明</span><span class="sxs-lookup"><span data-stu-id="07bb1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="07bb1-125">period</span><span class="sxs-lookup"><span data-stu-id="07bb1-125">period</span></span>    | <span data-ttu-id="07bb1-126">string</span><span class="sxs-lookup"><span data-stu-id="07bb1-126">string</span></span> | <span data-ttu-id="07bb1-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="07bb1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="07bb1-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="07bb1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="07bb1-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="07bb1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="07bb1-130">必需。</span><span class="sxs-lookup"><span data-stu-id="07bb1-130">Required.</span></span> |

<span data-ttu-id="07bb1-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="07bb1-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="07bb1-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="07bb1-132">The default output type is text/csv.</span></span> <span data-ttu-id="07bb1-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="07bb1-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07bb1-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="07bb1-134">Request headers</span></span>

| <span data-ttu-id="07bb1-135">名称</span><span class="sxs-lookup"><span data-stu-id="07bb1-135">Name</span></span>          | <span data-ttu-id="07bb1-136">说明</span><span class="sxs-lookup"><span data-stu-id="07bb1-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="07bb1-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="07bb1-137">Authorization</span></span> | <span data-ttu-id="07bb1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07bb1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="07bb1-140">响应</span><span class="sxs-lookup"><span data-stu-id="07bb1-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="07bb1-141">CSV</span><span class="sxs-lookup"><span data-stu-id="07bb1-141">CSV</span></span>

<span data-ttu-id="07bb1-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="07bb1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="07bb1-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="07bb1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="07bb1-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="07bb1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="07bb1-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="07bb1-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="07bb1-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="07bb1-146">Report Refresh Date</span></span>
- <span data-ttu-id="07bb1-147">未达限制</span><span class="sxs-lookup"><span data-stu-id="07bb1-147">Under Limit</span></span>
- <span data-ttu-id="07bb1-148">已发出警告</span><span class="sxs-lookup"><span data-stu-id="07bb1-148">Warning Issued</span></span>
- <span data-ttu-id="07bb1-149">已禁止发送</span><span class="sxs-lookup"><span data-stu-id="07bb1-149">Send Prohibited</span></span>
- <span data-ttu-id="07bb1-150">已禁止发送/接收</span><span class="sxs-lookup"><span data-stu-id="07bb1-150">Send/Receive Prohibited</span></span>
- <span data-ttu-id="07bb1-151">不确定</span><span class="sxs-lookup"><span data-stu-id="07bb1-151">Indeterminate</span></span>
- <span data-ttu-id="07bb1-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="07bb1-152">Report Date</span></span>
- <span data-ttu-id="07bb1-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="07bb1-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="07bb1-154">JSON</span><span class="sxs-lookup"><span data-stu-id="07bb1-154">JSON</span></span>

<span data-ttu-id="07bb1-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="07bb1-155">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07bb1-156">示例</span><span class="sxs-lookup"><span data-stu-id="07bb1-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="07bb1-157">CSV</span><span class="sxs-lookup"><span data-stu-id="07bb1-157">CSV</span></span>

<span data-ttu-id="07bb1-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="07bb1-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="07bb1-159">请求</span><span class="sxs-lookup"><span data-stu-id="07bb1-159">Request</span></span>

<span data-ttu-id="07bb1-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07bb1-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="07bb1-161">响应</span><span class="sxs-lookup"><span data-stu-id="07bb1-161">Response</span></span>

<span data-ttu-id="07bb1-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07bb1-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="07bb1-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="07bb1-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="07bb1-164">JSON</span><span class="sxs-lookup"><span data-stu-id="07bb1-164">JSON</span></span>

<span data-ttu-id="07bb1-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="07bb1-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="07bb1-166">请求</span><span class="sxs-lookup"><span data-stu-id="07bb1-166">Request</span></span>

<span data-ttu-id="07bb1-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07bb1-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="07bb1-168">响应</span><span class="sxs-lookup"><span data-stu-id="07bb1-168">Response</span></span>

<span data-ttu-id="07bb1-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07bb1-169">The following is an example of the response.</span></span>

> <span data-ttu-id="07bb1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="07bb1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
