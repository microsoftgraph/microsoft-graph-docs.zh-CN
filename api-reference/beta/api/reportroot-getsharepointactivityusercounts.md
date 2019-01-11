---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.openlocfilehash: 356f079a1d0836b6cd824a30d6882ed12f0155fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842201"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="a3b68-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a3b68-104">reportRoot: getSharePointActivityUserCounts</span></span>

> <span data-ttu-id="a3b68-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3b68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3b68-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3b68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3b68-107">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a3b68-107">Get the trend in the number of active users.</span></span> <span data-ttu-id="a3b68-108">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="a3b68-108">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="a3b68-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="a3b68-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="a3b68-110">权限</span><span class="sxs-lookup"><span data-stu-id="a3b68-110">Permissions</span></span>

<span data-ttu-id="a3b68-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3b68-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3b68-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3b68-113">Permission type</span></span>                        | <span data-ttu-id="a3b68-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3b68-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a3b68-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b68-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3b68-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3b68-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a3b68-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b68-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3b68-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3b68-118">Not supported.</span></span>                           |
| <span data-ttu-id="a3b68-119">应用</span><span class="sxs-lookup"><span data-stu-id="a3b68-119">Application</span></span>                            | <span data-ttu-id="a3b68-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3b68-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a3b68-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3b68-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a3b68-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="a3b68-122">Function parameters</span></span>

<span data-ttu-id="a3b68-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a3b68-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a3b68-124">参数</span><span class="sxs-lookup"><span data-stu-id="a3b68-124">Parameter</span></span> | <span data-ttu-id="a3b68-125">类型</span><span class="sxs-lookup"><span data-stu-id="a3b68-125">Type</span></span>   | <span data-ttu-id="a3b68-126">说明</span><span class="sxs-lookup"><span data-stu-id="a3b68-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a3b68-127">period</span><span class="sxs-lookup"><span data-stu-id="a3b68-127">period</span></span>    | <span data-ttu-id="a3b68-128">string</span><span class="sxs-lookup"><span data-stu-id="a3b68-128">string</span></span> | <span data-ttu-id="a3b68-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a3b68-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a3b68-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a3b68-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a3b68-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a3b68-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a3b68-132">必需。</span><span class="sxs-lookup"><span data-stu-id="a3b68-132">Required.</span></span> |

<span data-ttu-id="a3b68-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a3b68-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a3b68-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="a3b68-134">The default output type is text/csv.</span></span> <span data-ttu-id="a3b68-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="a3b68-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3b68-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3b68-136">Request headers</span></span>

| <span data-ttu-id="a3b68-137">名称</span><span class="sxs-lookup"><span data-stu-id="a3b68-137">Name</span></span>          | <span data-ttu-id="a3b68-138">说明</span><span class="sxs-lookup"><span data-stu-id="a3b68-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3b68-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3b68-139">Authorization</span></span> | <span data-ttu-id="a3b68-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3b68-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3b68-142">响应</span><span class="sxs-lookup"><span data-stu-id="a3b68-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a3b68-143">CSV</span><span class="sxs-lookup"><span data-stu-id="a3b68-143">CSV</span></span>

<span data-ttu-id="a3b68-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a3b68-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a3b68-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a3b68-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a3b68-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a3b68-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a3b68-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a3b68-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a3b68-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a3b68-148">Report Refresh Date</span></span>
- <span data-ttu-id="a3b68-149">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="a3b68-149">Visited Page</span></span>
- <span data-ttu-id="a3b68-150">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="a3b68-150">Viewed Or Edited</span></span>
- <span data-ttu-id="a3b68-151">已同步</span><span class="sxs-lookup"><span data-stu-id="a3b68-151">Synced</span></span>
- <span data-ttu-id="a3b68-152">已内部共享</span><span class="sxs-lookup"><span data-stu-id="a3b68-152">Shared Internally</span></span>
- <span data-ttu-id="a3b68-153">已外部共享</span><span class="sxs-lookup"><span data-stu-id="a3b68-153">Shared Externally</span></span>
- <span data-ttu-id="a3b68-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="a3b68-154">Report Date</span></span>
- <span data-ttu-id="a3b68-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="a3b68-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a3b68-156">JSON</span><span class="sxs-lookup"><span data-stu-id="a3b68-156">JSON</span></span>

<span data-ttu-id="a3b68-157">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a3b68-157">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b68-158">示例</span><span class="sxs-lookup"><span data-stu-id="a3b68-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a3b68-159">CSV</span><span class="sxs-lookup"><span data-stu-id="a3b68-159">CSV</span></span>

<span data-ttu-id="a3b68-160">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="a3b68-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a3b68-161">请求</span><span class="sxs-lookup"><span data-stu-id="a3b68-161">Request</span></span>

<span data-ttu-id="a3b68-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3b68-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a3b68-163">响应</span><span class="sxs-lookup"><span data-stu-id="a3b68-163">Response</span></span>

<span data-ttu-id="a3b68-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3b68-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a3b68-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a3b68-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a3b68-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a3b68-166">JSON</span></span>

<span data-ttu-id="a3b68-167">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3b68-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a3b68-168">请求</span><span class="sxs-lookup"><span data-stu-id="a3b68-168">Request</span></span>

<span data-ttu-id="a3b68-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3b68-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a3b68-170">响应</span><span class="sxs-lookup"><span data-stu-id="a3b68-170">Response</span></span>

<span data-ttu-id="a3b68-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3b68-171">The following is an example of the response.</span></span>

> <span data-ttu-id="a3b68-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3b68-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
