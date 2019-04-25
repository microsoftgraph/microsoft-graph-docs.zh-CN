---
title: 'reportRoot: getEmailActivityCounts'
description: 可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5f3f5c1c9e9caebe1217a18597778c9324195f03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546155"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="13467-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="13467-103">reportRoot: getEmailActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13467-104">可便于了解组织中的电子邮件活动趋势（如已发送、已阅读和已接收的电子邮件数）。</span><span class="sxs-lookup"><span data-stu-id="13467-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="13467-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="13467-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="13467-106">权限</span><span class="sxs-lookup"><span data-stu-id="13467-106">Permissions</span></span>

<span data-ttu-id="13467-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13467-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="13467-109">Permission type</span></span>                        | <span data-ttu-id="13467-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13467-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="13467-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13467-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13467-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="13467-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="13467-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13467-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13467-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="13467-114">Not supported.</span></span>                           |
| <span data-ttu-id="13467-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="13467-115">Application</span></span>                            | <span data-ttu-id="13467-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="13467-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="13467-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13467-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="13467-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="13467-118">Function parameters</span></span>

<span data-ttu-id="13467-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="13467-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="13467-120">参数</span><span class="sxs-lookup"><span data-stu-id="13467-120">Parameter</span></span> | <span data-ttu-id="13467-121">类型</span><span class="sxs-lookup"><span data-stu-id="13467-121">Type</span></span>   | <span data-ttu-id="13467-122">说明</span><span class="sxs-lookup"><span data-stu-id="13467-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="13467-123">period</span><span class="sxs-lookup"><span data-stu-id="13467-123">period</span></span>    | <span data-ttu-id="13467-124">string</span><span class="sxs-lookup"><span data-stu-id="13467-124">string</span></span> | <span data-ttu-id="13467-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="13467-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="13467-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="13467-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="13467-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="13467-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="13467-128">必需。</span><span class="sxs-lookup"><span data-stu-id="13467-128">Required.</span></span> |

<span data-ttu-id="13467-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13467-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="13467-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="13467-130">The default output type is text/csv.</span></span> <span data-ttu-id="13467-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="13467-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13467-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="13467-132">Request headers</span></span>

| <span data-ttu-id="13467-133">名称</span><span class="sxs-lookup"><span data-stu-id="13467-133">Name</span></span>          | <span data-ttu-id="13467-134">说明</span><span class="sxs-lookup"><span data-stu-id="13467-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="13467-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="13467-135">Authorization</span></span> | <span data-ttu-id="13467-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13467-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="13467-138">响应</span><span class="sxs-lookup"><span data-stu-id="13467-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="13467-139">CSV</span><span class="sxs-lookup"><span data-stu-id="13467-139">CSV</span></span>

<span data-ttu-id="13467-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="13467-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="13467-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="13467-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="13467-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="13467-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="13467-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="13467-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="13467-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="13467-144">Report Refresh Date</span></span>
- <span data-ttu-id="13467-145">已发送</span><span class="sxs-lookup"><span data-stu-id="13467-145">Send</span></span>
- <span data-ttu-id="13467-146">已接收</span><span class="sxs-lookup"><span data-stu-id="13467-146">Receive</span></span>
- <span data-ttu-id="13467-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="13467-147">Read</span></span>
- <span data-ttu-id="13467-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="13467-148">Report Date</span></span>
- <span data-ttu-id="13467-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="13467-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="13467-150">JSON</span><span class="sxs-lookup"><span data-stu-id="13467-150">JSON</span></span>

<span data-ttu-id="13467-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailActivitySummary](../resources/emailactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="13467-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13467-152">示例</span><span class="sxs-lookup"><span data-stu-id="13467-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="13467-153">CSV</span><span class="sxs-lookup"><span data-stu-id="13467-153">CSV</span></span>

<span data-ttu-id="13467-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="13467-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="13467-155">请求</span><span class="sxs-lookup"><span data-stu-id="13467-155">Request</span></span>

<span data-ttu-id="13467-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13467-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="13467-157">响应</span><span class="sxs-lookup"><span data-stu-id="13467-157">Response</span></span>

<span data-ttu-id="13467-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13467-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="13467-159">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="13467-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="13467-160">JSON</span><span class="sxs-lookup"><span data-stu-id="13467-160">JSON</span></span>

<span data-ttu-id="13467-161">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="13467-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="13467-162">请求</span><span class="sxs-lookup"><span data-stu-id="13467-162">Request</span></span>

<span data-ttu-id="13467-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="13467-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="13467-164">响应</span><span class="sxs-lookup"><span data-stu-id="13467-164">Response</span></span>

<span data-ttu-id="13467-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="13467-165">The following is an example of the response.</span></span>

> <span data-ttu-id="13467-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13467-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
