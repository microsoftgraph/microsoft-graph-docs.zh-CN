---
title: 'reportRoot: getYammerActivityCounts'
description: 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 749db3711cc6d06cb42b14ae95025ec10d4c19d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933622"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="27850-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="27850-103">reportRoot: getYammerActivityCounts</span></span>

> <span data-ttu-id="27850-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="27850-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27850-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27850-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27850-106">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="27850-106">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="27850-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="27850-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="27850-108">权限</span><span class="sxs-lookup"><span data-stu-id="27850-108">Permissions</span></span>

<span data-ttu-id="27850-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27850-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27850-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27850-111">Permission type</span></span>                        | <span data-ttu-id="27850-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27850-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="27850-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27850-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="27850-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27850-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="27850-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27850-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27850-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27850-116">Not supported.</span></span>                           |
| <span data-ttu-id="27850-117">应用</span><span class="sxs-lookup"><span data-stu-id="27850-117">Application</span></span>                            | <span data-ttu-id="27850-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27850-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="27850-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27850-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="27850-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="27850-120">Function parameters</span></span>

<span data-ttu-id="27850-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="27850-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="27850-122">参数</span><span class="sxs-lookup"><span data-stu-id="27850-122">Parameter</span></span> | <span data-ttu-id="27850-123">类型</span><span class="sxs-lookup"><span data-stu-id="27850-123">Type</span></span>   | <span data-ttu-id="27850-124">说明</span><span class="sxs-lookup"><span data-stu-id="27850-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="27850-125">period</span><span class="sxs-lookup"><span data-stu-id="27850-125">period</span></span>    | <span data-ttu-id="27850-126">string</span><span class="sxs-lookup"><span data-stu-id="27850-126">string</span></span> | <span data-ttu-id="27850-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="27850-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="27850-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="27850-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="27850-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="27850-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="27850-130">必需。</span><span class="sxs-lookup"><span data-stu-id="27850-130">Required.</span></span> |

<span data-ttu-id="27850-131">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="27850-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="27850-132">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="27850-132">The default output type is text/csv.</span></span> <span data-ttu-id="27850-133">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="27850-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27850-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="27850-134">Request headers</span></span>

| <span data-ttu-id="27850-135">名称</span><span class="sxs-lookup"><span data-stu-id="27850-135">Name</span></span>          | <span data-ttu-id="27850-136">说明</span><span class="sxs-lookup"><span data-stu-id="27850-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="27850-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="27850-137">Authorization</span></span> | <span data-ttu-id="27850-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27850-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="27850-140">响应</span><span class="sxs-lookup"><span data-stu-id="27850-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="27850-141">CSV</span><span class="sxs-lookup"><span data-stu-id="27850-141">CSV</span></span>

<span data-ttu-id="27850-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="27850-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="27850-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="27850-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="27850-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="27850-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="27850-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="27850-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="27850-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="27850-146">Report Refresh Date</span></span>
- <span data-ttu-id="27850-147">已赞</span><span class="sxs-lookup"><span data-stu-id="27850-147">Liked</span></span>
- <span data-ttu-id="27850-148">已发布</span><span class="sxs-lookup"><span data-stu-id="27850-148">Posted</span></span>
- <span data-ttu-id="27850-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="27850-149">Read</span></span>
- <span data-ttu-id="27850-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="27850-150">Report Date</span></span>
- <span data-ttu-id="27850-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="27850-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="27850-152">JSON</span><span class="sxs-lookup"><span data-stu-id="27850-152">JSON</span></span>

<span data-ttu-id="27850-153">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="27850-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27850-154">示例</span><span class="sxs-lookup"><span data-stu-id="27850-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="27850-155">CSV</span><span class="sxs-lookup"><span data-stu-id="27850-155">CSV</span></span>

<span data-ttu-id="27850-156">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="27850-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="27850-157">请求</span><span class="sxs-lookup"><span data-stu-id="27850-157">Request</span></span>

<span data-ttu-id="27850-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="27850-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="27850-159">响应</span><span class="sxs-lookup"><span data-stu-id="27850-159">Response</span></span>

<span data-ttu-id="27850-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="27850-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="27850-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="27850-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="27850-162">JSON</span><span class="sxs-lookup"><span data-stu-id="27850-162">JSON</span></span>

<span data-ttu-id="27850-163">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="27850-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="27850-164">请求</span><span class="sxs-lookup"><span data-stu-id="27850-164">Request</span></span>

<span data-ttu-id="27850-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="27850-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="27850-166">响应</span><span class="sxs-lookup"><span data-stu-id="27850-166">Response</span></span>

<span data-ttu-id="27850-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="27850-167">The following is an example of the response.</span></span>

> <span data-ttu-id="27850-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="27850-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
