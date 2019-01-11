---
title: 'reportRoot: getMailboxUsageDetail'
description: 获取邮箱使用情况的详细信息。
localization_priority: Normal
ms.openlocfilehash: 09fbb0ce1a4c652d4e24194b36edd790b1ec63f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865154"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="5b507-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5b507-103">reportRoot: getMailboxUsageDetail</span></span>

> <span data-ttu-id="5b507-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b507-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b507-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b507-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b507-106">获取邮箱使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5b507-106">Get details about mailbox usage.</span></span>

> <span data-ttu-id="5b507-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。</span><span class="sxs-lookup"><span data-stu-id="5b507-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b507-108">权限</span><span class="sxs-lookup"><span data-stu-id="5b507-108">Permissions</span></span>

<span data-ttu-id="5b507-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b507-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b507-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b507-111">Permission type</span></span>                        | <span data-ttu-id="5b507-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b507-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b507-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b507-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b507-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b507-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b507-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b507-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b507-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b507-116">Not supported.</span></span>                           |
| <span data-ttu-id="5b507-117">应用</span><span class="sxs-lookup"><span data-stu-id="5b507-117">Application</span></span>                            | <span data-ttu-id="5b507-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b507-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b507-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b507-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5b507-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="5b507-120">Function parameters</span></span>

<span data-ttu-id="5b507-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5b507-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5b507-122">参数</span><span class="sxs-lookup"><span data-stu-id="5b507-122">Parameter</span></span> | <span data-ttu-id="5b507-123">类型</span><span class="sxs-lookup"><span data-stu-id="5b507-123">Type</span></span>   | <span data-ttu-id="5b507-124">说明</span><span class="sxs-lookup"><span data-stu-id="5b507-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b507-125">period</span><span class="sxs-lookup"><span data-stu-id="5b507-125">period</span></span>    | <span data-ttu-id="5b507-126">string</span><span class="sxs-lookup"><span data-stu-id="5b507-126">string</span></span> | <span data-ttu-id="5b507-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5b507-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b507-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5b507-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b507-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5b507-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5b507-130">必需。</span><span class="sxs-lookup"><span data-stu-id="5b507-130">Required.</span></span> |

<span data-ttu-id="5b507-131">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5b507-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5b507-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="5b507-132">The default output type is text/csv.</span></span> <span data-ttu-id="5b507-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="5b507-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b507-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b507-134">Request headers</span></span>

| <span data-ttu-id="5b507-135">名称</span><span class="sxs-lookup"><span data-stu-id="5b507-135">Name</span></span>          | <span data-ttu-id="5b507-136">说明</span><span class="sxs-lookup"><span data-stu-id="5b507-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b507-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b507-137">Authorization</span></span> | <span data-ttu-id="5b507-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b507-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b507-140">响应</span><span class="sxs-lookup"><span data-stu-id="5b507-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5b507-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5b507-141">CSV</span></span>

<span data-ttu-id="5b507-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5b507-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b507-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5b507-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b507-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5b507-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b507-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5b507-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b507-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5b507-146">Report Refresh Date</span></span>
- <span data-ttu-id="5b507-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="5b507-147">User Principal Name</span></span>
- <span data-ttu-id="5b507-148">显示名称</span><span class="sxs-lookup"><span data-stu-id="5b507-148">Display Name</span></span>
- <span data-ttu-id="5b507-149">已删除</span><span class="sxs-lookup"><span data-stu-id="5b507-149">Is Deleted</span></span>
- <span data-ttu-id="5b507-150">删除日期</span><span class="sxs-lookup"><span data-stu-id="5b507-150">Deleted Date</span></span>
- <span data-ttu-id="5b507-151">创建日期</span><span class="sxs-lookup"><span data-stu-id="5b507-151">Created Date</span></span>
- <span data-ttu-id="5b507-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="5b507-152">Last Activity Date</span></span>
- <span data-ttu-id="5b507-153">项数</span><span class="sxs-lookup"><span data-stu-id="5b507-153">Item Count</span></span>
- <span data-ttu-id="5b507-154">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="5b507-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="5b507-155">发出警告配额（字节）</span><span class="sxs-lookup"><span data-stu-id="5b507-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="5b507-156">禁止发送配额（字节）</span><span class="sxs-lookup"><span data-stu-id="5b507-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="5b507-157">禁止发送/接收配额（字节）</span><span class="sxs-lookup"><span data-stu-id="5b507-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="5b507-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="5b507-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5b507-159">JSON</span><span class="sxs-lookup"><span data-stu-id="5b507-159">JSON</span></span>

<span data-ttu-id="5b507-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[mailboxUsageDetail](../resources/mailboxusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="5b507-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="5b507-161">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="5b507-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="5b507-162">示例</span><span class="sxs-lookup"><span data-stu-id="5b507-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5b507-163">CSV</span><span class="sxs-lookup"><span data-stu-id="5b507-163">CSV</span></span>

<span data-ttu-id="5b507-164">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="5b507-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5b507-165">请求</span><span class="sxs-lookup"><span data-stu-id="5b507-165">Request</span></span>

<span data-ttu-id="5b507-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b507-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5b507-167">响应</span><span class="sxs-lookup"><span data-stu-id="5b507-167">Response</span></span>

<span data-ttu-id="5b507-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b507-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b507-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5b507-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="5b507-170">JSON</span><span class="sxs-lookup"><span data-stu-id="5b507-170">JSON</span></span>

<span data-ttu-id="5b507-171">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="5b507-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5b507-172">请求</span><span class="sxs-lookup"><span data-stu-id="5b507-172">Request</span></span>

<span data-ttu-id="5b507-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b507-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5b507-174">响应</span><span class="sxs-lookup"><span data-stu-id="5b507-174">Response</span></span>

<span data-ttu-id="5b507-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b507-175">The following is an example of the response.</span></span>

> <span data-ttu-id="5b507-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5b507-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
      "reportPeriod": "7"
    }
  ]
}
```
