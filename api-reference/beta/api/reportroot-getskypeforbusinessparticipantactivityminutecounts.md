---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: 获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。 会议会话类型包括音频/视频。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f4cc8e2dfeb73425142785da753eff1577ab8fbb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411233"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="e1a3b-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e1a3b-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a3b-105">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="e1a3b-106">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="e1a3b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1a3b-108">权限</span><span class="sxs-lookup"><span data-stu-id="e1a3b-108">Permissions</span></span>

<span data-ttu-id="e1a3b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1a3b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1a3b-111">Permission type</span></span>                        | <span data-ttu-id="e1a3b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1a3b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e1a3b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1a3b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1a3b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1a3b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e1a3b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1a3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a3b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-116">Not supported.</span></span>                           |
| <span data-ttu-id="e1a3b-117">应用</span><span class="sxs-lookup"><span data-stu-id="e1a3b-117">Application</span></span>                            | <span data-ttu-id="e1a3b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1a3b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e1a3b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1a3b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e1a3b-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="e1a3b-120">Function parameters</span></span>

<span data-ttu-id="e1a3b-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e1a3b-122">参数</span><span class="sxs-lookup"><span data-stu-id="e1a3b-122">Parameter</span></span> | <span data-ttu-id="e1a3b-123">类型</span><span class="sxs-lookup"><span data-stu-id="e1a3b-123">Type</span></span>   | <span data-ttu-id="e1a3b-124">说明</span><span class="sxs-lookup"><span data-stu-id="e1a3b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e1a3b-125">period</span><span class="sxs-lookup"><span data-stu-id="e1a3b-125">period</span></span>    | <span data-ttu-id="e1a3b-126">string</span><span class="sxs-lookup"><span data-stu-id="e1a3b-126">string</span></span> | <span data-ttu-id="e1a3b-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e1a3b-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e1a3b-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e1a3b-130">必需。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-130">Required.</span></span> |

<span data-ttu-id="e1a3b-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e1a3b-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-132">The default output type is text/csv.</span></span> <span data-ttu-id="e1a3b-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1a3b-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1a3b-134">Request headers</span></span>

| <span data-ttu-id="e1a3b-135">名称</span><span class="sxs-lookup"><span data-stu-id="e1a3b-135">Name</span></span>          | <span data-ttu-id="e1a3b-136">说明</span><span class="sxs-lookup"><span data-stu-id="e1a3b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e1a3b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1a3b-137">Authorization</span></span> | <span data-ttu-id="e1a3b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e1a3b-140">响应</span><span class="sxs-lookup"><span data-stu-id="e1a3b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e1a3b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e1a3b-141">CSV</span></span>

<span data-ttu-id="e1a3b-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e1a3b-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e1a3b-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e1a3b-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e1a3b-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e1a3b-146">Report Refresh Date</span></span>
- <span data-ttu-id="e1a3b-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="e1a3b-147">Report Date</span></span>
- <span data-ttu-id="e1a3b-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="e1a3b-148">Report Period</span></span>
- <span data-ttu-id="e1a3b-149">音频/视频</span><span class="sxs-lookup"><span data-stu-id="e1a3b-149">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="e1a3b-150">JSON</span><span class="sxs-lookup"><span data-stu-id="e1a3b-150">JSON</span></span>

<span data-ttu-id="e1a3b-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-151">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1a3b-152">示例</span><span class="sxs-lookup"><span data-stu-id="e1a3b-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e1a3b-153">CSV</span><span class="sxs-lookup"><span data-stu-id="e1a3b-153">CSV</span></span>

<span data-ttu-id="e1a3b-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e1a3b-155">请求</span><span class="sxs-lookup"><span data-stu-id="e1a3b-155">Request</span></span>

<span data-ttu-id="e1a3b-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e1a3b-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e1a3b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1a3b-158">C#</span><span class="sxs-lookup"><span data-stu-id="e1a3b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1a3b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1a3b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1a3b-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="e1a3b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1a3b-161">响应</span><span class="sxs-lookup"><span data-stu-id="e1a3b-161">Response</span></span>

<span data-ttu-id="e1a3b-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e1a3b-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="e1a3b-164">JSON</span><span class="sxs-lookup"><span data-stu-id="e1a3b-164">JSON</span></span>

<span data-ttu-id="e1a3b-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e1a3b-166">请求</span><span class="sxs-lookup"><span data-stu-id="e1a3b-166">Request</span></span>

<span data-ttu-id="e1a3b-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e1a3b-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e1a3b-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1a3b-169">C#</span><span class="sxs-lookup"><span data-stu-id="e1a3b-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1a3b-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1a3b-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1a3b-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="e1a3b-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e1a3b-172">响应</span><span class="sxs-lookup"><span data-stu-id="e1a3b-172">Response</span></span>

<span data-ttu-id="e1a3b-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-173">The following is an example of the response.</span></span>

> <span data-ttu-id="e1a3b-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e1a3b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
      "reportRefreshDate": "2017-09-01", 
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
