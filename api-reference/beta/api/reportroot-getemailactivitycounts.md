---
title: 'reportRoot: getEmailActivityCounts'
description: 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。
localization_priority: Normal
ms.openlocfilehash: f3ddc2d1b9a11668ee6d90ac2cfb9b07d1d0ce0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873708"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="bccd7-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="bccd7-103">reportRoot: getEmailActivityCounts</span></span>

> <span data-ttu-id="bccd7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bccd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bccd7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bccd7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bccd7-106">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="bccd7-106">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="bccd7-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="bccd7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="bccd7-108">权限</span><span class="sxs-lookup"><span data-stu-id="bccd7-108">Permissions</span></span>

<span data-ttu-id="bccd7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bccd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bccd7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bccd7-111">Permission type</span></span>                        | <span data-ttu-id="bccd7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bccd7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bccd7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bccd7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bccd7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bccd7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bccd7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bccd7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bccd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bccd7-116">Not supported.</span></span>                           |
| <span data-ttu-id="bccd7-117">应用</span><span class="sxs-lookup"><span data-stu-id="bccd7-117">Application</span></span>                            | <span data-ttu-id="bccd7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bccd7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bccd7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bccd7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bccd7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="bccd7-120">Function parameters</span></span>

<span data-ttu-id="bccd7-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bccd7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bccd7-122">参数</span><span class="sxs-lookup"><span data-stu-id="bccd7-122">Parameter</span></span> | <span data-ttu-id="bccd7-123">类型</span><span class="sxs-lookup"><span data-stu-id="bccd7-123">Type</span></span>   | <span data-ttu-id="bccd7-124">说明</span><span class="sxs-lookup"><span data-stu-id="bccd7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bccd7-125">period</span><span class="sxs-lookup"><span data-stu-id="bccd7-125">period</span></span>    | <span data-ttu-id="bccd7-126">string</span><span class="sxs-lookup"><span data-stu-id="bccd7-126">string</span></span> | <span data-ttu-id="bccd7-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bccd7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bccd7-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bccd7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bccd7-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bccd7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bccd7-130">必需。</span><span class="sxs-lookup"><span data-stu-id="bccd7-130">Required.</span></span> |

<span data-ttu-id="bccd7-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bccd7-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bccd7-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="bccd7-132">The default output type is text/csv.</span></span> <span data-ttu-id="bccd7-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="bccd7-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bccd7-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="bccd7-134">Request headers</span></span>

| <span data-ttu-id="bccd7-135">名称</span><span class="sxs-lookup"><span data-stu-id="bccd7-135">Name</span></span>          | <span data-ttu-id="bccd7-136">说明</span><span class="sxs-lookup"><span data-stu-id="bccd7-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bccd7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bccd7-137">Authorization</span></span> | <span data-ttu-id="bccd7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bccd7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bccd7-140">响应</span><span class="sxs-lookup"><span data-stu-id="bccd7-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bccd7-141">CSV</span><span class="sxs-lookup"><span data-stu-id="bccd7-141">CSV</span></span>

<span data-ttu-id="bccd7-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bccd7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bccd7-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bccd7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bccd7-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bccd7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bccd7-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bccd7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bccd7-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bccd7-146">Report Refresh Date</span></span>
- <span data-ttu-id="bccd7-147">已发送</span><span class="sxs-lookup"><span data-stu-id="bccd7-147">Send</span></span>
- <span data-ttu-id="bccd7-148">已接收</span><span class="sxs-lookup"><span data-stu-id="bccd7-148">Receive</span></span>
- <span data-ttu-id="bccd7-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="bccd7-149">Read</span></span>
- <span data-ttu-id="bccd7-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="bccd7-150">Report Date</span></span>
- <span data-ttu-id="bccd7-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="bccd7-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bccd7-152">JSON</span><span class="sxs-lookup"><span data-stu-id="bccd7-152">JSON</span></span>

<span data-ttu-id="bccd7-153">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[emailActivitySummary](../resources/emailactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="bccd7-153">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bccd7-154">示例</span><span class="sxs-lookup"><span data-stu-id="bccd7-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bccd7-155">CSV</span><span class="sxs-lookup"><span data-stu-id="bccd7-155">CSV</span></span>

<span data-ttu-id="bccd7-156">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="bccd7-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bccd7-157">请求</span><span class="sxs-lookup"><span data-stu-id="bccd7-157">Request</span></span>

<span data-ttu-id="bccd7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bccd7-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bccd7-159">响应</span><span class="sxs-lookup"><span data-stu-id="bccd7-159">Response</span></span>

<span data-ttu-id="bccd7-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bccd7-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bccd7-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bccd7-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="bccd7-162">JSON</span><span class="sxs-lookup"><span data-stu-id="bccd7-162">JSON</span></span>

<span data-ttu-id="bccd7-163">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="bccd7-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bccd7-164">请求</span><span class="sxs-lookup"><span data-stu-id="bccd7-164">Request</span></span>

<span data-ttu-id="bccd7-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bccd7-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bccd7-166">响应</span><span class="sxs-lookup"><span data-stu-id="bccd7-166">Response</span></span>

<span data-ttu-id="bccd7-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bccd7-167">The following is an example of the response.</span></span>

> <span data-ttu-id="bccd7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bccd7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
