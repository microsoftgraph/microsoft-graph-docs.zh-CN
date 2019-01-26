---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 15734e15cf13cbbc03fd136d51bbdf9f4ac13ba0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573716"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="2b55a-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2b55a-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b55a-105">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="2b55a-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="2b55a-106">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="2b55a-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="2b55a-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="2b55a-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b55a-108">权限</span><span class="sxs-lookup"><span data-stu-id="2b55a-108">Permissions</span></span>

<span data-ttu-id="2b55a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b55a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b55a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b55a-111">Permission type</span></span>                        | <span data-ttu-id="2b55a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b55a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2b55a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b55a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b55a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b55a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2b55a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b55a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b55a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b55a-116">Not supported.</span></span>                           |
| <span data-ttu-id="2b55a-117">应用</span><span class="sxs-lookup"><span data-stu-id="2b55a-117">Application</span></span>                            | <span data-ttu-id="2b55a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b55a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2b55a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b55a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2b55a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="2b55a-120">Function parameters</span></span>

<span data-ttu-id="2b55a-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2b55a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2b55a-122">参数</span><span class="sxs-lookup"><span data-stu-id="2b55a-122">Parameter</span></span> | <span data-ttu-id="2b55a-123">类型</span><span class="sxs-lookup"><span data-stu-id="2b55a-123">Type</span></span>   | <span data-ttu-id="2b55a-124">说明</span><span class="sxs-lookup"><span data-stu-id="2b55a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2b55a-125">period</span><span class="sxs-lookup"><span data-stu-id="2b55a-125">period</span></span>    | <span data-ttu-id="2b55a-126">string</span><span class="sxs-lookup"><span data-stu-id="2b55a-126">string</span></span> | <span data-ttu-id="2b55a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2b55a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2b55a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2b55a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2b55a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2b55a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2b55a-130">必需。</span><span class="sxs-lookup"><span data-stu-id="2b55a-130">Required.</span></span> |

<span data-ttu-id="2b55a-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2b55a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2b55a-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="2b55a-132">The default output type is text/csv.</span></span> <span data-ttu-id="2b55a-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="2b55a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b55a-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b55a-134">Request headers</span></span>

| <span data-ttu-id="2b55a-135">名称</span><span class="sxs-lookup"><span data-stu-id="2b55a-135">Name</span></span>          | <span data-ttu-id="2b55a-136">说明</span><span class="sxs-lookup"><span data-stu-id="2b55a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2b55a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b55a-137">Authorization</span></span> | <span data-ttu-id="2b55a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b55a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2b55a-140">响应</span><span class="sxs-lookup"><span data-stu-id="2b55a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2b55a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="2b55a-141">CSV</span></span>

<span data-ttu-id="2b55a-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2b55a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2b55a-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2b55a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2b55a-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2b55a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2b55a-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2b55a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2b55a-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2b55a-146">Report Refresh Date</span></span>
- <span data-ttu-id="2b55a-147">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="2b55a-147">Visited Page</span></span>
- <span data-ttu-id="2b55a-148">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="2b55a-148">Viewed Or Edited</span></span>
- <span data-ttu-id="2b55a-149">已同步</span><span class="sxs-lookup"><span data-stu-id="2b55a-149">Synced</span></span>
- <span data-ttu-id="2b55a-150">已内部共享</span><span class="sxs-lookup"><span data-stu-id="2b55a-150">Shared Internally</span></span>
- <span data-ttu-id="2b55a-151">已外部共享</span><span class="sxs-lookup"><span data-stu-id="2b55a-151">Shared Externally</span></span>
- <span data-ttu-id="2b55a-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="2b55a-152">Report Date</span></span>
- <span data-ttu-id="2b55a-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="2b55a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2b55a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="2b55a-154">JSON</span></span>

<span data-ttu-id="2b55a-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="2b55a-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b55a-156">示例</span><span class="sxs-lookup"><span data-stu-id="2b55a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2b55a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="2b55a-157">CSV</span></span>

<span data-ttu-id="2b55a-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="2b55a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2b55a-159">请求</span><span class="sxs-lookup"><span data-stu-id="2b55a-159">Request</span></span>

<span data-ttu-id="2b55a-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b55a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2b55a-161">响应</span><span class="sxs-lookup"><span data-stu-id="2b55a-161">Response</span></span>

<span data-ttu-id="2b55a-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b55a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2b55a-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2b55a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="2b55a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="2b55a-164">JSON</span></span>

<span data-ttu-id="2b55a-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="2b55a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2b55a-166">请求</span><span class="sxs-lookup"><span data-stu-id="2b55a-166">Request</span></span>

<span data-ttu-id="2b55a-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b55a-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2b55a-168">响应</span><span class="sxs-lookup"><span data-stu-id="2b55a-168">Response</span></span>

<span data-ttu-id="2b55a-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b55a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="2b55a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2b55a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
