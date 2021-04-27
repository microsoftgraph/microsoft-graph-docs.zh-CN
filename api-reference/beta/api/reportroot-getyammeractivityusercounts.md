---
title: 'reportRoot: getYammerActivityUserCounts'
description: 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: eb1b80b55a93ccc2eff61fc8eb5ec9046d890f2e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054978"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="7f800-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7f800-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="7f800-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f800-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f800-105">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="7f800-105">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="7f800-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 Microsoft 365 [reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="7f800-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f800-107">权限</span><span class="sxs-lookup"><span data-stu-id="7f800-107">Permissions</span></span>

<span data-ttu-id="7f800-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f800-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f800-110">Permission type</span></span>                        | <span data-ttu-id="7f800-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f800-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f800-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f800-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f800-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f800-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f800-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f800-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f800-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f800-115">Not supported.</span></span>                           |
| <span data-ttu-id="7f800-116">应用</span><span class="sxs-lookup"><span data-stu-id="7f800-116">Application</span></span>                            | <span data-ttu-id="7f800-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f800-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="7f800-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="7f800-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7f800-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="7f800-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7f800-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f800-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7f800-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="7f800-121">Function parameters</span></span>

<span data-ttu-id="7f800-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7f800-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7f800-123">参数</span><span class="sxs-lookup"><span data-stu-id="7f800-123">Parameter</span></span> | <span data-ttu-id="7f800-124">类型</span><span class="sxs-lookup"><span data-stu-id="7f800-124">Type</span></span>   | <span data-ttu-id="7f800-125">说明</span><span class="sxs-lookup"><span data-stu-id="7f800-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f800-126">period</span><span class="sxs-lookup"><span data-stu-id="7f800-126">period</span></span>    | <span data-ttu-id="7f800-127">string</span><span class="sxs-lookup"><span data-stu-id="7f800-127">string</span></span> | <span data-ttu-id="7f800-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7f800-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f800-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7f800-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f800-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7f800-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f800-131">必需。</span><span class="sxs-lookup"><span data-stu-id="7f800-131">Required.</span></span> |

<span data-ttu-id="7f800-132">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f800-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7f800-133">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="7f800-133">The default output type is text/csv.</span></span> <span data-ttu-id="7f800-134">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="7f800-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f800-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f800-135">Request headers</span></span>

| <span data-ttu-id="7f800-136">名称</span><span class="sxs-lookup"><span data-stu-id="7f800-136">Name</span></span>          | <span data-ttu-id="7f800-137">说明</span><span class="sxs-lookup"><span data-stu-id="7f800-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f800-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f800-138">Authorization</span></span> | <span data-ttu-id="7f800-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f800-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f800-141">响应</span><span class="sxs-lookup"><span data-stu-id="7f800-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7f800-142">CSV</span><span class="sxs-lookup"><span data-stu-id="7f800-142">CSV</span></span>

<span data-ttu-id="7f800-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7f800-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f800-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7f800-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f800-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7f800-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f800-146">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7f800-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f800-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7f800-147">Report Refresh Date</span></span>
- <span data-ttu-id="7f800-148">已赞</span><span class="sxs-lookup"><span data-stu-id="7f800-148">Liked</span></span>
- <span data-ttu-id="7f800-149">已发布</span><span class="sxs-lookup"><span data-stu-id="7f800-149">Posted</span></span>
- <span data-ttu-id="7f800-150">已阅读</span><span class="sxs-lookup"><span data-stu-id="7f800-150">Read</span></span>
- <span data-ttu-id="7f800-151">报表日期</span><span class="sxs-lookup"><span data-stu-id="7f800-151">Report Date</span></span>
- <span data-ttu-id="7f800-152">报表周期</span><span class="sxs-lookup"><span data-stu-id="7f800-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7f800-153">JSON</span><span class="sxs-lookup"><span data-stu-id="7f800-153">JSON</span></span>

<span data-ttu-id="7f800-154">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` **[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7f800-154">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f800-155">示例</span><span class="sxs-lookup"><span data-stu-id="7f800-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7f800-156">CSV</span><span class="sxs-lookup"><span data-stu-id="7f800-156">CSV</span></span>

<span data-ttu-id="7f800-157">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="7f800-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7f800-158">请求</span><span class="sxs-lookup"><span data-stu-id="7f800-158">Request</span></span>

<span data-ttu-id="7f800-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f800-159">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7f800-160">响应</span><span class="sxs-lookup"><span data-stu-id="7f800-160">Response</span></span>

<span data-ttu-id="7f800-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f800-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f800-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7f800-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7f800-163">JSON</span><span class="sxs-lookup"><span data-stu-id="7f800-163">JSON</span></span>

<span data-ttu-id="7f800-164">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7f800-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7f800-165">请求</span><span class="sxs-lookup"><span data-stu-id="7f800-165">Request</span></span>

<span data-ttu-id="7f800-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f800-166">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7f800-167">响应</span><span class="sxs-lookup"><span data-stu-id="7f800-167">Response</span></span>

<span data-ttu-id="7f800-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f800-168">The following is an example of the response.</span></span>

> <span data-ttu-id="7f800-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7f800-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
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


