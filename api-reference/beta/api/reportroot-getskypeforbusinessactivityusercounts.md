---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.openlocfilehash: a012045c58acea9539a9ab92aee55e5d8bb106d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806382"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="f8b92-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f8b92-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

> <span data-ttu-id="f8b92-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8b92-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b92-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8b92-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8b92-107">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="f8b92-107">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="f8b92-108">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="f8b92-108">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="f8b92-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="f8b92-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8b92-110">权限</span><span class="sxs-lookup"><span data-stu-id="f8b92-110">Permissions</span></span>

<span data-ttu-id="f8b92-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8b92-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8b92-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8b92-113">Permission type</span></span>                        | <span data-ttu-id="f8b92-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8b92-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8b92-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b92-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8b92-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8b92-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f8b92-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8b92-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8b92-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8b92-118">Not supported.</span></span>                           |
| <span data-ttu-id="f8b92-119">应用</span><span class="sxs-lookup"><span data-stu-id="f8b92-119">Application</span></span>                            | <span data-ttu-id="f8b92-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8b92-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f8b92-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8b92-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f8b92-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="f8b92-122">Function parameters</span></span>

<span data-ttu-id="f8b92-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="f8b92-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f8b92-124">参数</span><span class="sxs-lookup"><span data-stu-id="f8b92-124">Parameter</span></span> | <span data-ttu-id="f8b92-125">类型</span><span class="sxs-lookup"><span data-stu-id="f8b92-125">Type</span></span>   | <span data-ttu-id="f8b92-126">说明</span><span class="sxs-lookup"><span data-stu-id="f8b92-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8b92-127">period</span><span class="sxs-lookup"><span data-stu-id="f8b92-127">period</span></span>    | <span data-ttu-id="f8b92-128">string</span><span class="sxs-lookup"><span data-stu-id="f8b92-128">string</span></span> | <span data-ttu-id="f8b92-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8b92-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8b92-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="f8b92-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8b92-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="f8b92-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8b92-132">必需。</span><span class="sxs-lookup"><span data-stu-id="f8b92-132">Required.</span></span> |

<span data-ttu-id="f8b92-133">此方法支持`$format`要自定义的响应的[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f8b92-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f8b92-134">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="f8b92-134">The default output type is text/csv.</span></span> <span data-ttu-id="f8b92-135">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="f8b92-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8b92-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8b92-136">Request headers</span></span>

| <span data-ttu-id="f8b92-137">名称</span><span class="sxs-lookup"><span data-stu-id="f8b92-137">Name</span></span>          | <span data-ttu-id="f8b92-138">说明</span><span class="sxs-lookup"><span data-stu-id="f8b92-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f8b92-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b92-139">Authorization</span></span> | <span data-ttu-id="f8b92-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8b92-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f8b92-142">响应</span><span class="sxs-lookup"><span data-stu-id="f8b92-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f8b92-143">CSV</span><span class="sxs-lookup"><span data-stu-id="f8b92-143">CSV</span></span>

<span data-ttu-id="f8b92-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f8b92-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8b92-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="f8b92-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8b92-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="f8b92-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f8b92-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="f8b92-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8b92-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="f8b92-148">Report Refresh Date</span></span>
- <span data-ttu-id="f8b92-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="f8b92-149">Report Date</span></span>
- <span data-ttu-id="f8b92-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="f8b92-150">Report Period</span></span>
- <span data-ttu-id="f8b92-151">对等</span><span class="sxs-lookup"><span data-stu-id="f8b92-151">Peer-to-peer</span></span>
- <span data-ttu-id="f8b92-152">组织</span><span class="sxs-lookup"><span data-stu-id="f8b92-152">Organized</span></span>
- <span data-ttu-id="f8b92-153">参与</span><span class="sxs-lookup"><span data-stu-id="f8b92-153">Participated</span></span>

### <a name="json"></a><span data-ttu-id="f8b92-154">JSON</span><span class="sxs-lookup"><span data-stu-id="f8b92-154">JSON</span></span>

<span data-ttu-id="f8b92-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="f8b92-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b92-156">示例</span><span class="sxs-lookup"><span data-stu-id="f8b92-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f8b92-157">CSV</span><span class="sxs-lookup"><span data-stu-id="f8b92-157">CSV</span></span>

<span data-ttu-id="f8b92-158">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="f8b92-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f8b92-159">请求</span><span class="sxs-lookup"><span data-stu-id="f8b92-159">Request</span></span>

<span data-ttu-id="f8b92-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8b92-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f8b92-161">响应</span><span class="sxs-lookup"><span data-stu-id="f8b92-161">Response</span></span>

<span data-ttu-id="f8b92-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8b92-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f8b92-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="f8b92-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f8b92-164">JSON</span><span class="sxs-lookup"><span data-stu-id="f8b92-164">JSON</span></span>

<span data-ttu-id="f8b92-165">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8b92-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f8b92-166">请求</span><span class="sxs-lookup"><span data-stu-id="f8b92-166">Request</span></span>

<span data-ttu-id="f8b92-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8b92-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f8b92-168">响应</span><span class="sxs-lookup"><span data-stu-id="f8b92-168">Response</span></span>

<span data-ttu-id="f8b92-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8b92-169">The following is an example of the response.</span></span>

> <span data-ttu-id="f8b92-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8b92-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
