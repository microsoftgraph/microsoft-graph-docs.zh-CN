---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7b18680a9fa2f47b9d7c2dceac7a64206b372c22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545770"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="cedb7-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="cedb7-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cedb7-105">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="cedb7-105">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="cedb7-106">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="cedb7-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="cedb7-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="cedb7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="cedb7-108">权限</span><span class="sxs-lookup"><span data-stu-id="cedb7-108">Permissions</span></span>

<span data-ttu-id="cedb7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cedb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cedb7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cedb7-111">Permission type</span></span>                        | <span data-ttu-id="cedb7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cedb7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cedb7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cedb7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cedb7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cedb7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cedb7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cedb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cedb7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cedb7-116">Not supported.</span></span>                           |
| <span data-ttu-id="cedb7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cedb7-117">Application</span></span>                            | <span data-ttu-id="cedb7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cedb7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cedb7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cedb7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cedb7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="cedb7-120">Function parameters</span></span>

<span data-ttu-id="cedb7-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="cedb7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cedb7-122">参数</span><span class="sxs-lookup"><span data-stu-id="cedb7-122">Parameter</span></span> | <span data-ttu-id="cedb7-123">类型</span><span class="sxs-lookup"><span data-stu-id="cedb7-123">Type</span></span>   | <span data-ttu-id="cedb7-124">说明</span><span class="sxs-lookup"><span data-stu-id="cedb7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cedb7-125">period</span><span class="sxs-lookup"><span data-stu-id="cedb7-125">period</span></span>    | <span data-ttu-id="cedb7-126">string</span><span class="sxs-lookup"><span data-stu-id="cedb7-126">string</span></span> | <span data-ttu-id="cedb7-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cedb7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cedb7-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="cedb7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cedb7-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="cedb7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cedb7-130">必需。</span><span class="sxs-lookup"><span data-stu-id="cedb7-130">Required.</span></span> |

<span data-ttu-id="cedb7-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cedb7-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cedb7-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="cedb7-132">The default output type is text/csv.</span></span> <span data-ttu-id="cedb7-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="cedb7-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cedb7-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="cedb7-134">Request headers</span></span>

| <span data-ttu-id="cedb7-135">名称</span><span class="sxs-lookup"><span data-stu-id="cedb7-135">Name</span></span>          | <span data-ttu-id="cedb7-136">说明</span><span class="sxs-lookup"><span data-stu-id="cedb7-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cedb7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="cedb7-137">Authorization</span></span> | <span data-ttu-id="cedb7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cedb7-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cedb7-140">响应</span><span class="sxs-lookup"><span data-stu-id="cedb7-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cedb7-141">CSV</span><span class="sxs-lookup"><span data-stu-id="cedb7-141">CSV</span></span>

<span data-ttu-id="cedb7-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cedb7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cedb7-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="cedb7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cedb7-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="cedb7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cedb7-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="cedb7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cedb7-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="cedb7-146">Report Refresh Date</span></span>
- <span data-ttu-id="cedb7-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="cedb7-147">Report Date</span></span>
- <span data-ttu-id="cedb7-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="cedb7-148">Report Period</span></span>
- <span data-ttu-id="cedb7-149">对等</span><span class="sxs-lookup"><span data-stu-id="cedb7-149">Peer-to-peer</span></span>
- <span data-ttu-id="cedb7-150">组织</span><span class="sxs-lookup"><span data-stu-id="cedb7-150">Organized</span></span>
- <span data-ttu-id="cedb7-151">参与</span><span class="sxs-lookup"><span data-stu-id="cedb7-151">Participated</span></span>

### <a name="json"></a><span data-ttu-id="cedb7-152">JSON</span><span class="sxs-lookup"><span data-stu-id="cedb7-152">JSON</span></span>

<span data-ttu-id="cedb7-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="cedb7-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedb7-154">示例</span><span class="sxs-lookup"><span data-stu-id="cedb7-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cedb7-155">CSV</span><span class="sxs-lookup"><span data-stu-id="cedb7-155">CSV</span></span>

<span data-ttu-id="cedb7-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="cedb7-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cedb7-157">请求</span><span class="sxs-lookup"><span data-stu-id="cedb7-157">Request</span></span>

<span data-ttu-id="cedb7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cedb7-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cedb7-159">响应</span><span class="sxs-lookup"><span data-stu-id="cedb7-159">Response</span></span>

<span data-ttu-id="cedb7-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cedb7-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cedb7-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="cedb7-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="cedb7-162">JSON</span><span class="sxs-lookup"><span data-stu-id="cedb7-162">JSON</span></span>

<span data-ttu-id="cedb7-163">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="cedb7-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cedb7-164">请求</span><span class="sxs-lookup"><span data-stu-id="cedb7-164">Request</span></span>

<span data-ttu-id="cedb7-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cedb7-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cedb7-166">响应</span><span class="sxs-lookup"><span data-stu-id="cedb7-166">Response</span></span>

<span data-ttu-id="cedb7-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cedb7-167">The following is an example of the response.</span></span>

> <span data-ttu-id="cedb7-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cedb7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityCounts)", 
  "value": [
    {
      "peerToPeer": 3436, 
      "organized": 58, 
      "participated": 209, 
      "reportRefreshDate": "2017-09-01", 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
