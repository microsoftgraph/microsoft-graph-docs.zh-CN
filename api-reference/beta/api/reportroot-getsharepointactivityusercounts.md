---
title: 'reportRoot: getSharePointActivityUserCounts'
description: 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 025233697300431f05d0ca3d098bc15f71c22f24
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049077"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="4b911-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4b911-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="4b911-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b911-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b911-106">获取活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="4b911-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="4b911-107">如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。</span><span class="sxs-lookup"><span data-stu-id="4b911-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="4b911-108">**注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="4b911-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b911-109">权限</span><span class="sxs-lookup"><span data-stu-id="4b911-109">Permissions</span></span>

<span data-ttu-id="4b911-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b911-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b911-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b911-112">Permission type</span></span>                        | <span data-ttu-id="4b911-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b911-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4b911-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b911-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b911-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b911-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4b911-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b911-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b911-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b911-117">Not supported.</span></span>                           |
| <span data-ttu-id="4b911-118">应用</span><span class="sxs-lookup"><span data-stu-id="4b911-118">Application</span></span>                            | <span data-ttu-id="4b911-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b911-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="4b911-120">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="4b911-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4b911-121">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="4b911-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4b911-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b911-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4b911-123">函数参数</span><span class="sxs-lookup"><span data-stu-id="4b911-123">Function parameters</span></span>

<span data-ttu-id="4b911-124">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4b911-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4b911-125">参数</span><span class="sxs-lookup"><span data-stu-id="4b911-125">Parameter</span></span> | <span data-ttu-id="4b911-126">类型</span><span class="sxs-lookup"><span data-stu-id="4b911-126">Type</span></span>   | <span data-ttu-id="4b911-127">说明</span><span class="sxs-lookup"><span data-stu-id="4b911-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4b911-128">period</span><span class="sxs-lookup"><span data-stu-id="4b911-128">period</span></span>    | <span data-ttu-id="4b911-129">string</span><span class="sxs-lookup"><span data-stu-id="4b911-129">string</span></span> | <span data-ttu-id="4b911-130">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4b911-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4b911-131">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4b911-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4b911-132">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4b911-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4b911-133">必需。</span><span class="sxs-lookup"><span data-stu-id="4b911-133">Required.</span></span> |

<span data-ttu-id="4b911-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b911-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4b911-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="4b911-135">The default output type is text/csv.</span></span> <span data-ttu-id="4b911-136">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="4b911-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b911-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b911-137">Request headers</span></span>

| <span data-ttu-id="4b911-138">名称</span><span class="sxs-lookup"><span data-stu-id="4b911-138">Name</span></span>          | <span data-ttu-id="4b911-139">说明</span><span class="sxs-lookup"><span data-stu-id="4b911-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4b911-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b911-140">Authorization</span></span> | <span data-ttu-id="4b911-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b911-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4b911-143">响应</span><span class="sxs-lookup"><span data-stu-id="4b911-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4b911-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4b911-144">CSV</span></span>

<span data-ttu-id="4b911-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4b911-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4b911-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4b911-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4b911-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4b911-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4b911-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4b911-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4b911-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4b911-149">Report Refresh Date</span></span>
- <span data-ttu-id="4b911-150">访问过的页面</span><span class="sxs-lookup"><span data-stu-id="4b911-150">Visited Page</span></span>
- <span data-ttu-id="4b911-151">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="4b911-151">Viewed Or Edited</span></span>
- <span data-ttu-id="4b911-152">已同步</span><span class="sxs-lookup"><span data-stu-id="4b911-152">Synced</span></span>
- <span data-ttu-id="4b911-153">已内部共享</span><span class="sxs-lookup"><span data-stu-id="4b911-153">Shared Internally</span></span>
- <span data-ttu-id="4b911-154">已外部共享</span><span class="sxs-lookup"><span data-stu-id="4b911-154">Shared Externally</span></span>
- <span data-ttu-id="4b911-155">报表日期</span><span class="sxs-lookup"><span data-stu-id="4b911-155">Report Date</span></span>
- <span data-ttu-id="4b911-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="4b911-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4b911-157">JSON</span><span class="sxs-lookup"><span data-stu-id="4b911-157">JSON</span></span>

<span data-ttu-id="4b911-158">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="4b911-158">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b911-159">示例</span><span class="sxs-lookup"><span data-stu-id="4b911-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4b911-160">CSV</span><span class="sxs-lookup"><span data-stu-id="4b911-160">CSV</span></span>

<span data-ttu-id="4b911-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="4b911-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4b911-162">请求</span><span class="sxs-lookup"><span data-stu-id="4b911-162">Request</span></span>

<span data-ttu-id="4b911-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b911-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="4b911-164">响应</span><span class="sxs-lookup"><span data-stu-id="4b911-164">Response</span></span>

<span data-ttu-id="4b911-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b911-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4b911-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4b911-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4b911-167">JSON</span><span class="sxs-lookup"><span data-stu-id="4b911-167">JSON</span></span>

<span data-ttu-id="4b911-168">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="4b911-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4b911-169">请求</span><span class="sxs-lookup"><span data-stu-id="4b911-169">Request</span></span>

<span data-ttu-id="4b911-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b911-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="4b911-171">响应</span><span class="sxs-lookup"><span data-stu-id="4b911-171">Response</span></span>

<span data-ttu-id="4b911-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b911-172">The following is an example of the response.</span></span>

> <span data-ttu-id="4b911-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4b911-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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


