---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: deab88950321bbb94d4bb4992f7fc61cc707b8c9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896712"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="db387-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="db387-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="db387-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db387-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db387-106">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="db387-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="db387-107">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="db387-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="db387-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="db387-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="db387-109">权限</span><span class="sxs-lookup"><span data-stu-id="db387-109">Permissions</span></span>

<span data-ttu-id="db387-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="db387-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="db387-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db387-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db387-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="db387-112">Permission type</span></span>                        | <span data-ttu-id="db387-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db387-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="db387-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db387-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="db387-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db387-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="db387-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db387-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db387-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db387-117">Not supported.</span></span>                           |
| <span data-ttu-id="db387-118">应用</span><span class="sxs-lookup"><span data-stu-id="db387-118">Application</span></span>                            | <span data-ttu-id="db387-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db387-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="db387-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="db387-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="db387-121">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="db387-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="db387-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db387-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="db387-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="db387-123">Function parameters</span></span>

<span data-ttu-id="db387-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="db387-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="db387-125">参数</span><span class="sxs-lookup"><span data-stu-id="db387-125">Parameter</span></span> | <span data-ttu-id="db387-126">类型</span><span class="sxs-lookup"><span data-stu-id="db387-126">Type</span></span>   | <span data-ttu-id="db387-127">说明</span><span class="sxs-lookup"><span data-stu-id="db387-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="db387-128">period</span><span class="sxs-lookup"><span data-stu-id="db387-128">period</span></span>    | <span data-ttu-id="db387-129">string</span><span class="sxs-lookup"><span data-stu-id="db387-129">string</span></span> | <span data-ttu-id="db387-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="db387-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="db387-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="db387-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="db387-132">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="db387-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="db387-133">必需。</span><span class="sxs-lookup"><span data-stu-id="db387-133">Required.</span></span> |

<span data-ttu-id="db387-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db387-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="db387-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="db387-135">The default output type is text/csv.</span></span> <span data-ttu-id="db387-136">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="db387-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db387-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="db387-137">Request headers</span></span>

| <span data-ttu-id="db387-138">名称</span><span class="sxs-lookup"><span data-stu-id="db387-138">Name</span></span>          | <span data-ttu-id="db387-139">说明</span><span class="sxs-lookup"><span data-stu-id="db387-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="db387-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="db387-140">Authorization</span></span> | <span data-ttu-id="db387-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="db387-141">Bearer {token}.</span></span> <span data-ttu-id="db387-142">Required.</span><span class="sxs-lookup"><span data-stu-id="db387-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="db387-143">响应</span><span class="sxs-lookup"><span data-stu-id="db387-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="db387-144">CSV</span><span class="sxs-lookup"><span data-stu-id="db387-144">CSV</span></span>

<span data-ttu-id="db387-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="db387-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="db387-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="db387-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="db387-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="db387-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="db387-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="db387-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="db387-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="db387-149">Report Refresh Date</span></span>
- <span data-ttu-id="db387-150">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="db387-150">Visited Page</span></span>
- <span data-ttu-id="db387-151">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="db387-151">Viewed Or Edited</span></span>
- <span data-ttu-id="db387-152">已同步</span><span class="sxs-lookup"><span data-stu-id="db387-152">Synced</span></span>
- <span data-ttu-id="db387-153">已内部共享</span><span class="sxs-lookup"><span data-stu-id="db387-153">Shared Internally</span></span>
- <span data-ttu-id="db387-154">已外部共享</span><span class="sxs-lookup"><span data-stu-id="db387-154">Shared Externally</span></span>
- <span data-ttu-id="db387-155">报表日期</span><span class="sxs-lookup"><span data-stu-id="db387-155">Report Date</span></span>
- <span data-ttu-id="db387-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="db387-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="db387-157">JSON</span><span class="sxs-lookup"><span data-stu-id="db387-157">JSON</span></span>

<span data-ttu-id="db387-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="db387-158">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db387-159">示例</span><span class="sxs-lookup"><span data-stu-id="db387-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="db387-160">CSV</span><span class="sxs-lookup"><span data-stu-id="db387-160">CSV</span></span>

<span data-ttu-id="db387-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="db387-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="db387-162">请求</span><span class="sxs-lookup"><span data-stu-id="db387-162">Request</span></span>

<span data-ttu-id="db387-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db387-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="db387-164">响应</span><span class="sxs-lookup"><span data-stu-id="db387-164">Response</span></span>

<span data-ttu-id="db387-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db387-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="db387-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="db387-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="db387-167">JSON</span><span class="sxs-lookup"><span data-stu-id="db387-167">JSON</span></span>

<span data-ttu-id="db387-168">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="db387-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="db387-169">请求</span><span class="sxs-lookup"><span data-stu-id="db387-169">Request</span></span>

<span data-ttu-id="db387-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db387-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="db387-171">响应</span><span class="sxs-lookup"><span data-stu-id="db387-171">Response</span></span>

<span data-ttu-id="db387-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db387-172">The following is an example of the response.</span></span>

> <span data-ttu-id="db387-173">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="db387-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db387-174">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="db387-174">All the properties will be returned from an actual call.</span></span>

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
