---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: 获取跨组工作负载的组活动数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 72c879af55f8608dd8f5cd2f1086f8469aacb651
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545903"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="6db78-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6db78-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db78-104">获取跨组工作负载的组活动数。</span><span class="sxs-lookup"><span data-stu-id="6db78-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="6db78-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="6db78-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="6db78-106">权限</span><span class="sxs-lookup"><span data-stu-id="6db78-106">Permissions</span></span>

<span data-ttu-id="6db78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6db78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6db78-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6db78-109">Permission type</span></span>                        | <span data-ttu-id="6db78-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6db78-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6db78-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6db78-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6db78-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db78-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6db78-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6db78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db78-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6db78-114">Not supported.</span></span>                           |
| <span data-ttu-id="6db78-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6db78-115">Application</span></span>                            | <span data-ttu-id="6db78-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db78-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6db78-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6db78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6db78-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6db78-118">Function parameters</span></span>

<span data-ttu-id="6db78-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6db78-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6db78-120">参数</span><span class="sxs-lookup"><span data-stu-id="6db78-120">Parameter</span></span> | <span data-ttu-id="6db78-121">类型</span><span class="sxs-lookup"><span data-stu-id="6db78-121">Type</span></span>   | <span data-ttu-id="6db78-122">说明</span><span class="sxs-lookup"><span data-stu-id="6db78-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6db78-123">period</span><span class="sxs-lookup"><span data-stu-id="6db78-123">period</span></span>    | <span data-ttu-id="6db78-124">string</span><span class="sxs-lookup"><span data-stu-id="6db78-124">string</span></span> | <span data-ttu-id="6db78-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6db78-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6db78-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6db78-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6db78-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6db78-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6db78-128">必需。</span><span class="sxs-lookup"><span data-stu-id="6db78-128">Required.</span></span> |

<span data-ttu-id="6db78-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6db78-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6db78-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="6db78-130">The default output type is text/csv.</span></span> <span data-ttu-id="6db78-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="6db78-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6db78-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="6db78-132">Request headers</span></span>

| <span data-ttu-id="6db78-133">名称</span><span class="sxs-lookup"><span data-stu-id="6db78-133">Name</span></span>          | <span data-ttu-id="6db78-134">说明</span><span class="sxs-lookup"><span data-stu-id="6db78-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6db78-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="6db78-135">Authorization</span></span> | <span data-ttu-id="6db78-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6db78-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6db78-138">响应</span><span class="sxs-lookup"><span data-stu-id="6db78-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6db78-139">CSV</span><span class="sxs-lookup"><span data-stu-id="6db78-139">CSV</span></span>

<span data-ttu-id="6db78-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6db78-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6db78-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6db78-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6db78-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6db78-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6db78-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6db78-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6db78-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6db78-144">Report Refresh Date</span></span>
- <span data-ttu-id="6db78-145">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="6db78-145">Exchange Emails Received</span></span>
- <span data-ttu-id="6db78-146">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="6db78-147">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-147">Yammer Messages Read</span></span>
- <span data-ttu-id="6db78-148">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="6db78-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="6db78-149">Report Date</span></span>
- <span data-ttu-id="6db78-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="6db78-150">Report Period</span></span>

<span data-ttu-id="6db78-151">由世纪互联运营的 Microsoft Graph 中国不支持以下各列:</span><span class="sxs-lookup"><span data-stu-id="6db78-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6db78-152">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="6db78-153">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-153">Yammer Messages Read</span></span>
- <span data-ttu-id="6db78-154">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="6db78-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="6db78-155">JSON</span><span class="sxs-lookup"><span data-stu-id="6db78-155">JSON</span></span>

<span data-ttu-id="6db78-156">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6db78-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="6db78-157">由世纪互联运营的 Microsoft Graph 中国不支持**[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** 对象中的以下属性:</span><span class="sxs-lookup"><span data-stu-id="6db78-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6db78-158">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="6db78-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="6db78-159">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="6db78-159">yammerMessagesRead</span></span>
- <span data-ttu-id="6db78-160">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="6db78-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="6db78-161">示例</span><span class="sxs-lookup"><span data-stu-id="6db78-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6db78-162">CSV</span><span class="sxs-lookup"><span data-stu-id="6db78-162">CSV</span></span>

<span data-ttu-id="6db78-163">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="6db78-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6db78-164">请求</span><span class="sxs-lookup"><span data-stu-id="6db78-164">Request</span></span>

<span data-ttu-id="6db78-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6db78-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6db78-166">响应</span><span class="sxs-lookup"><span data-stu-id="6db78-166">Response</span></span>

<span data-ttu-id="6db78-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6db78-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6db78-168">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6db78-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6db78-169">JSON</span><span class="sxs-lookup"><span data-stu-id="6db78-169">JSON</span></span>

<span data-ttu-id="6db78-170">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6db78-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6db78-171">请求</span><span class="sxs-lookup"><span data-stu-id="6db78-171">Request</span></span>

<span data-ttu-id="6db78-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6db78-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6db78-173">响应</span><span class="sxs-lookup"><span data-stu-id="6db78-173">Response</span></span>

<span data-ttu-id="6db78-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6db78-174">The following is an example of the response.</span></span>

> <span data-ttu-id="6db78-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6db78-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
