---
title: 'reportRoot: getYammerActivityUserCounts'
description: 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。
localization_priority: Normal
ms.openlocfilehash: 04a874a74740eadad72098c68eba5723e6d6368b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887246"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="84d15-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="84d15-103">reportRoot: getYammerActivityUserCounts</span></span>

> <span data-ttu-id="84d15-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84d15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84d15-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84d15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84d15-106">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="84d15-106">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="84d15-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="84d15-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="84d15-108">权限</span><span class="sxs-lookup"><span data-stu-id="84d15-108">Permissions</span></span>

<span data-ttu-id="84d15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84d15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84d15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84d15-111">Permission type</span></span>                        | <span data-ttu-id="84d15-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84d15-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84d15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84d15-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="84d15-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d15-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84d15-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84d15-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84d15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84d15-116">Not supported.</span></span>                           |
| <span data-ttu-id="84d15-117">应用</span><span class="sxs-lookup"><span data-stu-id="84d15-117">Application</span></span>                            | <span data-ttu-id="84d15-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d15-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="84d15-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84d15-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="84d15-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="84d15-120">Function parameters</span></span>

<span data-ttu-id="84d15-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="84d15-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="84d15-122">参数</span><span class="sxs-lookup"><span data-stu-id="84d15-122">Parameter</span></span> | <span data-ttu-id="84d15-123">类型</span><span class="sxs-lookup"><span data-stu-id="84d15-123">Type</span></span>   | <span data-ttu-id="84d15-124">说明</span><span class="sxs-lookup"><span data-stu-id="84d15-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84d15-125">period</span><span class="sxs-lookup"><span data-stu-id="84d15-125">period</span></span>    | <span data-ttu-id="84d15-126">string</span><span class="sxs-lookup"><span data-stu-id="84d15-126">string</span></span> | <span data-ttu-id="84d15-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="84d15-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84d15-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="84d15-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84d15-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="84d15-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="84d15-130">必需。</span><span class="sxs-lookup"><span data-stu-id="84d15-130">Required.</span></span> |

<span data-ttu-id="84d15-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="84d15-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="84d15-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="84d15-132">The default output type is text/csv.</span></span> <span data-ttu-id="84d15-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="84d15-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84d15-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="84d15-134">Request headers</span></span>

| <span data-ttu-id="84d15-135">名称</span><span class="sxs-lookup"><span data-stu-id="84d15-135">Name</span></span>          | <span data-ttu-id="84d15-136">说明</span><span class="sxs-lookup"><span data-stu-id="84d15-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84d15-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="84d15-137">Authorization</span></span> | <span data-ttu-id="84d15-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84d15-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84d15-140">响应</span><span class="sxs-lookup"><span data-stu-id="84d15-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="84d15-141">CSV</span><span class="sxs-lookup"><span data-stu-id="84d15-141">CSV</span></span>

<span data-ttu-id="84d15-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="84d15-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84d15-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="84d15-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84d15-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="84d15-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84d15-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="84d15-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="84d15-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="84d15-146">Report Refresh Date</span></span>
- <span data-ttu-id="84d15-147">已赞</span><span class="sxs-lookup"><span data-stu-id="84d15-147">Liked</span></span>
- <span data-ttu-id="84d15-148">已发布</span><span class="sxs-lookup"><span data-stu-id="84d15-148">Posted</span></span>
- <span data-ttu-id="84d15-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="84d15-149">Read</span></span>
- <span data-ttu-id="84d15-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="84d15-150">Report Date</span></span>
- <span data-ttu-id="84d15-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="84d15-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="84d15-152">JSON</span><span class="sxs-lookup"><span data-stu-id="84d15-152">JSON</span></span>

<span data-ttu-id="84d15-153">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="84d15-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d15-154">示例</span><span class="sxs-lookup"><span data-stu-id="84d15-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="84d15-155">CSV</span><span class="sxs-lookup"><span data-stu-id="84d15-155">CSV</span></span>

<span data-ttu-id="84d15-156">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="84d15-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="84d15-157">请求</span><span class="sxs-lookup"><span data-stu-id="84d15-157">Request</span></span>

<span data-ttu-id="84d15-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84d15-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="84d15-159">响应</span><span class="sxs-lookup"><span data-stu-id="84d15-159">Response</span></span>

<span data-ttu-id="84d15-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84d15-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="84d15-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="84d15-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="84d15-162">JSON</span><span class="sxs-lookup"><span data-stu-id="84d15-162">JSON</span></span>

<span data-ttu-id="84d15-163">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="84d15-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="84d15-164">请求</span><span class="sxs-lookup"><span data-stu-id="84d15-164">Request</span></span>

<span data-ttu-id="84d15-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84d15-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="84d15-166">响应</span><span class="sxs-lookup"><span data-stu-id="84d15-166">Response</span></span>

<span data-ttu-id="84d15-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84d15-167">The following is an example of the response.</span></span>

> <span data-ttu-id="84d15-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="84d15-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
